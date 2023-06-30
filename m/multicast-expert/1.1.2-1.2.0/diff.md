# Comparing `tmp/multicast_expert-1.1.2.tar.gz` & `tmp/multicast_expert-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicast_expert-1.1.2.tar", max compression
+gzip compressed data, was "multicast_expert-1.2.0.tar", max compression
```

## Comparing `multicast_expert-1.1.2.tar` & `multicast_expert-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1068 2022-07-31 02:40:01.128195 multicast_expert-1.1.2/LICENSE
--rw-r--r--   0        0        0     1781 2022-08-14 00:56:27.095503 multicast_expert-1.1.2/multicast_expert/__init__.py
--rw-r--r--   0        0        0     9442 2023-05-16 16:22:20.124465 multicast_expert-1.1.2/multicast_expert/os_multicast.py
--rw-r--r--   0        0        0     8653 2023-05-16 04:15:49.645516 multicast_expert-1.1.2/multicast_expert/rx_socket.py
--rw-r--r--   0        0        0     5353 2023-05-16 16:46:03.132302 multicast_expert-1.1.2/multicast_expert/tx_socket.py
--rw-r--r--   0        0        0     3980 2023-05-16 16:21:52.434761 multicast_expert-1.1.2/multicast_expert/utils.py
--rw-r--r--   0        0        0      552 2023-05-16 16:46:12.582453 multicast_expert-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    17128 2022-08-14 02:29:08.542970 multicast_expert-1.1.2/README.rst
--rw-r--r--   0        0        0    18044 2023-05-16 16:46:48.821217 multicast_expert-1.1.2/setup.py
--rw-r--r--   0        0        0    17838 2023-05-16 16:46:48.822214 multicast_expert-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 03:07:57.033966 multicast_expert-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1781 2023-06-30 03:07:57.035961 multicast_expert-1.2.0/multicast_expert/__init__.py
+-rw-r--r--   0        0        0     9559 2023-06-30 03:08:03.570432 multicast_expert-1.2.0/multicast_expert/os_multicast.py
+-rw-r--r--   0        0        0        0 2023-06-30 03:08:03.570432 multicast_expert-1.2.0/multicast_expert/py.typed
+-rw-r--r--   0        0        0    10758 2023-06-30 03:08:03.571429 multicast_expert-1.2.0/multicast_expert/rx_socket.py
+-rw-r--r--   0        0        0     5612 2023-06-30 03:08:03.572427 multicast_expert-1.2.0/multicast_expert/tx_socket.py
+-rw-r--r--   0        0        0     4356 2023-06-30 03:08:03.572427 multicast_expert-1.2.0/multicast_expert/utils.py
+-rw-r--r--   0        0        0      568 2023-06-30 03:08:03.573424 multicast_expert-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17523 2023-06-30 03:08:03.569435 multicast_expert-1.2.0/README.rst
+-rw-r--r--   0        0        0    18441 2023-06-30 03:09:23.991735 multicast_expert-1.2.0/setup.py
+-rw-r--r--   0        0        0    18233 2023-06-30 03:09:23.992732 multicast_expert-1.2.0/PKG-INFO
```

### Comparing `multicast_expert-1.1.2/LICENSE` & `multicast_expert-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multicast_expert-1.1.2/multicast_expert/__init__.py` & `multicast_expert-1.2.0/multicast_expert/__init__.py`

 * *Files identical despite different names*

### Comparing `multicast_expert-1.1.2/multicast_expert/os_multicast.py` & `multicast_expert-1.2.0/multicast_expert/os_multicast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Script containing the nitty-gritty OS level functions of multicast_expert.
 
 import platform
 import socket
 import struct
 import ctypes
-from typing import List
+from typing import List, Optional, Dict
 from dataclasses import dataclass
 from .utils import is_mac, is_windows
 
 import netifaces
 
 # Import needed Win32 DLL functions
 if is_windows:
@@ -20,17 +20,17 @@
 def iface_ip_to_name(iface_ip: str) -> str:
     """
     Convert a network interface's interface IP into its interface name.
     """
 
     # Go from IP to interface name using netifaces.  To do that, we have to iterate through
     # all of the machine's interfaces
-    iface_name = None
+    iface_name: Optional[str] = None
     for interface in netifaces.interfaces():
-        addresses_at_each_level = netifaces.ifaddresses(interface)
+        addresses_at_each_level: Dict[int, List[Dict[str, str]]] = netifaces.ifaddresses(interface)
         for address_family in [netifaces.AF_INET, netifaces.AF_INET6]:
             if address_family in addresses_at_each_level:
                 for address in addresses_at_each_level[address_family]:
                     if address["addr"] == iface_ip:
                         iface_name = interface
 
     if iface_name is None:
@@ -114,15 +114,15 @@
     Generates an ipv6_mreq structure to be used with IPV6_ADD_MEMBERSHIP.
     """
     # Structure documented here on Windows: https://docs.microsoft.com/en-us/windows/win32/api/ws2ipdef/ns-ws2ipdef-ipv6_mreq
     # and here on Linux: https://github.com/torvalds/linux/blob/3d7cb6b04c3f3115719235cc6866b10326de34cd/include/uapi/linux/in6.h#L60
     return struct.pack("=16sI", socket.inet_pton(socket.AF_INET6, mcast_ip), iface_info.iface_idx)
 
 
-def set_multicast_if(mcast_socket: socket.socket, mcast_ips: List[str], iface_info: IfaceInfo, addr_family: int):
+def set_multicast_if(mcast_socket: socket.socket, mcast_ips: List[str], iface_info: IfaceInfo, addr_family: int) -> None:
     """
     Set the IP_MULTICAST_IF / IPV6_MULTICAST_IF socket option to an interface on a given socket.
     Note that this option needs 4 different code paths to set it, on Windows IPv6 / Windows IPv4 / Unix IPv6 / Unix IPv4
     """
     if is_windows:
         # On Windows, IP_MULTICAST_IF takes just the interface index
         # See docs here: https://docs.microsoft.com/en-us/windows/win32/winsock/ipproto-ip-socket-options
@@ -142,15 +142,15 @@
         else:  # IPv6
             # Linux/Mac IPv6 is same as Windows IPv6.
             # Note: Documentation is very misleading, it does not take a pointer from the Python perspective,
             # it just takes an int!
             mcast_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_IF, struct.pack("I", iface_info.iface_idx))
 
 
-def add_memberships(mcast_socket: socket.socket, mcast_ips: List[str], iface_info: IfaceInfo, addr_family: int):
+def add_memberships(mcast_socket: socket.socket, mcast_ips: List[str], iface_info: IfaceInfo, addr_family: int) -> None:
     """
     Add a non-source-specific membership for the given multicast IPs on the given socket.
     """
 
     for mcast_ip in mcast_ips:
         if is_windows:
             # See docs here: https://docs.microsoft.com/en-us/windows/win32/winsock/ipproto-ip-socket-options
@@ -166,15 +166,15 @@
             if addr_family == socket.AF_INET:
                 mcast_socket.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, make_ip_mreqn_struct(mcast_ip, iface_info))
             else: # IPv6
                 # Note: Docs call the option "IPV6_ADD_MEMBERSHIP" but Python only has "IPV6_JOIN_GROUP"
                 mcast_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_JOIN_GROUP, make_ipv6_mreq_struct(mcast_ip, iface_info))
 
 
-def add_source_specific_memberships(mcast_socket: socket.socket, mcast_ips: List[str], source_ips: List[str], iface_info: IfaceInfo):
+def add_source_specific_memberships(mcast_socket: socket.socket, mcast_ips: List[str], source_ips: List[str], iface_info: IfaceInfo) -> None:
     """
     Add a source-specific membership for the given multicast IPs on the given socket, with the given sources.
     Currently only supports IPv6.
     """
     for mcast_ip in mcast_ips:
         for source_ip in source_ips:
             if is_windows:
@@ -196,8 +196,8 @@
             else:
                 # Struct documented here: https://linux.die.net/man/7/ip
                 mreq_source_bytes = struct.pack("@4s4s4s",
                                                 socket.inet_aton(mcast_ip), # imr_multiaddr
                                                 socket.inet_aton(iface_info.iface_ip), # imr_interface
                                                 socket.inet_aton(source_ip)) # imr_sourceaddr
 
-            mcast_socket.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_SOURCE_MEMBERSHIP, mreq_source_bytes)
+            mcast_socket.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_SOURCE_MEMBERSHIP, mreq_source_bytes) # type: ignore[attr-defined]
```

### Comparing `multicast_expert-1.1.2/multicast_expert/rx_socket.py` & `multicast_expert-1.2.0/multicast_expert/rx_socket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,191 @@
+from __future__ import annotations
+
 import platform
+
+import netifaces
 import select
 import socket
 import struct
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Type, cast, Union
+from types import TracebackType
 import ctypes
 
-from .utils import get_interface_ips, get_default_gateway_iface_ip, validate_mcast_ip, MulticastExpertError, is_mac, is_windows
+from .utils import get_interface_ips, get_default_gateway_iface_ip, validate_mcast_ip, MulticastExpertError, is_mac, is_windows, IPv4Or6Address
 from . import os_multicast, LOCALHOST_IPV6, LOCALHOST_IPV4
 
 class McastRxSocket:
     """
     Class to wrap a socket that receives from one or more multicast groups.
     """
 
-    def __init__(self, addr_family: int, mcast_ips: List[str], port: int, iface_ip: str=None, source_ips: List[str]=None, blocking=True):
+    def __init__(self, addr_family: int, mcast_ips: List[str], port: int, iface_ip: Optional[str] = None, iface_ips: Optional[List[str]] = None, source_ips: Optional[List[str]] = None, blocking: bool = True):
         """
         Create a socket which receives UDP datagrams over multicast.  The socket must be opened
         (e.g. using a with statement) before it can be used.
 
         Note: This socket can only receive multicast traffic, not regular unicast traffic.
 
         Note 2: 
 
         :param addr_family: Sets IPv4 or IPv6 operation.  Either socket.AF_INET or socket.AF_INET6.
         :param mcast_ips: List of all possible multicast IPs that this socket can receive from.
         :param port: The port to listen on.
