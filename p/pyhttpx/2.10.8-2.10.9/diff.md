# Comparing `tmp/pyhttpx-2.10.8.tar.gz` & `tmp/pyhttpx-2.10.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.8.tar", last modified: Fri Jun 23 04:51:59 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.9.tar", last modified: Fri Jun 30 09:48:40 2023, max compression
```

## Comparing `pyhttpx-2.10.8.tar` & `pyhttpx-2.10.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.8/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.8/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/PKG-INFO
--rw-rw-rw-   0        0        0     2592 2023-05-31 14:45:44.000000 pyhttpx-2.10.8/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.8/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.8/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     8043 2023-06-03 00:48:29.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10286 2023-06-01 09:25:13.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19331 2023-06-03 00:48:29.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4404 2023-06-01 09:51:28.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.8/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9501 2023-06-22 11:47:40.000000 pyhttpx-2.10.8/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16893 2023-06-23 04:51:56.000000 pyhttpx-2.10.8/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.8/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.8/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.8/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-06-23 04:51:56.000000 pyhttpx-2.10.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 04:51:59.000000 pyhttpx-2.10.8/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1735 2023-06-23 00:57:09.000000 pyhttpx-2.10.8/tests/requestTest.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.8/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.9/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2592 2023-05-31 14:45:44.000000 pyhttpx-2.10.9/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.9/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.9/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8043 2023-06-03 00:48:29.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10286 2023-06-01 09:25:13.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19354 2023-06-30 07:32:53.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2390 2023-06-30 02:23:54.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4404 2023-06-01 09:51:28.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.9/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9494 2023-06-30 02:02:38.000000 pyhttpx-2.10.9/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16893 2023-06-23 04:51:56.000000 pyhttpx-2.10.9/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.9/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.9/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.9/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-30 09:48:39.000000 pyhttpx-2.10.9/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-06-30 09:48:36.000000 pyhttpx-2.10.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:48:40.000000 pyhttpx-2.10.9/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1735 2023-06-30 09:48:36.000000 pyhttpx-2.10.9/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.9/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.8/LICENSE` & `pyhttpx-2.10.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/README.md` & `pyhttpx-2.10.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/exception.py` & `pyhttpx-2.10.9/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/keyexchange.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/pyaiossl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/pyssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
 
     def mutable_recv(self, size=1024):
         try:
             self.sock.settimeout(self.timeout)
             s = self.sock.recv(size)
             return s
 
-        except socket.timeout:
+        except (socket.timeout,ConnectionResetError):
             raise ReadTimeout('read timeout %s:%s' % (self.host, self.port))
 
     def recv(self):
 
         while True:
             s = self.process()
             if s is None:
```

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/socks.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,17 @@
             http_headers.append(b"Proxy-Authorization: Basic "
                                  + b64encode(username.encode('latin1') + b":" + password.encode('latin1')))
 
         http_headers.append(b"\r\n")
         try:
             super(SocketProxy, self).connect((proxy_addr, proxy_port))
             self.sendall(b"\r\n".join(http_headers))
-            status_line = self.recv(4096).decode()
+
+            line = self.recv(4096)
+            status_line = line.decode('latin1')
             proto, status_code, status_msg = status_line.split(" ", 2)
         except (socket.timeout, ConnectionRefusedError,UnicodeDecodeError):
             raise ProxyError(
                 "Proxy server connection time out")
 
         if not proto.startswith("HTTP/"):
             raise ProxyError(
```

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/suites.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.9/pyhttpx/layers/tls/tls_context.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/models.py` & `pyhttpx-2.10.9/pyhttpx/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
             if 'chunked'  == self.headers.get('transfer-encoding'):
                 #chunked
                 #if self.plaintext_buffer.endswith(b'\r\n0\r\n'):
                 #if self.plaintext_buffer.endswith(b'\r\n0\r\n'):
                 tmp = self.plaintext_buffer.split(b'\r\n')
                 if b'0' in tmp:
-                    
-                    self.body = b'\r\n'.join(tmp[:-2])
+
+                    self.body = b'\r\n'.join(tmp[:tmp.index(b'0')])
                     self.read_ended = True
 
             else:
 
                 if self.content_length:
                     if self.content_length <= len(self.plaintext_buffer):
                         self.body = self.plaintext_buffer[:self.content_length]
```

### Comparing `pyhttpx-2.10.8/pyhttpx/session.py` & `pyhttpx-2.10.9/pyhttpx/session.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/utils.py` & `pyhttpx-2.10.9/pyhttpx/utils.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx/websocket.py` & `pyhttpx-2.10.9/pyhttpx/websocket.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.9/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/setup.py` & `pyhttpx-2.10.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.8",
+    version = "2.10.9",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.8/tests/requestTest.py` & `pyhttpx-2.10.9/tests/requestTest.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.8/tests/websocketTest.py` & `pyhttpx-2.10.9/tests/websocketTest.py`

 * *Files identical despite different names*