-        :param iface_ip: Interface IP that this socket sends on.  If left as None, multicast_expert will
-            attempt to guess an interface by using the interface your default gateway is on (aka
-            the one your PC uses to access the internet).  Be careful, this default may not be desired
-            in many cases.  See the docs for details.
+        :param iface_ips: Interface IPs that this socket receives from.  If left as None, multicast_expert will
+            attempt to listen on all (non-loopback) interfaces discovered on your machine.  Be careful, this default 
+            may not be desired in many cases.  See the docs for details.
+        :param iface_ip: Legacy alias for iface_ips.  If this is given and iface_ips is not, this adds the
+            given interface IP to iface_ips.
         :param source_ips: Optional, list of source addresses to restrict the multicast subscription to.  The
             OS will drop messages not from one of these IPs, and may even use special IGMPv3 source-specific
             subscription packets to ask for only those specific multicasts from switches/routers.
             This option is only supported for IPv4, currently no major OS supports it with IPv6.
         :param blocking: Whether reception from this socket blocks.  This can be changed later using settimeout()
         """
         self.addr_family = addr_family
-        self.iface_ip = iface_ip
+        self.iface_ips = iface_ips
         self.mcast_ips = mcast_ips
         self.port = port
         self.source_ips = source_ips
 
         self.is_opened = False
-        self.timeout = None if blocking else 0
+        self.timeout: Optional[float] = None if blocking else 0.0
 
-        if self.iface_ip is None:
-            self.iface_ip = get_default_gateway_iface_ip(self.addr_family)
+        # Handle legacy iface_ip argument if given
+        if iface_ip is not None:
+            if iface_ips is not None:
+                raise MulticastExpertError("Both iface_ips and iface_ip may not be specified at the same time!")
+
+            self.iface_ips = [iface_ip]
+
+        if self.iface_ips is None:
+            self.iface_ips = get_interface_ips(addr_family == socket.AF_INET, addr_family == socket.AF_INET6)
+
+            # Don't include the localhost IPs when listening on all interfaces, as that would cause
+            # us to receive all mcasts sent by the current machine.
+            if self.addr_family == socket.AF_INET6 and LOCALHOST_IPV6 in self.iface_ips:
+                self.iface_ips.remove(LOCALHOST_IPV6)
+            if self.addr_family == socket.AF_INET and LOCALHOST_IPV4 in self.iface_ips:
+                self.iface_ips.remove(LOCALHOST_IPV4)
 
-            if self.iface_ip is None:
+            if len(self.iface_ips) == 0:
                 raise MulticastExpertError(
-                    "iface_ip not specified but unable to determine the default gateway on this machine")
+                    "Unable to discover any listenable interfaces on this machine.")
 
-        # Resolve the interface
-        try:
-            self.iface_info = os_multicast.get_iface_info(self.iface_ip)
-        except KeyError:
-            raise MulticastExpertError(
-                "iface_ip %s does not seem to correspond to a valid interface.  Valid interfaces: %s" %
-                (self.iface_ip, ", ".join(get_interface_ips())))
+        # Resolve the interfaces now.  This prevents having to do this relatively expensive call
+        # multiple times later.
+        self.iface_infos = {}
+        for iface_ip in self.iface_ips:
+            try:
+                self.iface_infos[iface_ip] = os_multicast.get_iface_info(iface_ip)
+            except KeyError:
+                raise MulticastExpertError(
+                    "Interface IP %s does not seem to correspond to a valid interface.  Valid interfaces: %s" %
+                    (iface_ip, ", ".join(get_interface_ips())))
 
         # Sanity check multicast addresses
         for mcast_ip in self.mcast_ips:
             validate_mcast_ip(mcast_ip, self.addr_family)
 
         # Sanity check source_ips
         self.is_source_specific = not (source_ips is None or len(source_ips) == 0)
         if self.is_source_specific and self.addr_family == socket.AF_INET6:
             raise MulticastExpertError("Source-specific multicast currently cannot be used with IPv6!")
 
-    def __enter__(self):
+    def __enter__(self) -> McastRxSocket:
         if self.is_opened:
             raise MulticastExpertError("Attempt to open an McastRxSocket that is already open!")
 
-        # On Windows, we just have to create one socket and bind it to the interface address, then subscribe
-        # to all multicast addresses.
-        # On Unix, we need one socket bound to each multicast address.
-        if is_windows:
-            bind_ip_and_mcast_ips_list = [(self.iface_ip, self.mcast_ips)]
-        else:
-            bind_ip_and_mcast_ips_list = [(mcast_ip, [mcast_ip]) for mcast_ip in self.mcast_ips]
-
         # Create the sockets and set options
         self.sockets = []
-        for bind_ip_and_mcast_ips in bind_ip_and_mcast_ips_list:
 
-            bind_address = bind_ip_and_mcast_ips[0]
-            mcast_ips = bind_ip_and_mcast_ips[1]
+        # On Windows, we have to create a socket and bind it for each interface address, then subscribe
+        # to all multicast addresses on each of those sockets
+        # On Unix, we need one socket bound to each multicast address, and each of those sockets
+        # can receive from all interfaces.
+        if is_windows:
+            for iface_ip in self.iface_ips:
+                new_socket = socket.socket(family=self.addr_family, type=socket.SOCK_DGRAM)
+                new_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
-            new_socket = socket.socket(family=self.addr_family, type=socket.SOCK_DGRAM)
-            new_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+                new_socket.bind((iface_ip, self.port))
 
-            if self.addr_family == socket.AF_INET6 and not (is_windows):
-                # Note: for Unix IPv6, need to specify the scope ID in the bind address in order for link-local mcast addresses to work
-                new_socket.bind((bind_address, self.port, 0, self.iface_info.iface_idx))
-            else:
-                new_socket.bind((bind_address, self.port))
-
-            if self.is_source_specific:
-                os_multicast.add_source_specific_memberships(new_socket, mcast_ips, self.source_ips, self.iface_info)
-            else:
-                os_multicast.add_memberships(new_socket, mcast_ips, self.iface_info, self.addr_family)
-
-            # On Windows, by default, sent packets are looped back to local sockets on the same interface, even for interfaces
-            # that are not loopback.  Change this by disabling IP_MULTICAST_LOOP unless the loopback interface is used.
-            # Note that this is *completely and totally different* from what the Win32 docs say that this option does.
+                if self.is_source_specific:
+                    os_multicast.add_source_specific_memberships(new_socket, self.mcast_ips, cast(List[str], self.source_ips), self.iface_infos[iface_ip])
+                else:
+                    os_multicast.add_memberships(new_socket, self.mcast_ips, self.iface_infos[iface_ip], self.addr_family)
 
-            if is_windows:  
-                loop_enabled = (self.iface_ip == LOCALHOST_IPV4 or self.iface_ip == LOCALHOST_IPV6)
+                # On Windows, by default, sent packets are looped back to local sockets on the same interface, even for interfaces
+                # that are not loopback.  Change this by disabling IP_MULTICAST_LOOP unless the loopback interface is used.
+                # Note: multicast_expert submitted a PR to clarify this in the Windows docs, and it was accepted!
+                loop_enabled = (iface_ip == LOCALHOST_IPV4 or iface_ip == LOCALHOST_IPV6)
                 if self.addr_family == socket.AF_INET:
                     new_socket.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_LOOP, loop_enabled)
                 else:
                     new_socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_LOOP, loop_enabled)
 
-            self.sockets.append(new_socket)
+                self.sockets.append(new_socket)
+        else:
+            for mcast_ip in self.mcast_ips:
+                new_socket = socket.socket(family=self.addr_family, type=socket.SOCK_DGRAM)
+                new_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+
+                if self.addr_family == socket.AF_INET6 and LOCALHOST_IPV6 in self.iface_ips:
+                    # Note: for Unix IPv6, need to specify the scope ID in the bind address in order for link-local mcast addresses to work.
+                    new_socket.bind((mcast_ip, self.port, 0, self.iface_infos[LOCALHOST_IPV6].iface_idx))
+                else:
+                    new_socket.bind((mcast_ip, self.port))
+
+                # Add memberships on each interface
+                for iface_ip in self.iface_ips:
+                    if self.is_source_specific:
+                        os_multicast.add_source_specific_memberships(new_socket, [mcast_ip], cast(List[str], self.source_ips), self.iface_infos[iface_ip])
+                    else:
+                        os_multicast.add_memberships(new_socket, [mcast_ip], self.iface_infos[iface_ip], self.addr_family)
+
+                self.sockets.append(new_socket)
 
         self.is_opened = True
 
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type: Optional[Type[BaseException]], exc: Optional[BaseException], traceback: Optional[TracebackType]) -> None:
 
         if not self.is_opened:
             raise MulticastExpertError("Attempt to close an McastRxSocket that is already closed!")
 
         # Close socket
         for socket in self.sockets:
             socket.close()
         self.is_opened = False
 
-    def recvfrom(self, bufsize=4096, flags=0) -> Optional[Tuple[bytes, Tuple]]:
+    def recvfrom(self, bufsize: int = 4096, flags: int = 0) -> Optional[Tuple[bytes, IPv4Or6Address]]:
         """
         Receive a UDP packet from the socket, returning the bytes and the sender address.
         This respects the current blocking and timeout settings.
 
         The "bufsize" and "flags" arguments have the same meaning as the arguments to socket.recv(), see the
         manual for that function for details.
 
         :return: Tuple of (bytes, address).  For IPv4, address is a tuple of IP address (str) and port number.
-            For IPv6, address is a tuple of IP address (str), port number, flow info, and scope ID.
+            For IPv6, address is a tuple of IP address (str), port number, flow info (int), and scope ID (int).
             If no packets were received (nonblocking mode or timeout), None is returned.
         """
 
         # Use select() to find a socket that is ready for reading
         read_list, write_list, exception_list = select.select(self.sockets, [], [], self.timeout)
 
         if len(read_list) == 0:
             # No data to read
             return None
 
         # Since we only want to return one packet at a time, just pick the first readable socket.
-        return read_list[0].recvfrom(bufsize, flags)
+        return cast(Tuple[bytes, IPv4Or6Address], read_list[0].recvfrom(bufsize, flags))
 
-    def recv(self, bufsize=4096, flags=0) -> Optional[bytes]:
+    def recv(self, bufsize: int = 4096, flags: int = 0) -> Optional[bytes]:
         """
         Receive a UDP packet from the socket, returning the bytes.
         This respects the current blocking and timeout settings.
 
         Note: If you need information about the sender of the packet, use recvfrom() instead.
 
         The "bufsize" and "flags" arguments have the same meaning as the arguments to socket.recv(), see the
@@ -172,15 +202,15 @@
     def filenos(self) -> List[int]:
         """
         Get a list of the socket file descriptor(s) used by this socket.  You can use this with the select module
         to implement blocking I/O on multiple different multicast sockets.
         """
         return [socket.fileno() for socket in self.sockets]
 
-    def settimeout(self, timeout: float):
+    def settimeout(self, timeout: float) -> None:
         """
         Set the timeout on socket operations.  Behavior depends on the value passed for timeout:
 
         * Number > 0: Receiving packets will abort if more than timeout seconds elapse while waiting for a packet.
         * 0: Socket will be put in nonblocking mode
         * None: Socket will block forever (the default)
         """
```

### Comparing `multicast_expert-1.1.2/multicast_expert/tx_socket.py` & `multicast_expert-1.2.0/multicast_expert/tx_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from __future__ import annotations
+
 import platform
 import socket
 import struct
-from typing import List, Tuple
+from typing import List, Tuple, Optional, Type
+from types import TracebackType
 import ctypes
 
-from .utils import get_interface_ips, validate_mcast_ip, get_default_gateway_iface_ip, MulticastExpertError, is_mac, is_windows
+from .utils import get_interface_ips, validate_mcast_ip, get_default_gateway_iface_ip, MulticastExpertError, is_mac, is_windows, IPv4Or6Address
 from . import os_multicast, LOCALHOST_IPV4, LOCALHOST_IPV6
 
+
 class McastTxSocket:
     """
     Class to wrap a socket that sends to one or more multicast groups.
     """
 
-    def __init__(self, addr_family: int, mcast_ips: List[str], iface_ip: str=None, ttl: int=1):
+    def __init__(self, addr_family: int, mcast_ips: List[str], iface_ip: Optional[str] = None, ttl: int = 1):
         """
         Create a socket which transmits UDP datagrams over multicast.  The socket must be opened
         (e.g. using a with statement) before it can be used.
 
         :param addr_family: Sets IPv4 or IPv6 operation.  Either socket.AF_INET or socket.AF_INET6.
         :param mcast_ips: List of all possible multicast IPs that this socket can send to.
         :param iface_ip: Interface IP that this socket sends on.  If left as None, multicast_expert will
@@ -48,15 +52,15 @@
             raise MulticastExpertError("iface_ip %s does not seem to correspond to a valid interface.  Valid interfaces: %s" %
                                        (self.iface_ip, ", ".join(get_interface_ips())))
 
         # Sanity check multicast addresses
         for mcast_ip in self.mcast_ips:
             validate_mcast_ip(mcast_ip, self.addr_family)
 
-    def __enter__(self):
+    def __enter__(self) -> McastTxSocket:
         if self.is_opened:
             raise MulticastExpertError("Attempt to open an McastTxSocket that is already open!")
 
         # Open the socket and set options
         self.socket = socket.socket(family=self.addr_family, type=socket.SOCK_DGRAM)
         self.socket.bind((self.iface_ip, 0)) # Bind to any available port
 
@@ -82,30 +86,30 @@
             else:
                 self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_MULTICAST_LOOP, enable_loopback)
 
         self.is_opened = True
 
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type: Optional[Type[BaseException]], exc: Optional[BaseException], traceback: Optional[TracebackType]) -> None:
 
         if not self.is_opened:
             raise MulticastExpertError("Attempt to close an McastTxSocket that is already closed!")
 
         # Close socket
         self.socket.close()
         self.is_opened = False
 
-    def sendto(self, bytes: bytes, address: Tuple[str, int]):
+    def sendto(self, bytes: bytes, address: IPv4Or6Address) -> None:
         """
         Send a UDP datagram containing the given bytes out of the socket to the given destination
         address.
 
-        :param bytes Bytes to send:
-        :param address Tuple of the destination multicast address and the destination port:
+        :param bytes: Bytes to send
+        :param address: Tuple of the destination multicast address and the destination port
         """
 
         if address[0] not in self.mcast_ips_set:
             raise MulticastExpertError("The given destination address (%s) was not one of the addresses given for this McastTxSocket to transmit to!" % (address[0], ))
 
         self.socket.sendto(bytes, address)
 
@@ -115,8 +119,8 @@
         """
         return self.socket.fileno()
 
     def getsockname(self) -> Tuple[str, int]:
         """
         Get the local IP and port that this socket bound itself to.
         """
-        return self.socket.getsockname()
+        return self.socket.getsockname()  # type: ignore[no-any-return]
```

### Comparing `multicast_expert-1.1.2/multicast_expert/utils.py` & `multicast_expert-1.2.0/multicast_expert/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import socket
-from typing import List, Dict, Optional
+from typing import List, Dict, Optional, Union, Tuple
 import ipaddress
 import platform
 
 import netifaces
 
 is_windows = platform.system() == "Windows"
 is_mac = platform.system() == "Darwin"
 
+
+# Type which can represent an IPv4 or an IPv6 address.
+# For IPv4, address is a tuple of IP address (str) and port number.
+# For IPv6, address is a tuple of IP address (str), port number, flow info (int), and scope ID (int).
+IPv4Or6Address = Union[Tuple[str, int], Tuple[str, int, int, int]]
+
+
 # Exception class for this library
 class MulticastExpertError(RuntimeError):
     pass
 
 
-def get_interface_ips(include_ipv4=True, include_ipv6=True) -> List[str]:
+def get_interface_ips(include_ipv4: bool = True, include_ipv6: bool = True) -> List[str]:
     """
     Use this function to get a list of all the interface IP addresses available on this machine.
     Should be useful for generating help menus / info messages / etc.
     This is a thin wrapper around the netifaces library's functionality.
 
     :param include_ipv4: If true, IPv4 addresses will be included in the results
     :param include_ipv6: If true, IPv6 addresses will be included in the results
 
     :return: List of the interface IP of every interface on your machine, as a string.
     """
 
     ip_list = []
     for interface in netifaces.interfaces():
 
-        all_addresses: List[Dict] = []
+        all_addresses: List[Dict[str, str]] = []
         addresses_at_each_level = netifaces.ifaddresses(interface)
 
         if include_ipv4:
             # Note: Check needed because some interfaces do not have an ipv4 or ipv6 address
             if netifaces.AF_INET in addresses_at_each_level:
                 all_addresses.extend(addresses_at_each_level[netifaces.AF_INET])
 
@@ -81,21 +88,21 @@
     if not addr_family in gateways["default"]:
         return None
 
     default_gateway = gateways["default"][addr_family]
     default_gateway_iface = default_gateway[1] # element 1 is the iface name, per the docs
 
     # Now, use the interface name to get the IP address of that interface
-    interface_addresses = netifaces.ifaddresses(default_gateway_iface)
+    interface_addresses: Dict[int, List[Dict[str, str]]] = netifaces.ifaddresses(default_gateway_iface)
     if addr_family not in interface_addresses:
         return None
     return interface_addresses[addr_family][0]["addr"]
 
 
-def validate_mcast_ip(mcast_ip: str, addr_family: int):
+def validate_mcast_ip(mcast_ip: str, addr_family: int) -> None:
     """
     Validate that the given mcast_ip is a valid multicast address in the given addr family (IPv4 or IPv6).
     An exception is thrown if validation fails.
     """
     address_obj = ipaddress.ip_address(mcast_ip)
     if not address_obj.is_multicast:
         raise MulticastExpertError("mcast_ip %s is not a multicast address!" % (mcast_ip,))
```

### Comparing `multicast_expert-1.1.2/pyproject.toml` & `multicast_expert-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "multicast_expert"
-version = "1.1.2"
+version = "1.2.0"
 description = "A library to take the fiddly parts out of multicast networking!"
 authors = ["Jamie Smith <jsmith@crackofdawn.onmicrosoft.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/multiplemonomials/multicast_expert"
 
 [tool.poetry.dependencies]
 python = "^3.8" # Need Python 3.8 for socket.IPPROTO_IPV6
 netifaces = "0.*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
+mypy = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multicast_expert-1.1.2/README.rst` & `multicast_expert-1.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 *******************
 Multicasting Basics
 *******************
 
 Before I can explain how to use this library, I first need to explain the basics of multicasting itself.  There's not a lot of info out there on the net about how to do multicasting right, and much of what there is is buried deep in OS documentation.  So let's go over some of the basic concepts first.
 
-First and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Multicasting happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to one specific network interface that it will use.  There is no such thing as "bind to 0.0.0.0" or "listen on all addresses"!
+First and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Sending multicasts happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to a specific network interface that it will use.  At the OS level, there is no such thing as "bind to 0.0.0.0" or "listen on all interface"!
+
+However, multicast_expert does allow an "multi-interface" mode which combines together multiple OS sockets to allow listening for incoming multicasts on several or all network interfaces.  This allows "bind to 0.0.0.0"-like behavior for Rx sockets only!
 
 Now that we've gotten that out of the way, we can cover the four essential topics for multicast: multicast addresses, understanding network routing, creating a transmitter, and creating a receiver.
 
 Multicast Addresses
 ===================
 A multicast IPv4 address is defined as any IPv4 address whose most significant four bits are "1110".  This means any IP address whose first number is in the range of 224 through 239 (0xE0-0xEF) is a multicast address.  Similarly, for IPv6, any address whose first byte is 0xFF is a multicast address.
 
@@ -47,15 +49,15 @@
 Box                                       What does it do with multicast packets?
 ========================================= ============================================
 Ethernet Switch (No IGMP Snooping)        Forwards to all hosts
 Ethernet Switch (IGMP Snooping Enabled)   Forwards to any hosts that have subscribed
 Router                                    Depends on configuration.
 ========================================= ============================================
 
-**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I've seen a number of devices that do not implement the standard as I've written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which worked fine out of the box but started dropping most multicast traffic when IGMP snooping was enabled!
+**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I've seen a number of devices that do not implement the standard as I've written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which seemed to work fine initially but started dropping most multicast traffic when IGMP snooping was enabled!
 
 Since lots of devices come with weird multicast settings out of the box, prepare to have to check and fix the configuration on each switch/device when you start using multicast on your network.
 
 Sending Multicasts
 ===================
 
 To send multicasts, an application can pretty much just create a normal UDP socket and have it send packets to a multicast IP address.  However, there is one additional piece needed, which is that the OS needs to be told which interface to send the multicasts on.  This is always done using the IP_MULTICAST_IF setsockopt() option, but the exact syntax and procedure for using this option differs by OS.  Luckily, Multicast Expert takes care of that for you!
@@ -123,20 +125,20 @@
 Q: Do McastRxSockets receive regular (unicast) UDP packets going to the same interface and port?
     A: On Windows, yes.  On Unix, no.  Unfortunately, this is a platform difference that I haven't found an easy way to work around.
 
 Q: Can I create multiple McastRxSockets on the same port and interface?
     A: As long as they have different mcast addresses, then yes, this works how you'd expect.
 
 Q: Is it possible to receive multicasts on all interfaces with a single socket?
-    A: For reception, this should be possible; it may be implemented in a future version of the library.
+    A: Yes!  As of multicast_expert 1.2.0, the default behavior of McastRxSocket, when you do not pass any interface IP addresses explicitly, is to listen on all non-loopback interfaces of the machine.
 
 Q: Why are my multicasts to the loopback device not going through in Linux?
     A: Linux seems to be very picky about what it allows through loopback.  First of all, you need to use ``ip route`` to add a route directing your multicast address to the ``lo`` interface.  For example, the command ``sudo ip route add 239.2.2.0/24 dev lo`` would allow any multicasts in the 239.2.2.x range through loopback.
 
-    Additionally, for IPv6, I have found that multicasts to addresses that don't start with ``ffx1`` (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...
+    Additionally, for IPv6, I have found that multicasts to addresses that don't start with ``ffx1`` for any value of x (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...
 
 Q: My multicasts aren't being received in Linux, even though I see them coming in in packet dumps.
     A: On Linux, you must also be careful of a kernel feature called Reverse Path Filtering (RPF).  You see, in most cases, multicast doesn't care about unicast IPs or subnets -- you can quite easily have a machine with IP 10.0.0.1 send multicasts to 192.168.1.2, even though those are on different subnets so they can't normally communicate.  However, RPF throws a wrench in this.  In its default "loose" mode (setting 2), it blocks reception of IP packets if they come from an IP address not reachable by any interface.  So, for example, if you receive a multicast from 10.0.0.1 but you only have routes in your routing table for 192.168.x.x IP addresses, the kernel will summarily drop the packet.  The easiest fix is to label one of your network interfaces as a default route.  This makes all IP addresses reachable from an interface, so all packets will be able to get by the check.
 
     RPF's "strict" mode (setting 1) is even worse.  It applies the same check, but on a per-interface level.  So, in order to receive packets from multicast address X, each individual interface must have a routing rule permitting it to send packets to X.  If this is too much of a pain to set up, you can turn RPF off using sysctl (`this seems like a decent guide <https://access.redhat.com/solutions/53031#:~:text=rp_filter%20parameter%20only%20has%20two,default%20is%201%20(loose).>`_).  Just remember to change it both for the "all" interface and for whichever interfaces you want to affect -- the kernel takes the stricter of the two values.
 
     If RPF isn't the problem, you may also want to check any firewalls (firewalld/iptables) and see if those are blocking multicast packets.
```

### Comparing `multicast_expert-1.1.2/setup.py` & `multicast_expert-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces<1.0.0']
 
 setup_kwargs = {
     'name': 'multicast-expert',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': 'A library to take the fiddly parts out of multicast networking!',
-    'long_description': '###########################\nMulticast Expert for Python\n###########################\n\nMulticasting is one of the cooler features of Internet Protocol (IP).  It allows a single source to send out IP packets (usually UDP) which are then received by multiple other devices on the network.  No configuration in advance is needed -- the sender just sends packets, and other devices may subscribe to these packets at their leisure.  Using a protocol called IGMP, computers and network switches communicate to ensure that the multicasts are only sent where they are needed, and not anywhere else.  It\'s great for applications such as audio/video transmission or distributed systems where you need to send out data to many different machines on a network.\n\nIdeally, multicasting is as simple as sending a packet to a specific multicast address, and then having certain other machines receive it.  It looks a bit like this:\n\n.. image:: https://app.box.com/shared/static/ftsh3tq2gvrzibhqwr26n1nvwqazcmlu.png\n    :alt: Diagram of a multicast packet being sent on a network\n\nOf course, in practice, things are a bit more complicated -- chiefly because using multicast requires setting additional socket options whose values and formats often differ by OS.  To that end, this library was created, so that you can use multicast networking without having to mess around with low level OS stuff.  Multicast Expert includes all the required pieces to create and use IPv4 and IPv6 multicast sockets on Windows, Mac, and Linux.\n\n*******************\nMulticasting Basics\n*******************\n\nBefore I can explain how to use this library, I first need to explain the basics of multicasting itself.  There\'s not a lot of info out there on the net about how to do multicasting right, and much of what there is is buried deep in OS documentation.  So let\'s go over some of the basic concepts first.\n\nFirst and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Multicasting happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to one specific network interface that it will use.  There is no such thing as "bind to 0.0.0.0" or "listen on all addresses"!\n\nNow that we\'ve gotten that out of the way, we can cover the four essential topics for multicast: multicast addresses, understanding network routing, creating a transmitter, and creating a receiver.\n\nMulticast Addresses\n===================\nA multicast IPv4 address is defined as any IPv4 address whose most significant four bits are "1110".  This means any IP address whose first number is in the range of 224 through 239 (0xE0-0xEF) is a multicast address.  Similarly, for IPv6, any address whose first byte is 0xFF is a multicast address.\n\nWhen a network interface (e.g. your Ethernet card) sees a packet going to a multicast IP address, it processes it differently.  The exact specifics are outside of the scope of this document and depend on the specific medium, but often it will mark that packet as multicast at the link layer too, e.g. by giving it a special destination MAC address.  This ensures that the packet is delivered correctly by the link layer.\n\nIf you are simply trying to receive existing multicast packets, all you need to know is the group address that the multicasts are being sent on.  But if you\'re trying to build your own application that communicates via multicast, you\'ll need to select an IPv4 or IPv6 multicast address to use for it.  Many of these addresses have to be officially assigned by IANA (the `wikipedia page on multicast addresses <https://en.wikipedia.org/wiki/Multicast_address#IPv4>`_ has the full details), though IP addresses in the 239.x.x.x range are "administratively scoped" and available for private use on LANs.\n\nMulticast Routing in Networks\n=============================\nCompared to regular IP packets, multicast packets are handled differently by networking devices such as Ethernet switches and routers.  It\'s all too easy to forget to take this into account, and then find yourself asking "wait, why am I not receiving any multicast traffic", or even "wait, why am I receiving *all of the multicasts* that I didn\'t ask for?"  This section will go over some basics of how multicast packets move through Ethernet networks.  Other networks may differ in the specifics, but the basic concepts should be similar.\n\nFor a simple ("unmanaged") Ethernet switch, its handling of multicast packets is very simple.  It simply treats them like broadcasts, and forwards them to every other port of the switch.\n\nAs you might imagine, if you have a large network full of multicast users, and switches are broadcasting every message everywhere, you could get some pretty awful network congestion.  To combat this, more complex ("managed") Ethernet switches often have a feature called "IGMP snooping".  When a switch has this setting enabled, it listens for what\'s called an "IGMP join message" to be sent by a host.  This message is automatically sent by your OS whenever you open a multicast receive socket, and indicates that host X wants to receive traffic going to multicast address Y.  When the switch sees one of these messages, it automatically begins routing traffic going to multicast address Y into host X\'s network link.  No IGMP join message?  No multicasts for you.\n\nNote: for IPv6, MLD messages are used instead of IGMP, but they do pretty much the same thing.\n\nLast but not least, routers.  In contrast to Ethernet switches, which connect individual hosts together, routers connect entire networks together.  They have quite a bit more logic and generally require at least some manual configuration of what packets are routed where.  Often, multicasts are just used within the local network and are dropped by routers (you can guarantee this by setting the Time To Live to 1, forcing them to be dropped by any router).  However, the specifics depend on the router configuration, and often individual multicast addresses are treated differently.  If you really do need to pass multicasts through a router, you should contact your ISP or your network admin to verify the router settings.\n\nIn conclusion, here\'s a table of how different boxes handle multicasts:\n\n========================================= ============================================\nBox                                       What does it do with multicast packets?\n========================================= ============================================\nEthernet Switch (No IGMP Snooping)        Forwards to all hosts\nEthernet Switch (IGMP Snooping Enabled)   Forwards to any hosts that have subscribed\nRouter                                    Depends on configuration.\n========================================= ============================================\n\n**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I\'ve seen a number of devices that do not implement the standard as I\'ve written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which worked fine out of the box but started dropping most multicast traffic when IGMP snooping was enabled!\n\nSince lots of devices come with weird multicast settings out of the box, prepare to have to check and fix the configuration on each switch/device when you start using multicast on your network.\n\nSending Multicasts\n===================\n\nTo send multicasts, an application can pretty much just create a normal UDP socket and have it send packets to a multicast IP address.  However, there is one additional piece needed, which is that the OS needs to be told which interface to send the multicasts on.  This is always done using the IP_MULTICAST_IF setsockopt() option, but the exact syntax and procedure for using this option differs by OS.  Luckily, Multicast Expert takes care of that for you!\n\nReceiving Multicasts\n====================\n\nTo receive multicasts, essentially two things need to happen.  First, your OS needs to be told to send out an IGMP join message, telling other devices on the network to send multicast packets your way.  This generally happens as a side effect of enabling the IP_ADD_MEMBERSHIP socket option (or one of its variants) on a socket.  Then, the OS network stack needs to be configured to forward multicast packets which arrive on the given interface to your application.  This process is pretty different on Windows and Unix.\n\nOn Windows, multicast sockets are bound to a given port and interface (using bind()) when they are initially created.  Then, IP_ADD_MEMBERSHIP commands are used to further associate them with individual multicast addresses, so that when a packet is received to that multicast addr, it goes to the correct socket.  This is convenient as it means one socket can use multiple multicast groups and still not receive unwanted traffic from other groups that use the same port.  However, there\'s no way to block unicast traffic going to that interface and port from also being received by the multicast socket.\n\nBut on Unix, the situation is a bit different.  The IP_ADD_MEMBERSHIP command does not directly set up filtering by multicast address, it pretty much just sends the IGMP join message and opens the interface to receive packets going to the multicast address.  It does not directly associate the socket with the multicast address, it\'s still a "regular" UDP socket.  So, if you were to take a multicast socket and bind it to 0.0.0.0, it would end up receiving all UDP traffic on the port number, even traffic to other multicast addresses or to the unicast address.  The only way to fix this is to bind the socket to the specific multicast address instead, causing any traffic with a different destination address to not be accepted by the socket.  Unfortunately, a socket can only be bound to one destination address at a time, so this means multicast expert needs to create a different socket under the hood for each multicast address you want to listen on.\n\n**********************\nUsing Multicast Expert\n**********************\n\nNow let\'s get into some actual code examples.  Now first, before we can create any sockets, we need to find the interface address we want to use (see above).  Luckily, Multicast Expert comes with a convenient function to list all available network interfaces:\n\n>>> import multicast_expert\n>>> multicast_expert.get_interface_ips(include_ipv4=True, include_ipv6=False)\n[\'192.168.0.248\', \'192.168.153.1\', \'127.0.0.1\']\n\n(note that this function is a wrapper around the netifaces library, which provides quite a bit more functionality if you need it)\n\nBut which of those is the interface we actually want to use?  Well, that depends on your specific nework setup, but to make an educated guess, we also have a function to get the interface your machine uses to contact the internet.  This is not always correct but will work for many network setups.\n\n>>> multicast_expert.get_default_gateway_iface_ip_v4()\n\'192.168.0.248\'\n\nTransmitting Multicasts\n=======================\n\nTo send some data to a multicast, use the McastTxSocket class.  This wraps a socket internally, and does all the hard work of configuring it correctly for multicast.  For now we will use \'239.1.2.3\' as our multicast address since it\'s in the administratively scoped block.\n\nThe following block shows how to create a Tx socket and send some data:\n\n>>> import socket\n>>> with multicast_expert.McastTxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], iface_ip=\'192.168.0.248\') as mcast_tx_sock:\n...     mcast_tx_sock.sendto(b\'Hello World\', (\'239.1.2.3\', 12345))\n\nNote: when you construct the socket, you have to pass in all of the multicast IPs that you will want to use the socket to send to.  These must be known in advance in order to configure socket options correctly.\n\nNote 2: If you omitted the iface_ip= argument, the get_default_gateway_iface_ip_v4() function would have been called to guess the iface ip.  So, we could have omitted this argument for the same result.\n\nReceiving Multicasts\n====================\n\nTo receive from one or more multicast addresses, use the McastRxSocket class.  For example:\n\n>>> with multicast_expert.McastRxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], port=12345, iface_ip=\'192.168.0.248\') as mcast_rx_sock:\n...     bytes, src_address = mcast_rx_sock.recvfrom()\n\nThe above code will listen on the 239.1.2.3 multicast address, and will block until a packet is received.  To change the blocking behavior, use the settimeout() function.\n\nFull Example\n============\nFor a complete example of how to use this library, see the system test script `here <https://github.com/multiplemonomials/multicast_expert/blob/main/examples/mcast_communicator.py>`_.\n\nFAQ\n===\nQ: What happens if an interface changes IP address (e.g. due to the user modifying a static IP) after I create a multicast socket on that interface?\n    A: On all machines tested so far, multicast sockets will stick with their assigned interface once created, even if the IP of that interface changes or it is brought down.\n\nQ: Do McastRxSockets receive regular (unicast) UDP packets going to the same interface and port?\n    A: On Windows, yes.  On Unix, no.  Unfortunately, this is a platform difference that I haven\'t found an easy way to work around.\n\nQ: Can I create multiple McastRxSockets on the same port and interface?\n    A: As long as they have different mcast addresses, then yes, this works how you\'d expect.\n\nQ: Is it possible to receive multicasts on all interfaces with a single socket?\n    A: For reception, this should be possible; it may be implemented in a future version of the library.\n\nQ: Why are my multicasts to the loopback device not going through in Linux?\n    A: Linux seems to be very picky about what it allows through loopback.  First of all, you need to use ``ip route`` to add a route directing your multicast address to the ``lo`` interface.  For example, the command ``sudo ip route add 239.2.2.0/24 dev lo`` would allow any multicasts in the 239.2.2.x range through loopback.\n\n    Additionally, for IPv6, I have found that multicasts to addresses that don\'t start with ``ffx1`` (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...\n\nQ: My multicasts aren\'t being received in Linux, even though I see them coming in in packet dumps.\n    A: On Linux, you must also be careful of a kernel feature called Reverse Path Filtering (RPF).  You see, in most cases, multicast doesn\'t care about unicast IPs or subnets -- you can quite easily have a machine with IP 10.0.0.1 send multicasts to 192.168.1.2, even though those are on different subnets so they can\'t normally communicate.  However, RPF throws a wrench in this.  In its default "loose" mode (setting 2), it blocks reception of IP packets if they come from an IP address not reachable by any interface.  So, for example, if you receive a multicast from 10.0.0.1 but you only have routes in your routing table for 192.168.x.x IP addresses, the kernel will summarily drop the packet.  The easiest fix is to label one of your network interfaces as a default route.  This makes all IP addresses reachable from an interface, so all packets will be able to get by the check.\n\n    RPF\'s "strict" mode (setting 1) is even worse.  It applies the same check, but on a per-interface level.  So, in order to receive packets from multicast address X, each individual interface must have a routing rule permitting it to send packets to X.  If this is too much of a pain to set up, you can turn RPF off using sysctl (`this seems like a decent guide <https://access.redhat.com/solutions/53031#:~:text=rp_filter%20parameter%20only%20has%20two,default%20is%201%20(loose).>`_).  Just remember to change it both for the "all" interface and for whichever interfaces you want to affect -- the kernel takes the stricter of the two values.\n\n    If RPF isn\'t the problem, you may also want to check any firewalls (firewalld/iptables) and see if those are blocking multicast packets.\n\nQ: If I have a socket that receives from multiple mcast addresses, say A and B, and I receive a packet, how do I tell whether the packet was sent to multicast address A or B?\n    A: You can\'t, or at least I haven\'t found a way to do this from Python.  You\'ll need to create multiple sockets if you need this information.',
+    'long_description': '###########################\nMulticast Expert for Python\n###########################\n\nMulticasting is one of the cooler features of Internet Protocol (IP).  It allows a single source to send out IP packets (usually UDP) which are then received by multiple other devices on the network.  No configuration in advance is needed -- the sender just sends packets, and other devices may subscribe to these packets at their leisure.  Using a protocol called IGMP, computers and network switches communicate to ensure that the multicasts are only sent where they are needed, and not anywhere else.  It\'s great for applications such as audio/video transmission or distributed systems where you need to send out data to many different machines on a network.\n\nIdeally, multicasting is as simple as sending a packet to a specific multicast address, and then having certain other machines receive it.  It looks a bit like this:\n\n.. image:: https://app.box.com/shared/static/ftsh3tq2gvrzibhqwr26n1nvwqazcmlu.png\n    :alt: Diagram of a multicast packet being sent on a network\n\nOf course, in practice, things are a bit more complicated -- chiefly because using multicast requires setting additional socket options whose values and formats often differ by OS.  To that end, this library was created, so that you can use multicast networking without having to mess around with low level OS stuff.  Multicast Expert includes all the required pieces to create and use IPv4 and IPv6 multicast sockets on Windows, Mac, and Linux.\n\n*******************\nMulticasting Basics\n*******************\n\nBefore I can explain how to use this library, I first need to explain the basics of multicasting itself.  There\'s not a lot of info out there on the net about how to do multicasting right, and much of what there is is buried deep in OS documentation.  So let\'s go over some of the basic concepts first.\n\nFirst and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Sending multicasts happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to a specific network interface that it will use.  At the OS level, there is no such thing as "bind to 0.0.0.0" or "listen on all interface"!\n\nHowever, multicast_expert does allow an "multi-interface" mode which combines together multiple OS sockets to allow listening for incoming multicasts on several or all network interfaces.  This allows "bind to 0.0.0.0"-like behavior for Rx sockets only!\n\nNow that we\'ve gotten that out of the way, we can cover the four essential topics for multicast: multicast addresses, understanding network routing, creating a transmitter, and creating a receiver.\n\nMulticast Addresses\n===================\nA multicast IPv4 address is defined as any IPv4 address whose most significant four bits are "1110".  This means any IP address whose first number is in the range of 224 through 239 (0xE0-0xEF) is a multicast address.  Similarly, for IPv6, any address whose first byte is 0xFF is a multicast address.\n\nWhen a network interface (e.g. your Ethernet card) sees a packet going to a multicast IP address, it processes it differently.  The exact specifics are outside of the scope of this document and depend on the specific medium, but often it will mark that packet as multicast at the link layer too, e.g. by giving it a special destination MAC address.  This ensures that the packet is delivered correctly by the link layer.\n\nIf you are simply trying to receive existing multicast packets, all you need to know is the group address that the multicasts are being sent on.  But if you\'re trying to build your own application that communicates via multicast, you\'ll need to select an IPv4 or IPv6 multicast address to use for it.  Many of these addresses have to be officially assigned by IANA (the `wikipedia page on multicast addresses <https://en.wikipedia.org/wiki/Multicast_address#IPv4>`_ has the full details), though IP addresses in the 239.x.x.x range are "administratively scoped" and available for private use on LANs.\n\nMulticast Routing in Networks\n=============================\nCompared to regular IP packets, multicast packets are handled differently by networking devices such as Ethernet switches and routers.  It\'s all too easy to forget to take this into account, and then find yourself asking "wait, why am I not receiving any multicast traffic", or even "wait, why am I receiving *all of the multicasts* that I didn\'t ask for?"  This section will go over some basics of how multicast packets move through Ethernet networks.  Other networks may differ in the specifics, but the basic concepts should be similar.\n\nFor a simple ("unmanaged") Ethernet switch, its handling of multicast packets is very simple.  It simply treats them like broadcasts, and forwards them to every other port of the switch.\n\nAs you might imagine, if you have a large network full of multicast users, and switches are broadcasting every message everywhere, you could get some pretty awful network congestion.  To combat this, more complex ("managed") Ethernet switches often have a feature called "IGMP snooping".  When a switch has this setting enabled, it listens for what\'s called an "IGMP join message" to be sent by a host.  This message is automatically sent by your OS whenever you open a multicast receive socket, and indicates that host X wants to receive traffic going to multicast address Y.  When the switch sees one of these messages, it automatically begins routing traffic going to multicast address Y into host X\'s network link.  No IGMP join message?  No multicasts for you.\n\nNote: for IPv6, MLD messages are used instead of IGMP, but they do pretty much the same thing.\n\nLast but not least, routers.  In contrast to Ethernet switches, which connect individual hosts together, routers connect entire networks together.  They have quite a bit more logic and generally require at least some manual configuration of what packets are routed where.  Often, multicasts are just used within the local network and are dropped by routers (you can guarantee this by setting the Time To Live to 1, forcing them to be dropped by any router).  However, the specifics depend on the router configuration, and often individual multicast addresses are treated differently.  If you really do need to pass multicasts through a router, you should contact your ISP or your network admin to verify the router settings.\n\nIn conclusion, here\'s a table of how different boxes handle multicasts:\n\n========================================= ============================================\nBox                                       What does it do with multicast packets?\n========================================= ============================================\nEthernet Switch (No IGMP Snooping)        Forwards to all hosts\nEthernet Switch (IGMP Snooping Enabled)   Forwards to any hosts that have subscribed\nRouter                                    Depends on configuration.\n========================================= ============================================\n\n**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I\'ve seen a number of devices that do not implement the standard as I\'ve written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which seemed to work fine initially but started dropping most multicast traffic when IGMP snooping was enabled!\n\nSince lots of devices come with weird multicast settings out of the box, prepare to have to check and fix the configuration on each switch/device when you start using multicast on your network.\n\nSending Multicasts\n===================\n\nTo send multicasts, an application can pretty much just create a normal UDP socket and have it send packets to a multicast IP address.  However, there is one additional piece needed, which is that the OS needs to be told which interface to send the multicasts on.  This is always done using the IP_MULTICAST_IF setsockopt() option, but the exact syntax and procedure for using this option differs by OS.  Luckily, Multicast Expert takes care of that for you!\n\nReceiving Multicasts\n====================\n\nTo receive multicasts, essentially two things need to happen.  First, your OS needs to be told to send out an IGMP join message, telling other devices on the network to send multicast packets your way.  This generally happens as a side effect of enabling the IP_ADD_MEMBERSHIP socket option (or one of its variants) on a socket.  Then, the OS network stack needs to be configured to forward multicast packets which arrive on the given interface to your application.  This process is pretty different on Windows and Unix.\n\nOn Windows, multicast sockets are bound to a given port and interface (using bind()) when they are initially created.  Then, IP_ADD_MEMBERSHIP commands are used to further associate them with individual multicast addresses, so that when a packet is received to that multicast addr, it goes to the correct socket.  This is convenient as it means one socket can use multiple multicast groups and still not receive unwanted traffic from other groups that use the same port.  However, there\'s no way to block unicast traffic going to that interface and port from also being received by the multicast socket.\n\nBut on Unix, the situation is a bit different.  The IP_ADD_MEMBERSHIP command does not directly set up filtering by multicast address, it pretty much just sends the IGMP join message and opens the interface to receive packets going to the multicast address.  It does not directly associate the socket with the multicast address, it\'s still a "regular" UDP socket.  So, if you were to take a multicast socket and bind it to 0.0.0.0, it would end up receiving all UDP traffic on the port number, even traffic to other multicast addresses or to the unicast address.  The only way to fix this is to bind the socket to the specific multicast address instead, causing any traffic with a different destination address to not be accepted by the socket.  Unfortunately, a socket can only be bound to one destination address at a time, so this means multicast expert needs to create a different socket under the hood for each multicast address you want to listen on.\n\n**********************\nUsing Multicast Expert\n**********************\n\nNow let\'s get into some actual code examples.  Now first, before we can create any sockets, we need to find the interface address we want to use (see above).  Luckily, Multicast Expert comes with a convenient function to list all available network interfaces:\n\n>>> import multicast_expert\n>>> multicast_expert.get_interface_ips(include_ipv4=True, include_ipv6=False)\n[\'192.168.0.248\', \'192.168.153.1\', \'127.0.0.1\']\n\n(note that this function is a wrapper around the netifaces library, which provides quite a bit more functionality if you need it)\n\nBut which of those is the interface we actually want to use?  Well, that depends on your specific nework setup, but to make an educated guess, we also have a function to get the interface your machine uses to contact the internet.  This is not always correct but will work for many network setups.\n\n>>> multicast_expert.get_default_gateway_iface_ip_v4()\n\'192.168.0.248\'\n\nTransmitting Multicasts\n=======================\n\nTo send some data to a multicast, use the McastTxSocket class.  This wraps a socket internally, and does all the hard work of configuring it correctly for multicast.  For now we will use \'239.1.2.3\' as our multicast address since it\'s in the administratively scoped block.\n\nThe following block shows how to create a Tx socket and send some data:\n\n>>> import socket\n>>> with multicast_expert.McastTxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], iface_ip=\'192.168.0.248\') as mcast_tx_sock:\n...     mcast_tx_sock.sendto(b\'Hello World\', (\'239.1.2.3\', 12345))\n\nNote: when you construct the socket, you have to pass in all of the multicast IPs that you will want to use the socket to send to.  These must be known in advance in order to configure socket options correctly.\n\nNote 2: If you omitted the iface_ip= argument, the get_default_gateway_iface_ip_v4() function would have been called to guess the iface ip.  So, we could have omitted this argument for the same result.\n\nReceiving Multicasts\n====================\n\nTo receive from one or more multicast addresses, use the McastRxSocket class.  For example:\n\n>>> with multicast_expert.McastRxSocket(socket.AF_INET, mcast_ips=[\'239.1.2.3\'], port=12345, iface_ip=\'192.168.0.248\') as mcast_rx_sock:\n...     bytes, src_address = mcast_rx_sock.recvfrom()\n\nThe above code will listen on the 239.1.2.3 multicast address, and will block until a packet is received.  To change the blocking behavior, use the settimeout() function.\n\nFull Example\n============\nFor a complete example of how to use this library, see the system test script `here <https://github.com/multiplemonomials/multicast_expert/blob/main/examples/mcast_communicator.py>`_.\n\nFAQ\n===\nQ: What happens if an interface changes IP address (e.g. due to the user modifying a static IP) after I create a multicast socket on that interface?\n    A: On all machines tested so far, multicast sockets will stick with their assigned interface once created, even if the IP of that interface changes or it is brought down.\n\nQ: Do McastRxSockets receive regular (unicast) UDP packets going to the same interface and port?\n    A: On Windows, yes.  On Unix, no.  Unfortunately, this is a platform difference that I haven\'t found an easy way to work around.\n\nQ: Can I create multiple McastRxSockets on the same port and interface?\n    A: As long as they have different mcast addresses, then yes, this works how you\'d expect.\n\nQ: Is it possible to receive multicasts on all interfaces with a single socket?\n    A: Yes!  As of multicast_expert 1.2.0, the default behavior of McastRxSocket, when you do not pass any interface IP addresses explicitly, is to listen on all non-loopback interfaces of the machine.\n\nQ: Why are my multicasts to the loopback device not going through in Linux?\n    A: Linux seems to be very picky about what it allows through loopback.  First of all, you need to use ``ip route`` to add a route directing your multicast address to the ``lo`` interface.  For example, the command ``sudo ip route add 239.2.2.0/24 dev lo`` would allow any multicasts in the 239.2.2.x range through loopback.\n\n    Additionally, for IPv6, I have found that multicasts to addresses that don\'t start with ``ffx1`` for any value of x (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...\n\nQ: My multicasts aren\'t being received in Linux, even though I see them coming in in packet dumps.\n    A: On Linux, you must also be careful of a kernel feature called Reverse Path Filtering (RPF).  You see, in most cases, multicast doesn\'t care about unicast IPs or subnets -- you can quite easily have a machine with IP 10.0.0.1 send multicasts to 192.168.1.2, even though those are on different subnets so they can\'t normally communicate.  However, RPF throws a wrench in this.  In its default "loose" mode (setting 2), it blocks reception of IP packets if they come from an IP address not reachable by any interface.  So, for example, if you receive a multicast from 10.0.0.1 but you only have routes in your routing table for 192.168.x.x IP addresses, the kernel will summarily drop the packet.  The easiest fix is to label one of your network interfaces as a default route.  This makes all IP addresses reachable from an interface, so all packets will be able to get by the check.\n\n    RPF\'s "strict" mode (setting 1) is even worse.  It applies the same check, but on a per-interface level.  So, in order to receive packets from multicast address X, each individual interface must have a routing rule permitting it to send packets to X.  If this is too much of a pain to set up, you can turn RPF off using sysctl (`this seems like a decent guide <https://access.redhat.com/solutions/53031#:~:text=rp_filter%20parameter%20only%20has%20two,default%20is%201%20(loose).>`_).  Just remember to change it both for the "all" interface and for whichever interfaces you want to affect -- the kernel takes the stricter of the two values.\n\n    If RPF isn\'t the problem, you may also want to check any firewalls (firewalld/iptables) and see if those are blocking multicast packets.\n\nQ: If I have a socket that receives from multiple mcast addresses, say A and B, and I receive a packet, how do I tell whether the packet was sent to multicast address A or B?\n    A: You can\'t, or at least I haven\'t found a way to do this from Python.  You\'ll need to create multiple sockets if you need this information.',
     'author': 'Jamie Smith',
     'author_email': 'jsmith@crackofdawn.onmicrosoft.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/multiplemonomials/multicast_expert',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `multicast_expert-1.1.2/PKG-INFO` & `multicast_expert-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicast-expert
-Version: 1.1.2
+Version: 1.2.0
 Summary: A library to take the fiddly parts out of multicast networking!
 Home-page: https://github.com/multiplemonomials/multicast_expert
 License: MIT
 Author: Jamie Smith
 Author-email: jsmith@crackofdawn.onmicrosoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,17 @@
 
 *******************
 Multicasting Basics
 *******************
 
 Before I can explain how to use this library, I first need to explain the basics of multicasting itself.  There's not a lot of info out there on the net about how to do multicasting right, and much of what there is is buried deep in OS documentation.  So let's go over some of the basic concepts first.
 
-First and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Multicasting happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to one specific network interface that it will use.  There is no such thing as "bind to 0.0.0.0" or "listen on all addresses"!
+First and foremost, there is one principle that I need to make clear, or you will not have a good time trying to use multicast.  **Sending multicasts happens at the network interface level, not the machine level**.  Almost every machine has at least two network interfaces: the loopback interface to itself and the Ethernet/WiFi connection it uses to access the the Internet.  Many machines also have additional interfaces such as bridges to Docker containers/virtual machines, VPNs, or additional private LANs.  With normal (unicast) networking, you simply tell the OS what IP address you want to send a packet to, and it will select the appropriate interface automatically (using a structure called the routing table).  This is not so with multicast!  Every multicast socket needs to be bound to a specific network interface that it will use.  At the OS level, there is no such thing as "bind to 0.0.0.0" or "listen on all interface"!
+
+However, multicast_expert does allow an "multi-interface" mode which combines together multiple OS sockets to allow listening for incoming multicasts on several or all network interfaces.  This allows "bind to 0.0.0.0"-like behavior for Rx sockets only!
 
 Now that we've gotten that out of the way, we can cover the four essential topics for multicast: multicast addresses, understanding network routing, creating a transmitter, and creating a receiver.
 
 Multicast Addresses
 ===================
 A multicast IPv4 address is defined as any IPv4 address whose most significant four bits are "1110".  This means any IP address whose first number is in the range of 224 through 239 (0xE0-0xEF) is a multicast address.  Similarly, for IPv6, any address whose first byte is 0xFF is a multicast address.
 
@@ -65,15 +67,15 @@
 Box                                       What does it do with multicast packets?
 ========================================= ============================================
 Ethernet Switch (No IGMP Snooping)        Forwards to all hosts
 Ethernet Switch (IGMP Snooping Enabled)   Forwards to any hosts that have subscribed
 Router                                    Depends on configuration.
 ========================================= ============================================
 
-**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I've seen a number of devices that do not implement the standard as I've written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which worked fine out of the box but started dropping most multicast traffic when IGMP snooping was enabled!
+**NOTE:** Be careful of boxes with unexpected behavior!  Multicast is one of the more rarely used features of IP and often does not seem to be well tested.  In my time working with multicast, I've seen a number of devices that do not implement the standard as I've written it here.  For instance, some switches can individually have IGMP snooping enabled/disabled on each port, producing unexpected behavior.  I think the worst was a desktop switch which seemed to work fine initially but started dropping most multicast traffic when IGMP snooping was enabled!
 
 Since lots of devices come with weird multicast settings out of the box, prepare to have to check and fix the configuration on each switch/device when you start using multicast on your network.
 
 Sending Multicasts
 ===================
 
 To send multicasts, an application can pretty much just create a normal UDP socket and have it send packets to a multicast IP address.  However, there is one additional piece needed, which is that the OS needs to be told which interface to send the multicasts on.  This is always done using the IP_MULTICAST_IF setsockopt() option, but the exact syntax and procedure for using this option differs by OS.  Luckily, Multicast Expert takes care of that for you!
@@ -141,20 +143,20 @@
 Q: Do McastRxSockets receive regular (unicast) UDP packets going to the same interface and port?
     A: On Windows, yes.  On Unix, no.  Unfortunately, this is a platform difference that I haven't found an easy way to work around.
 
 Q: Can I create multiple McastRxSockets on the same port and interface?
     A: As long as they have different mcast addresses, then yes, this works how you'd expect.
 
 Q: Is it possible to receive multicasts on all interfaces with a single socket?
-    A: For reception, this should be possible; it may be implemented in a future version of the library.
+    A: Yes!  As of multicast_expert 1.2.0, the default behavior of McastRxSocket, when you do not pass any interface IP addresses explicitly, is to listen on all non-loopback interfaces of the machine.
 
 Q: Why are my multicasts to the loopback device not going through in Linux?
     A: Linux seems to be very picky about what it allows through loopback.  First of all, you need to use ``ip route`` to add a route directing your multicast address to the ``lo`` interface.  For example, the command ``sudo ip route add 239.2.2.0/24 dev lo`` would allow any multicasts in the 239.2.2.x range through loopback.
 
-    Additionally, for IPv6, I have found that multicasts to addresses that don't start with ``ffx1`` (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...
+    Additionally, for IPv6, I have found that multicasts to addresses that don't start with ``ffx1`` for any value of x (i.e. non-interface-local addresses) do not seem to be sent on loopback.  Still trying to find any document explaining this behavior...
 
 Q: My multicasts aren't being received in Linux, even though I see them coming in in packet dumps.
     A: On Linux, you must also be careful of a kernel feature called Reverse Path Filtering (RPF).  You see, in most cases, multicast doesn't care about unicast IPs or subnets -- you can quite easily have a machine with IP 10.0.0.1 send multicasts to 192.168.1.2, even though those are on different subnets so they can't normally communicate.  However, RPF throws a wrench in this.  In its default "loose" mode (setting 2), it blocks reception of IP packets if they come from an IP address not reachable by any interface.  So, for example, if you receive a multicast from 10.0.0.1 but you only have routes in your routing table for 192.168.x.x IP addresses, the kernel will summarily drop the packet.  The easiest fix is to label one of your network interfaces as a default route.  This makes all IP addresses reachable from an interface, so all packets will be able to get by the check.
 
     RPF's "strict" mode (setting 1) is even worse.  It applies the same check, but on a per-interface level.  So, in order to receive packets from multicast address X, each individual interface must have a routing rule permitting it to send packets to X.  If this is too much of a pain to set up, you can turn RPF off using sysctl (`this seems like a decent guide <https://access.redhat.com/solutions/53031#:~:text=rp_filter%20parameter%20only%20has%20two,default%20is%201%20(loose).>`_).  Just remember to change it both for the "all" interface and for whichever interfaces you want to affect -- the kernel takes the stricter of the two values.
 
     If RPF isn't the problem, you may also want to check any firewalls (firewalld/iptables) and see if those are blocking multicast packets.
```

