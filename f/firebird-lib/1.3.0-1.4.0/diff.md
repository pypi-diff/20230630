# Comparing `tmp/firebird-lib-1.3.0.tar.gz` & `tmp/firebird-lib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebird-lib-1.3.0.tar", last modified: Fri Mar  3 13:14:55 2023, max compression
+gzip compressed data, was "firebird-lib-1.4.0.tar", last modified: Fri Jun 30 11:16:17 2023, max compression
```

## Comparing `firebird-lib-1.3.0.tar` & `firebird-lib-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.432348 firebird-lib-1.3.0/
--rw-r--r--   0 pcisar    (1000) users      (100)     1068 2020-04-30 09:23:34.000000 firebird-lib-1.3.0/LICENSE
--rw-r--r--   0 pcisar    (1000) users      (100)     3078 2023-03-03 13:14:55.432348 firebird-lib-1.3.0/PKG-INFO
--rw-r--r--   0 pcisar    (1000) users      (100)      604 2020-10-12 15:07:38.000000 firebird-lib-1.3.0/README.rst
--rw-r--r--   0 pcisar    (1000) users      (100)     1403 2023-03-03 13:11:45.000000 firebird-lib-1.3.0/pyproject.toml
--rw-r--r--   0 pcisar    (1000) users      (100)       38 2023-03-03 13:14:55.432348 firebird-lib-1.3.0/setup.cfg
--rw-r--r--   0 pcisar    (1000) users      (100)      260 2021-02-09 17:41:50.000000 firebird-lib-1.3.0/setup.py
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.424348 firebird-lib-1.3.0/src/
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.424348 firebird-lib-1.3.0/src/firebird/
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.428348 firebird-lib-1.3.0/src/firebird/lib/
--rw-r--r--   0 pcisar    (1000) users      (100)        0 2022-11-06 10:06:19.000000 firebird-lib-1.3.0/src/firebird/lib/__init__.py
--rw-r--r--   0 pcisar    (1000) users      (100)    28254 2022-10-12 16:01:58.000000 firebird-lib-1.3.0/src/firebird/lib/gstat.py
--rw-r--r--   0 pcisar    (1000) users      (100)     5428 2022-11-06 10:23:43.000000 firebird-lib-1.3.0/src/firebird/lib/log.py
--rw-r--r--   0 pcisar    (1000) users      (100)    73053 2022-10-12 16:38:44.000000 firebird-lib-1.3.0/src/firebird/lib/logmsgs.py
--rw-r--r--   0 pcisar    (1000) users      (100)    41658 2022-11-06 10:24:11.000000 firebird-lib-1.3.0/src/firebird/lib/monitor.py
--rw-r--r--   0 pcisar    (1000) users      (100)   211009 2022-10-14 13:02:37.000000 firebird-lib-1.3.0/src/firebird/lib/schema.py
--rw-r--r--   0 pcisar    (1000) users      (100)    70960 2022-10-12 17:09:46.000000 firebird-lib-1.3.0/src/firebird/lib/trace.py
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.428348 firebird-lib-1.3.0/src/firebird_lib.egg-info/
--rw-r--r--   0 pcisar    (1000) users      (100)     3078 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/PKG-INFO
--rw-r--r--   0 pcisar    (1000) users      (100)      560 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/SOURCES.txt
--rw-r--r--   0 pcisar    (1000) users      (100)        1 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/dependency_links.txt
--rw-r--r--   0 pcisar    (1000) users      (100)       44 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/requires.txt
--rw-r--r--   0 pcisar    (1000) users      (100)        9 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/top_level.txt
--rw-r--r--   0 pcisar    (1000) users      (100)        1 2023-03-03 13:14:54.000000 firebird-lib-1.3.0/src/firebird_lib.egg-info/zip-safe
-drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-03-03 13:14:55.428348 firebird-lib-1.3.0/test/
--rw-r--r--   0 pcisar    (1000) users      (100)   243259 2022-10-03 14:01:59.000000 firebird-lib-1.3.0/test/test_gstat.py
--rw-r--r--   0 pcisar    (1000) users      (100)    21336 2022-10-03 14:02:10.000000 firebird-lib-1.3.0/test/test_log.py
--rw-r--r--   0 pcisar    (1000) users      (100)    25207 2022-10-14 09:30:45.000000 firebird-lib-1.3.0/test/test_monitor.py
--rw-r--r--   0 pcisar    (1000) users      (100)   216005 2022-10-14 12:44:56.000000 firebird-lib-1.3.0/test/test_schema.py
--rw-r--r--   0 pcisar    (1000) users      (100)   152488 2022-10-03 14:03:43.000000 firebird-lib-1.3.0/test/test_trace.py
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.672497 firebird-lib-1.4.0/
+-rw-r--r--   0 pcisar    (1000) users      (100)     1068 2020-04-30 09:23:34.000000 firebird-lib-1.4.0/LICENSE
+-rw-r--r--   0 pcisar    (1000) users      (100)     3078 2023-06-30 11:16:17.672497 firebird-lib-1.4.0/PKG-INFO
+-rw-r--r--   0 pcisar    (1000) users      (100)      604 2020-10-12 15:07:38.000000 firebird-lib-1.4.0/README.rst
+-rw-r--r--   0 pcisar    (1000) users      (100)     1403 2023-06-29 14:41:58.000000 firebird-lib-1.4.0/pyproject.toml
+-rw-r--r--   0 pcisar    (1000) users      (100)       38 2023-06-30 11:16:17.672497 firebird-lib-1.4.0/setup.cfg
+-rw-r--r--   0 pcisar    (1000) users      (100)      260 2021-02-09 17:41:50.000000 firebird-lib-1.4.0/setup.py
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.668497 firebird-lib-1.4.0/src/
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.668497 firebird-lib-1.4.0/src/firebird/
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.668497 firebird-lib-1.4.0/src/firebird/lib/
+-rw-r--r--   0 pcisar    (1000) users      (100)        0 2022-11-06 10:06:19.000000 firebird-lib-1.4.0/src/firebird/lib/__init__.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    28254 2022-10-12 16:01:58.000000 firebird-lib-1.4.0/src/firebird/lib/gstat.py
+-rw-r--r--   0 pcisar    (1000) users      (100)     5428 2022-11-06 10:23:43.000000 firebird-lib-1.4.0/src/firebird/lib/log.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    73053 2022-10-12 16:38:44.000000 firebird-lib-1.4.0/src/firebird/lib/logmsgs.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    48803 2023-06-30 10:08:48.000000 firebird-lib-1.4.0/src/firebird/lib/monitor.py
+-rw-r--r--   0 pcisar    (1000) users      (100)   212194 2023-06-30 10:36:36.000000 firebird-lib-1.4.0/src/firebird/lib/schema.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    70960 2022-10-12 17:09:46.000000 firebird-lib-1.4.0/src/firebird/lib/trace.py
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.668497 firebird-lib-1.4.0/src/firebird_lib.egg-info/
+-rw-r--r--   0 pcisar    (1000) users      (100)     3078 2023-06-30 11:16:17.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/PKG-INFO
+-rw-r--r--   0 pcisar    (1000) users      (100)      560 2023-06-30 11:16:17.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 pcisar    (1000) users      (100)        1 2023-06-30 11:16:17.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 pcisar    (1000) users      (100)       44 2023-06-30 11:16:17.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/requires.txt
+-rw-r--r--   0 pcisar    (1000) users      (100)        9 2023-06-30 11:16:17.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/top_level.txt
+-rw-r--r--   0 pcisar    (1000) users      (100)        1 2023-03-03 13:14:54.000000 firebird-lib-1.4.0/src/firebird_lib.egg-info/zip-safe
+drwxr-xr-x   0 pcisar    (1000) users      (100)        0 2023-06-30 11:16:17.672497 firebird-lib-1.4.0/test/
+-rw-r--r--   0 pcisar    (1000) users      (100)   243259 2022-10-03 14:01:59.000000 firebird-lib-1.4.0/test/test_gstat.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    21336 2022-10-03 14:02:10.000000 firebird-lib-1.4.0/test/test_log.py
+-rw-r--r--   0 pcisar    (1000) users      (100)    28735 2023-06-30 09:25:06.000000 firebird-lib-1.4.0/test/test_monitor.py
+-rw-r--r--   0 pcisar    (1000) users      (100)   220248 2023-06-30 10:33:05.000000 firebird-lib-1.4.0/test/test_schema.py
+-rw-r--r--   0 pcisar    (1000) users      (100)   152488 2022-10-03 14:03:43.000000 firebird-lib-1.4.0/test/test_trace.py
```

### Comparing `firebird-lib-1.3.0/LICENSE` & `firebird-lib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/PKG-INFO` & `firebird-lib-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebird-lib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Firebird driver extension library
 Author-email: Pavel Cisar <pcisar@users.sourceforge.net>
 License: MIT License
         
         Copyright (c) 2020 FirebirdSQL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `firebird-lib-1.3.0/README.rst` & `firebird-lib-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/pyproject.toml` & `firebird-lib-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "firebird-lib"
-version = "1.3.0"
+version = "1.4.0"
 description = "Firebird driver extension library"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [{ name = "Pavel Cisar", email = "pcisar@users.sourceforge.net"}]
 keywords = ["Firebird", "RDBMS", "driver", "extension", "library"]
 classifiers = [
@@ -23,16 +23,16 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Topic :: Software Development",
     "Topic :: Database",
     ]
 dependencies = [
-    "firebird-base>=1.5.0",
-    "firebird-driver>=1.7.0",
+    "firebird-base>=1.6.1",
+    "firebird-driver>=1.9.0",
     ]
 
 [project.urls]
 Home = "https://github.com/FirebirdSQL/python3-lib"
 Documentation = "https://firebird-lib.rtfd.io"
 "Bug Reports" = "https://github.com/FirebirdSQL/python3-lib/issues"
 Funding = "https://www.firebirdsql.org/en/donate/"
```

### Comparing `firebird-lib-1.3.0/src/firebird/lib/gstat.py` & `firebird-lib-1.4.0/src/firebird/lib/gstat.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/src/firebird/lib/log.py` & `firebird-lib-1.4.0/src/firebird/lib/log.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/src/firebird/lib/logmsgs.py` & `firebird-lib-1.4.0/src/firebird/lib/logmsgs.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/src/firebird/lib/monitor.py` & `firebird-lib-1.4.0/src/firebird/lib/monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,31 +37,25 @@
 
 """
 
 from __future__ import annotations
 from typing import Dict, List, Any, Union
 import datetime
 import weakref
+from uuid import UUID
 from enum import Enum, IntEnum
 from firebird.base.collections import DataList
-from firebird.driver import tpb, Connection, Cursor, Statement, Isolation, Error, TraAccessMode
-from .schema import ObjectType, CharacterSet, Procedure, Trigger, Function
+from firebird.driver import (tpb, Connection, Cursor, Statement, Isolation, Error,
+                             TraAccessMode, ReplicaMode, ShutdownMode)
+from .schema import ObjectType, CharacterSet, Procedure, Trigger, Function, ObjectType
 
 FLAG_NOT_SET = 0
 FLAG_SET = 1
 
 # Enums
-class ShutdownMode(IntEnum):
-    """Shutdown mode.
-    """
-    ONLINE = 0
-    MULTI = 1
-    SINGLE = 2
-    FULL = 3
-
 class BackupState(IntEnum):
     """Physical backup state.
     """
     NORMAL = 0
     STALLED = 1
     MERGE = 2
 
@@ -69,19 +63,22 @@
     """Object state.
     """
     IDLE = 0
     ACTIVE = 1
 
 class IsolationMode(IntEnum):
     """Transaction solation mode.
+
+    .. versionchanged:: 1.4.0 - `READ_COMMITTED_READ_CONSISTENCY` value added
     """
     CONSISTENCY = 0
     CONCURRENCY = 1
     READ_COMMITTED_RV = 2
     READ_COMMITTED_NO_RV = 3
+    READ_COMMITTED_READ_CONSISTENCY = 4
 
 class Group(IntEnum):
     """Statistics group.
     """
     DATABASE = 0
     ATTACHMENT = 1
     TRANSACTION = 2
@@ -91,14 +88,25 @@
 class Security(Enum):
     """Security database.
     """
     DEFAULT = 'Default'
     SELF = 'Self'
     OTHER = 'Other'
 
+class CryptState(IntEnum):
+    """Database encryption state.
+
+    .. versionadded:: 1.4.0
+    """
+    NOT_ENCRYPTED = 0
+    ENCRYPTED = 1
+    DECRYPTION_IN_PROGRESS = 2
+    ENCRYPTION_IN_PROGRESS = 3
+
+
 # Classes
 class Monitor:
     """Class for access to Firebird monitoring tables.
     """
     def __init__(self, connection: Connection):
         """
         Arguments:
@@ -115,14 +123,15 @@
         self.__attachments = None
         self.__transactions = None
         self.__statements = None
         self.__callstack = None
         self.__iostats = None
         self.__variables = None
         self.__tablestats = None
+        self.__compiled_statements = None
     def __del__(self):
         if not self.closed:
             self.close()
     def __enter__(self) -> Monitor:
         return self
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self.close()
@@ -220,21 +229,22 @@
                                         CallStackInfo, 'item.id', frozen=True)
         return self.__callstack
     @property
     def iostats(self) -> DataList[IOStatsInfo]:
         """List of all I/O statistics.
         """
         if self.__iostats is None:
-            cmd = """SELECT r.MON$STAT_ID, r.MON$STAT_GROUP,
+            ext = '' if self.db.ods < 13.0 else  ', r.MON$RECORD_IMGC'
+            cmd = f"""SELECT r.MON$STAT_ID, r.MON$STAT_GROUP,
 r.MON$RECORD_SEQ_READS, r.MON$RECORD_IDX_READS, r.MON$RECORD_INSERTS,
 r.MON$RECORD_UPDATES, r.MON$RECORD_DELETES, r.MON$RECORD_BACKOUTS,
 r.MON$RECORD_PURGES, r.MON$RECORD_EXPUNGES, r.MON$RECORD_LOCKS, r.MON$RECORD_WAITS,
 r.MON$RECORD_CONFLICTS, r.MON$BACKVERSION_READS, r.MON$FRAGMENT_READS, r.MON$RECORD_RPT_READS,
 io.MON$PAGE_FETCHES, io.MON$PAGE_MARKS, io.MON$PAGE_READS, io.MON$PAGE_WRITES,
-m.MON$MEMORY_ALLOCATED, m.MON$MEMORY_USED, m.MON$MAX_MEMORY_ALLOCATED, m.MON$MAX_MEMORY_USED
+m.MON$MEMORY_ALLOCATED, m.MON$MEMORY_USED, m.MON$MAX_MEMORY_ALLOCATED, m.MON$MAX_MEMORY_USED{ext}
 FROM MON$RECORD_STATS r join MON$IO_STATS io
   on r.MON$STAT_ID = io.MON$STAT_ID and r.MON$STAT_GROUP = io.MON$STAT_GROUP
   join MON$MEMORY_USAGE m
   on r.MON$STAT_ID = m.MON$STAT_ID and r.MON$STAT_GROUP = m.MON$STAT_GROUP"""
             self.__iostats = DataList((IOStatsInfo(self, row) for row
                                        in self._select(cmd)),
                                       IOStatsInfo, 'item.stat_id', frozen=True)
@@ -249,25 +259,37 @@
                                         ContextVariableInfo, 'item.stat_id', frozen=True)
         return self.__variables
     @property
     def tablestats(self) -> DataList[TableStatsInfo]:
         """List of all table record I/O statistics.
         """
         if self.__tablestats is None:
-            cmd = """SELECT ts.MON$STAT_ID, ts.MON$STAT_GROUP, ts.MON$TABLE_NAME,
+            ext = '' if self.db.ods < 13.0 else  ', r.MON$RECORD_IMGC'
+            cmd = f"""SELECT ts.MON$STAT_ID, ts.MON$STAT_GROUP, ts.MON$TABLE_NAME,
 ts.MON$RECORD_STAT_ID, r.MON$RECORD_SEQ_READS, r.MON$RECORD_IDX_READS, r.MON$RECORD_INSERTS,
 r.MON$RECORD_UPDATES, r.MON$RECORD_DELETES, r.MON$RECORD_BACKOUTS,
 r.MON$RECORD_PURGES, r.MON$RECORD_EXPUNGES, r.MON$RECORD_LOCKS, r.MON$RECORD_WAITS,
-r.MON$RECORD_CONFLICTS, r.MON$BACKVERSION_READS, r.MON$FRAGMENT_READS, r.MON$RECORD_RPT_READS
+r.MON$RECORD_CONFLICTS, r.MON$BACKVERSION_READS, r.MON$FRAGMENT_READS, r.MON$RECORD_RPT_READS{ext}
 FROM MON$TABLE_STATS ts join MON$RECORD_STATS r
   on ts.MON$RECORD_STAT_ID = r.MON$STAT_ID"""
             self.__tablestats = DataList((TableStatsInfo(self, row) for row
                                           in self._select(cmd)),
                                          TableStatsInfo, 'item.stat_id', frozen=True)
         return self.__tablestats
+    @property
+    def compiled_statements(self) -> DataList[CompiledStatementInfo]:
+        """List of all compiled statements.
+
+        .. versionadded:: 1.4.0
+        """
+        if self.__compiled_statements is None:
+            self.__compiled_statements = DataList((CompiledStatementInfo(self, row) for row
+                                                   in self._select('select * from mon$compiled_statements')),
+                                                  CompiledStatementInfo, 'item.id', frozen=True)
+        return self.__compiled_statements
 
 class InfoItem:
     """Base class for all database monitoring objects.
     """
     def __init__(self, monitor: Monitor, attributes: Dict[str, Any]):
         #: Weak reference to parent `.Monitor` instance.
         self.monitor: Monitor = monitor if isinstance(monitor, weakref.ProxyType) else weakref.proxy(monitor)
@@ -399,14 +421,60 @@
         return Security(self._attributes.get('MON$SEC_DATABASE'))
     @property
     def tablestats(self) -> Dict[str, TableStatsInfo]:
         """Dictionary of `.TableStatsInfo` instances for this object.
         """
         return {io.table_name: io for io in self.monitor.tablestats
                 if (io.stat_id == self.stat_id) and (io.group is Group.DATABASE)}
+    # Firebird 4
+    @property
+    def crypt_state(self) -> Optional[CryptState]:
+        """Current state of database encryption.
+
+        .. versionadded:: 1.4.0
+        """
+        value = self._attributes.get('MON$CRYPT_STATE')
+        return None if value is None else CryptState(value)
+    @property
+    def guid(self) -> Optional[UUID]:
+        """Database GUID (persistent until restore / fixup).
+
+        .. versionadded:: 1.4.0
+        """
+        value = self._attributes.get('MON$GUID')
+        return None if value is None else UUID(value)
+    @property
+    def file_id(self) -> Optional[str]:
+        """Unique ID of the database file at the filesystem level.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$FILE_ID')
+    @property
+    def next_attachment(self) -> Optional[int]:
+        """Current value of the next attachment ID counter.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$NEXT_ATTACHMENT')
+    @property
+    def next_statement(self) -> Optional[int]:
+        """Current value of the next statement ID counter.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$NEXT_STATEMENT')
+    @property
+    def replica_mode(self) -> Optional[ReplicaMode]:
+        """Database replica mode.
+
+        .. versionadded:: 1.4.0
+        """
+        value = self._attributes.get('MON$REPLICA_MODE')
+        return None if value is None else ReplicaMode(value)
 
 class AttachmentInfo(InfoItem):
     """Information about attachment (connection) to database.
     """
     def __init__(self, monitor: Monitor, attributes: Dict[str, Any]):
         super().__init__(monitor, attributes)
         self._strip_attribute('MON$ATTACHMENT_NAME')
@@ -468,35 +536,35 @@
         return self._attributes['MON$ATTACHMENT_NAME']
     @property
     def user(self) -> str:
         """User name.
         """
         return self._attributes['MON$USER']
     @property
-    def role(self) -> str:
+    def role(self) -> Optional[str]:
         """Role name.
         """
         return self._attributes['MON$ROLE']
     @property
-    def remote_protocol(self) -> str:
+    def remote_protocol(self) -> Optional[str]:
         """Remote protocol name.
         """
         return self._attributes['MON$REMOTE_PROTOCOL']
     @property
-    def remote_address(self) -> str:
+    def remote_address(self) -> Optional[str]:
         """Remote address.
         """
         return self._attributes['MON$REMOTE_ADDRESS']
     @property
-    def remote_pid(self) -> int:
+    def remote_pid(self) -> Optional[int]:
         """Remote client process ID.
         """
         return self._attributes['MON$REMOTE_PID']
     @property
-    def remote_process(self) -> str:
+    def remote_process(self) -> Optional[str]:
         """Remote client process pathname.
         """
         return self._attributes['MON$REMOTE_PROCESS']
     @property
     def character_set(self) -> CharacterSet:
         """Character set name for this attachment.
         """
@@ -562,14 +630,65 @@
         return bool(self._attributes.get('MON$SYSTEM_FLAG'))
     @property
     def tablestats(self) -> Dict[str, TableStatsInfo]:
         """Dictionary of `.TableStatsInfo` instances for this object.
         """
         return {io.table_name: io for io in self.monitor.tablestats
                 if (io.stat_id == self.stat_id) and (io.group is Group.ATTACHMENT)}
+    # Firebird 4
+    @property
+    def idle_timeout(self) -> Optional[int]:
+        """Connection level idle timeout.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$IDLE_TIMEOUT')
+    @property
+    def idle_timer(self) -> Optional[datetime]:
+        """Idle timer expiration time.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$IDLE_TIMER')
+    @property
+    def statement_timeout(self) -> Optional[int]:
+        """Connection level statement timeout.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$STATEMENT_TIMEOUT')
+    @property
+    def wire_compressed(self) -> Optional[bool]:
+        """Wire compression.
+
+        .. versionadded:: 1.4.0
+        """
+        return bool(self._attributes.get('MON$WIRE_COMPRESSED'))
+    @property
+    def wire_encrypted(self) -> Optional[bool]:
+        """Wire encryption.
+
+        .. versionadded:: 1.4.0
+        """
+        return bool(self._attributes.get('MON$WIRE_ENCRYPTED'))
+    @property
+    def wire_crypt_plugin(self) -> Optional[str]:
+        """Name of the wire encryption plugin used by client.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$WIRE_CRYPT_PLUGIN')
+    # Firebird 5
+    @property
+    def session_timezone(self) -> Optional[str]:
+        """Actual timezone of the session.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$SESSION_TIMEZONE')
 
 class TransactionInfo(InfoItem):
     """Information about transaction.
     """
     def is_active(self) -> bool:
         """Returns True if transaction is active.
         """
@@ -743,14 +862,37 @@
                                          and (io.group is Group.STATEMENT))
     @property
     def tablestats(self) -> Dict[str, TableStatsInfo]:
         """Dictionary of `.TableStatsInfo` instances for this object.
         """
         return {io.table_name: io for io in self.monitor.tablestats
                 if (io.stat_id == self.stat_id) and (io.group is Group.STATEMENT)}
+    # Firebird 4
+    @property
+    def timeout(self) -> Optional[int]:
+        """Connection level statement timeout.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$STATEMENT_TIMEOUT')
+    @property
+    def timer(self) -> Optional[datetime]:
+        """Statement timer expiration time.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$STATEMENT_TIMER')
+    # Firebird 5
+    @property
+    def compiled_statement(self) -> Optional[CompiledStatementInfo]:
+        """`.CompiledStatementInfo` instance to which this statement relates.
+
+        .. versionadded:: 1.4.0
+        """
+        return self.monitor.compiled_statements.get(self._attributes['MON$COMPILED_STATEMENT_ID'])
 
 class CallStackInfo(InfoItem):
     """Information about PSQL call (stack frame).
     """
     def __init__(self, monitor: Monitor, attributes: Dict[str, Any]):
         super().__init__(monitor, attributes)
         self._strip_attribute('MON$OBJECT_NAME')
@@ -815,14 +957,22 @@
                else self.monitor._con.schema.packages.get(name)
     @property
     def iostats(self) -> IOStatsInfo:
         """`.IOStatsInfo` for this object.
         """
         return self.monitor.iostats.find(lambda io: (io.stat_id == self.stat_id)
                                          and (io.group is Group.CALL))
+    # Firebird 5
+    @property
+    def compiled_statement(self) -> Optional[CompiledStatementInfo]:
+        """`.CompiledStatementInfo` instance to which this statement relates.
+
+        .. versionadded:: 1.4.0
+        """
+        return self.monitor.compiled_statements.get(self._attributes['MON$COMPILED_STATEMENT_ID'])
 
 class IOStatsInfo(InfoItem):
     """Information about page and row level I/O operations, and about memory consumption.
     """
     @property
     def owner(self) -> Union[DatabaseInfo, AttachmentInfo, TransactionInfo,
                              StatementInfo, CallStackInfo]:
@@ -954,14 +1104,23 @@
         """
         return self._attributes.get('MON$FRAGMENT_READS')
     @property
     def repeated_reads(self) -> int:
         """Number of repeated record reads.
         """
         return self._attributes.get('MON$RECORD_RPT_READS')
+    # Firebird 4
+    @property
+    def intermediate_gc(self) -> Optional[int]:
+        """Number of records processed by the intermediate garbage collection.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes.get('MON$RECORD_IMGC')
+
 
 class TableStatsInfo(InfoItem):
     """Information about row level I/O operations on single table.
     """
     def __init__(self, monitor: Monitor, attributes: Dict[str, Any]):
         super().__init__(monitor, attributes)
         self._strip_attribute('MON$TABLE_NAME')
@@ -1102,7 +1261,58 @@
         """
         return self._attributes['MON$VARIABLE_NAME']
     @property
     def value(self) -> str:
         """Value of context variable.
         """
         return self._attributes['MON$VARIABLE_VALUE']
+
+# Firebird 5
+
+class CompiledStatementInfo(InfoItem):
+    """Information about compiled statement.
+
+    .. versionadded:: 1.4.0
+    """
+    def __init__(self, monitor: Monitor, attributes: Dict[str, Any]):
+        super().__init__(monitor, attributes)
+        self._strip_attribute('MON$OBJECT_NAME')
+        self._strip_attribute('MON$PACKAGE_NAME')
+        self._strip_attribute('MON$SQL_TEXT')
+        self._strip_attribute('MON$EXPLAINED_PLAN')
+    @property
+    def id(self) -> int:
+        """Compiled statement ID.
+        """
+        return self._attributes['MON$COMPILED_STATEMENT_ID']
+    @property
+    def sql(self) -> Optional[str]:
+        """Text of the SQL query.
+        """
+        return self._attributes['MON$SQL_TEXT']
+    @property
+    def plan(self) -> Optional[str]:
+        """Plan (in the explained form) of the SQL query.
+        """
+        return self._attributes.get('MON$EXPLAINED_PLAN')
+    @property
+    def object_name(self) -> Optional[str]:
+        """PSQL object name.
+        """
+        return self._attributes.get('MON$OBJECT_NAME')
+    @property
+    def object_type(self) -> Optional[ObjectType]:
+        """PSQL object type.
+        """
+        value = self._attributes.get('MON$OBJECT_TYPE')
+        return value if value is None else ObjectType(value)
+    @property
+    def package_name(self) -> Optional[str]:
+        """Package name of the PSQL object.
+        """
+        return self._attributes.get('MON$PACKAGE_NAME')
+    @property
+    def iostats(self) -> IOStatsInfo:
+        """`.IOStatsInfo` for this object.
+        """
+        return self.monitor.iostats.find(lambda io: (io.stat_id == self.stat_id)
+                                         and (io.group is Group.STATEMENT))
```

### Comparing `firebird-lib-1.3.0/src/firebird/lib/schema.py` & `firebird-lib-1.4.0/src/firebird/lib/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #coding:utf-8
 #
 # PROGRAM/MODULE: firebird-lib
 # FILE:           firebird/lib/schema.py
-# DESCRIPTION:    Module work with Firebird database schema
+# DESCRIPTION:    Module for work with Firebird database schema
 # CREATED:        21.9.2020
 #
 # The contents of this file are subject to the MIT License
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -28,15 +28,15 @@
 # Copyright (c) 2020 Firebird Project (www.firebirdsql.org)
 # All Rights Reserved.
 #
 # Contributor(s): Pavel Císař (original code)
 #                 ______________________________________
 # pylint: disable=C0302, C0301, W0212, R0902, R0912,R0913, R0914, R0915, R0904, C0103
 
-"""firebird.lib.schema - Module work with Firebird database schema
+"""firebird.lib.schema - Module for work with Firebird database schema
 
 
 """
 
 from __future__ import annotations
 from typing import Dict, Tuple, List, Any, Optional, Union
 import weakref
@@ -101,16 +101,24 @@
                 FieldType.BLOB_ID: 'BLOB_ID', FieldType.BLOB: 'BLOB',
                 FieldType.TIME: 'TIME', FieldType.DATE: 'DATE',
                 FieldType.TIMESTAMP: 'TIMESTAMP', FieldType.INT64: 'BIGINT',
                 FieldType.BOOLEAN: 'BOOLEAN'}
 
 INTEGRAL_SUBTYPES = ('UNKNOWN', 'NUMERIC', 'DECIMAL')
 
+class IndexType(Enum):
+    """Index ordering.
+    """
+    ASCENDING = 'ASCENDING'
+    DESCENDING = 'DESCENDING'
+
 class ObjectType(IntEnum):
     """Dependent type codes.
+
+    .. versionchanged:: 1.4.0 - `PACKAGE` renamed to `PACKAGE_HEADER`, added values 20-37
     """
     TABLE = 0
     VIEW = 1
     TRIGGER = 2
     DOMAIN = 3
     CHECK = 4
     PROCEDURE = 5
@@ -122,22 +130,36 @@
     CHARACTER_SET = 11
     USER_GROUP = 12
     ROLE = 13
     GENERATOR = 14
     UDF = 15
     BLOB_FILTER = 16
     COLLATION = 17
-    PACKAGE = 18
+    PACKAGE_HEADER = 18
     PACKAGE_BODY = 19
-
-class IndexType(Enum):
-    """Index ordering.
-    """
-    ASCENDING = 'ASCENDING'
-    DESCENDING = 'DESCENDING'
+    PRIVILEGE = 20
+    # Object types for DDL operations
+    DATABASE = 21
+    RELATIONS = 22
+    VIEWS = 23
+    PROCEDURES = 24
+    FUNCTIONS = 25
+    PACKAGES = 26
+    GENERATORS = 27
+    DOMAINS = 28
+    EXCEPTIONS = 29
+    ROLES = 30
+    CHARSETS = 31
+    COLLATIONS = 32
+    FILTERS = 33
+    # Codes that could be used in RDB$DEPENDENCIES or RDB$USER_PRIVILEGES
+    JOBS = 34
+    TABLESPACE = 35
+    TABLESPACES = 36
+    INDEX_CONDITION = 37
 
 class FunctionType(IntEnum):
     """Function type codes.
     """
     VALUE = 0
     BOOLEAN = 1
 
@@ -820,18 +842,19 @@
     def _get_all_indices(self) -> Tuple[DataList[Index], DataList[Index], DataList[Index]]:
         if self.__indices is None:
             self.__fail_if_closed()
             # Dummy call to _get_constraint_indices() is necessary as
             # Index.is_sys_object() that is called in Index.__init__() will
             # drop result from internal cursor and we'll not load all indices.
             self._get_constraint_indices()
-            cmd = """select RDB$INDEX_NAME, RDB$RELATION_NAME, RDB$INDEX_ID,
+            ext = '' if self.ods < 13.0 else  ', RDB$CONDITION_SOURCE'
+            cmd = f"""select RDB$INDEX_NAME, RDB$RELATION_NAME, RDB$INDEX_ID,
             RDB$UNIQUE_FLAG, RDB$DESCRIPTION, RDB$SEGMENT_COUNT, RDB$INDEX_INACTIVE,
             RDB$INDEX_TYPE, RDB$FOREIGN_KEY, RDB$SYSTEM_FLAG, RDB$EXPRESSION_SOURCE,
-            RDB$STATISTICS from RDB$INDICES"""
+            RDB$STATISTICS{ext} from RDB$INDICES"""
             indices = DataList((Index(self, row) for row in self._select(cmd)),
                                Index, 'item.name', frozen=True)
             sys_indices, user_indices = indices.split(lambda i: i.is_sys_object(), frozen=True)
             self.__indices = (user_indices, sys_indices, indices)
         return self.__indices
     def _get_all_generators(self) -> Tuple[DataList[Sequence], DataList[Sequence], DataList[Sequence]]:
         if self.__generators is None:
@@ -1015,14 +1038,17 @@
                                'THEN', 'TIME', 'TIMESTAMP', 'TIMEZONE_HOUR',
                                'TIMEZONE_MINUTE', 'TO', 'TRAILING', 'TRIGGER', 'TRIM',
                                'TRUE', 'UNBOUNDED', 'UNION', 'UNIQUE', 'UNKNOWN', 'UPDATE',
                                'UPDATING', 'UPPER', 'USER', 'USING', 'VALUE', 'VALUES',
                                'VAR_POP', 'VAR_SAMP', 'VARBINARY', 'VARCHAR', 'VARIABLE',
                                'VARYING', 'VIEW', 'WHEN', 'WHERE', 'WHILE', 'WINDOW',
                                'WITH', 'WITHOUT', 'YEAR']
+        elif self.ods == 13.1: # Firebird 5.0
+            self._ic.execute("SELECT RDB$KEYWORD_NAME FROM RDB$KEYWORDS WHERE RDB$KEYWORD_RESERVED")
+            self._reserved_ = [r[0] for r in self._ic]
         else:
             raise Error(f"Unsupported ODS version: {self.ods}")
         self.__attrs = self._select_row('select * from RDB$DATABASE')
         self._default_charset_name = self.__attrs['RDB$CHARACTER_SET_NAME'].strip()
         self._ic.execute("select RDB$OWNER_NAME from RDB$RELATIONS where RDB$RELATION_NAME = 'RDB$DATABASE'")
         self.__owner = self._ic.fetchone()[0].strip()
         # Load enumerate types defined in RDB$TYPES table
@@ -1122,28 +1148,31 @@
         elif itype is ObjectType.USER:
             res = self._get_users().get(name)
             if not res:
                 res = UserInfo(user_name=name)
                 self.__users.append(res)
             result = res
         elif itype is ObjectType.COLUMN:
-            result = self.all_tables.get(name).columns.get(subname)
+            if subname is None:
+                result = self.all_domains.get(name)
+            else:
+                result = self.all_tables.get(name).columns.get(subname)
         elif itype is ObjectType.INDEX:
             result = self.all_indices.get(name)
         elif itype is ObjectType.CHARACTER_SET:
             result = self.character_sets.get(name)
         elif itype is ObjectType.ROLE:
             result = self.roles.get(name)
         elif itype is ObjectType.GENERATOR:
             result = self.all_generators.get(name)
         elif itype is ObjectType.UDF:
             result = self.all_functions.get(name)
         elif itype is ObjectType.COLLATION:
             result = self.collations.get(name)
-        elif itype in (ObjectType.PACKAGE, ObjectType.PACKAGE_BODY): # Package
+        elif itype in (ObjectType.PACKAGE_HEADER, ObjectType.PACKAGE_BODY): # Package
             result = self.packages.get(name)
         return result
     def get_metadata_ddl(self, *, sections=SCRIPT_DEFAULT_ORDER) -> List[str]:
         """Return list of DDL SQL commands for creation of specified categories of database objects.
 
         Keyword Args:
             sections (list): List of section identifiers.
@@ -2306,22 +2335,22 @@
     @property
     def index_type(self) -> IndexType:
         """Index type (ASCENDING or DESCENDING).
         """
         return (IndexType.DESCENDING if self._attributes['RDB$INDEX_TYPE'] == 1
                 else IndexType.ASCENDING)
     @property
-    def partner_index(self) -> Index:
+    def partner_index(self) -> Optional[Index]:
         """Associated unique/primary key :class:`Index` instance, or None.
         """
         return (self.schema.all_indices.get(pname) if (pname := self._attributes['RDB$FOREIGN_KEY'])
                 else None)
     @property
-    def expression(self) -> str:
-        """Source of an expression or None.
+    def expression(self) -> Optional[str]:
+        """Index expression or None.
         """
         return self._attributes['RDB$EXPRESSION_SOURCE']
     @property
     def statistics(self) -> float:
         """Latest selectivity of the index.
         """
         return self._attributes['RDB$STATISTICS']
@@ -2351,18 +2380,26 @@
         return self.__segment_statistics
     @property
     def segments(self) -> DataList[TableColumn]:
         """List of index segments (table columns).
         """
         return DataList(self.table.columns.get(colname) for colname in self.segment_names)
     @property
-    def constraint(self) -> Constraint:
+    def constraint(self) -> Optional[Constraint]:
         """`Constraint` instance that uses this index or None.
         """
         return self.schema.constraints.get(self.schema._get_constraint_indices().get(self.name))
+    # Firebird 5
+    @property
+    def condition(self) -> Optional[str]:
+        """Index condition or None.
+
+        .. versionadded:: 1.4.0
+        """
+        return self._attributes['RDB$CONDITION_SOURCE']
 
 class ViewColumn(SchemaItem):
     """Represents view column.
 
     Supported SQL actions:
         `comment`
     """
@@ -4751,15 +4788,15 @@
 
     Supported SQL actions:
         `create` (body=bool), `recreate` (body=bool), `create_or_alter` (body=bool),
         `alter` (header=string_or_list), `drop` (body=bool)
     """
     def __init__(self, schema: Schema, attributes: Dict[str, Any]):
         super().__init__(schema, attributes)
-        self._type_code.extend([ObjectType.PACKAGE, ObjectType.PACKAGE_BODY])
+        self._type_code.extend([ObjectType.PACKAGE_HEADER, ObjectType.PACKAGE_BODY])
         self._actions.extend(['create', 'recreate', 'create_or_alter', 'alter', 'drop',
                               'comment'])
         self._strip_attribute('RDB$PACKAGE_NAME')
         self._strip_attribute('RDB$SECURITY_CLASS')
         self._strip_attribute('RDB$OWNER_NAME')
     def _get_create_sql(self, **params) -> str:
         "Returns SQL command to CREATE package."
```

### Comparing `firebird-lib-1.3.0/src/firebird/lib/trace.py` & `firebird-lib-1.4.0/src/firebird/lib/trace.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/src/firebird_lib.egg-info/PKG-INFO` & `firebird-lib-1.4.0/src/firebird_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebird-lib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Firebird driver extension library
 Author-email: Pavel Cisar <pcisar@users.sourceforge.net>
 License: MIT License
         
         Copyright (c) 2020 FirebirdSQL
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `firebird-lib-1.3.0/src/firebird_lib.egg-info/SOURCES.txt` & `firebird-lib-1.4.0/src/firebird_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/test/test_gstat.py` & `firebird-lib-1.4.0/test/test_gstat.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/test/test_log.py` & `firebird-lib-1.4.0/test/test_log.py`

 * *Files identical despite different names*

### Comparing `firebird-lib-1.3.0/test/test_monitor.py` & `firebird-lib-1.4.0/test/test_monitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,22 +30,19 @@
 #
 # Contributor(s): Pavel Císař (original code)
 #                 ______________________________________
 
 import unittest
 import sys, os
 import datetime
-from contextlib import closing
-from re import finditer
-from pprint import pprint
 from firebird.base.collections import DataList
 from firebird.driver import *
 from firebird.lib.monitor import *
 from firebird.lib.schema import CharacterSet
-from firebird.lib import schema as sm
+#from firebird.lib import schema as sm
 from io import StringIO
 
 FB30 = '3.0'
 FB40 = '4.0'
 FB50 = '5.0'
 
 if driver_config.get_server('local') is None:
@@ -183,23 +180,25 @@
                 self.assertFalse(m.closed)
     def test_03_DatabaseInfo(self):
         with Monitor(self.con) as m:
             self.assertEqual(m.db.name.upper(), self.dbfile.upper())
             self.assertEqual(m.db.page_size, 8192)
             if self.version == FB30:
                 self.assertEqual(m.db.ods, 12.0)
-            else:
+            elif self.version == FB40:
                 self.assertEqual(m.db.ods, 13.0)
+            else:
+                self.assertEqual(m.db.ods, 13.1)
             self.assertIsInstance(m.db.oit, int)
             self.assertIsInstance(m.db.oat, int)
             self.assertIsInstance(m.db.ost, int)
             self.assertIsInstance(m.db.next_transaction, int)
             self.assertIsInstance(m.db.cache_size, int)
             self.assertEqual(m.db.sql_dialect, 3)
-            self.assertIs(m.db.shutdown_mode, ShutdownMode.ONLINE)
+            self.assertIs(m.db.shutdown_mode, ShutdownMode.NORMAL)
             self.assertEqual(m.db.sweep_interval, 20000)
             self.assertFalse(m.db.read_only)
             self.assertTrue(m.db.forced_writes)
             self.assertTrue(m.db.reserve_space)
             self.assertIsInstance(m.db.created, datetime.datetime)
             self.assertIsInstance(m.db.pages, int)
             self.assertIs(m.db.backup_state, BackupState.NORMAL)
@@ -210,14 +209,29 @@
             self.assertEqual(m.db.iostats.stat_id, m.db.stat_id)
             # TableStats
             for table_name, stats in m.db.tablestats.items():
                 self.assertIsNotNone(self.con.schema.all_tables.get(table_name))
                 self.assertIsInstance(stats, TableStatsInfo)
                 self.assertEqual(stats.stat_id, m.db.stat_id)
                 self.assertEqual(stats.owner, m.db)
+            # Firebird 4 properties
+            if self.version == FB30:
+                self.assertIsNone(m.db.crypt_state)
+                self.assertIsNone(m.db.guid)
+                self.assertIsNone(m.db.file_id)
+                self.assertIsNone(m.db.next_attachment)
+                self.assertIsNone(m.db.next_statement)
+                self.assertIsNone(m.db.replica_mode)
+            else:
+                self.assertEqual(m.db.crypt_state, CryptState.NOT_ENCRYPTED)
+                self.assertEqual(m.db.guid, UUID('53e6200c-2b09-42a8-8384-e07bc9aa2883'))
+                self.assertIsInstance(m.db.file_id, str)
+                self.assertGreater(m.db.next_attachment, 0)
+                self.assertGreater(m.db.next_statement, 0)
+                self.assertEqual(m.db.replica_mode, ReplicaMode.NONE)
     def test_04_AttachmentInfo(self):
         with Monitor(self.con) as m:
             sql = "select RDB$SET_CONTEXT('USER_SESSION','TESTVAR','TEST_VALUE') from rdb$database"
             with self.con.cursor() as c:
                 c.execute(sql)
                 c.fetchone()
                 #
@@ -237,16 +251,18 @@
                 self.assertEqual(s.character_set.name, 'UTF8')
                 self.assertIsInstance(s.timestamp, datetime.datetime)
                 self.assertIsInstance(s.transactions, list)
                 self.assertIn(s.auth_method, ['Srp', 'Srp256', 'Win_Sspi', 'Legacy_Auth'])
                 self.assertIsInstance(s.client_version, str)
                 if self.version == FB30:
                     self.assertEqual(s.remote_version, 'P15')
-                else:
+                elif self.version == FB40:
                     self.assertEqual(s.remote_version, 'P17')
+                else:
+                    self.assertEqual(s.remote_version, 'P18')
                 self.assertIsInstance(s.remote_os_user, str)
                 self.assertIsInstance(s.remote_host, str)
                 self.assertFalse(s.system)
                 for x in s.transactions:
                     self.assertIsInstance(x, TransactionInfo)
                 self.assertIsInstance(s.statements, list)
                 for x in s.statements:
@@ -282,14 +298,35 @@
                     self.assertEqual(len(m.attachments), cnt)
                     self.assertIsNone(m.attachments.get(att_id))
                     # Current attachment
                     with self.assertRaises(Error) as cm:
                         m.this_attachment.terminate()
                     self.assertTupleEqual(cm.exception.args,
                                           ("Can't terminate current session.",))
+                # Firebird 4
+                if self.version == FB30:
+                    self.assertIsNone(s.idle_timeout)
+                    self.assertIsNone(s.idle_timer)
+                    self.assertIsNone(s.statement_timeout)
+                    self.assertIsNone(s.wire_compressed)
+                    self.assertIsNone(s.wire_encrypted)
+                    self.assertIsNone(s.wire_crypt_plugin)
+                else:
+                    self.assertEqual(s.idle_timeout, 0)
+                    self.assertIsNone(s.idle_timer)
+                    self.assertEqual(s.statement_timeout, 0)
+                    self.assertFalse(s.wire_compressed)
+                    self.assertTrue(s.wire_encrypted)
+                    self.assertEqual(s.wire_crypt_plugin, 'ChaCha64')
+                # Firebird 5
+                if self.version in [FB30, FB40]:
+                    self.assertIsNone(s.session_timezone)
+                else:
+                    self.assertIsInstance(s.session_timezone, str)
+
     def test_05_TransactionInfo(self):
         c = self.con.cursor()
         sql = "select RDB$SET_CONTEXT('USER_TRANSACTION','TESTVAR','TEST_VALUE') from rdb$database"
         c.execute(sql)
         c.fetchone()
         #
         with Monitor(self.con) as m:
@@ -299,15 +336,18 @@
             self.assertEqual(s.id, m._ic.transaction.info.id)
             self.assertIs(s.attachment, m.this_attachment)
             self.assertIsInstance(s.state, State)
             self.assertIsInstance(s.timestamp, datetime.datetime)
             self.assertIsInstance(s.top, int)
             self.assertIsInstance(s.oldest, int)
             self.assertIsInstance(s.oldest_active, int)
-            self.assertIs(s.isolation_mode, IsolationMode.READ_COMMITTED_RV)
+            if self.version == FB30:
+                self.assertIs(s.isolation_mode, IsolationMode.READ_COMMITTED_RV)
+            else: # Firebird 4+
+                self.assertIs(s.isolation_mode, IsolationMode.READ_COMMITTED_READ_CONSISTENCY)
             self.assertEqual(s.lock_timeout, -1)
             self.assertIsInstance(s.statements, list)
             for x in s.statements:
                 self.assertIsInstance(x, StatementInfo)
             self.assertIsInstance(s.variables, list)
             self.assertIs(s.iostats.group, Group.TRANSACTION)
             self.assertEqual(s.iostats.stat_id, s.stat_id)
@@ -330,15 +370,15 @@
                 self.assertIsInstance(stats, TableStatsInfo)
                 self.assertEqual(stats.stat_id, s.stat_id)
                 self.assertEqual(stats.owner, s)
         c.close()
     def test_06_StatementInfo(self):
         with Monitor(self.con) as m:
             m.take_snapshot()
-            s = m.this_attachment.statements[0]
+            s: StatementInfo = m.this_attachment.statements[0]
             #
             self.assertIsInstance(s.id, int)
             self.assertIs(s.attachment, m.this_attachment)
             self.assertEqual(s.transaction.id, m.transactions[0].id)
             self.assertIsInstance(s.state, State)
             self.assertIsInstance(s.timestamp, datetime.datetime)
             self.assertEqual(s.sql, "select * from mon$attachments")
@@ -376,14 +416,29 @@
             self.assertFalse(s.is_idle())
             # TableStats
             for table_name, stats in s.tablestats.items():
                 self.assertIsNotNone(self.con.schema.all_tables.get(table_name))
                 self.assertIsInstance(stats, TableStatsInfo)
                 self.assertEqual(stats.stat_id, s.stat_id)
                 self.assertEqual(stats.owner, s)
+            # Firebird 4
+            if self.version == FB30:
+                self.assertIsNone(s.timeout)
+                self.assertIsNone(s.timer)
+            else:
+                self.assertEqual(s.timeout, 0)
+                self.assertIsNone(s.timer)
+            # Firebird 5
+            if self.version in [FB30, FB40]:
+                self.assertIsNone(s.compiled_statement)
+            else:
+                self.assertIsInstance(s.compiled_statement, CompiledStatementInfo)
+                self.assertEqual(s.sql, s.compiled_statement.sql)
+                self.assertEqual(s.plan, s.compiled_statement.plan)
+                self.assertEqual(s._attributes['MON$COMPILED_STATEMENT_ID'], s.compiled_statement.id)
     def test_07_CallStackInfo(self):
         with Monitor(self.con) as m:
             m.take_snapshot()
             stmt = m.this_attachment.statements[0]
             # We have to use mocks for callstack
             stack = DataList(key_expr='item.id')
             stack.append(CallStackInfo(m,
@@ -434,14 +489,15 @@
             #
             x = m.callstack.get(3)
             self.assertIs(x.caller, s)
             self.assertIsInstance(x.dbobject, Procedure)
             self.assertEqual(x.dbobject.name, 'SHIP_ORDER')
             self.assertEqual(x.object_type, 5) # procedure
             self.assertEqual(x.object_name, 'SHIP_ORDER')
+
     def test_08_IOStatsInfo(self):
         with Monitor(self.con) as m:
             m.take_snapshot()
             #
             for io in m.iostats:
                 self.assertIs(io, io.owner.iostats)
             #
@@ -466,14 +522,19 @@
             self.assertIsInstance(s.backversion_reads, int)
             self.assertIsInstance(s.fragment_reads, int)
             self.assertIsInstance(s.repeated_reads, int)
             self.assertIsInstance(s.memory_used, int)
             self.assertIsInstance(s.memory_allocated, int)
             self.assertIsInstance(s.max_memory_used, int)
             self.assertIsInstance(s.max_memory_allocated, int)
+            # Firebird 4
+            if self.version == FB30:
+                self.assertIsNone(s.intermediate_gc)
+            else:
+                self.assertEqual(s.intermediate_gc, 0)
     def test_09_ContextVariableInfo(self):
         c = self.con.cursor()
         sql = "select RDB$SET_CONTEXT('USER_SESSION','SVAR','TEST_VALUE') from rdb$database"
         c.execute(sql)
         c.fetchone()
         c2 = self.con.cursor()
         sql = "select RDB$SET_CONTEXT('USER_TRANSACTION','TVAR','TEST_VALUE') from rdb$database"
@@ -481,15 +542,15 @@
         c2.fetchone()
         #
         with Monitor(self.con) as m:
             m.take_snapshot()
             #
             self.assertEqual(len(m.variables), 2)
             #
-            s = m.variables[0]
+            s: ContextVariableInfo = m.variables[0]
             self.assertIs(s.attachment, m.this_attachment)
             self.assertIsNone(s.transaction)
             self.assertEqual(s.name, 'SVAR')
             self.assertEqual(s.value, 'TEST_VALUE')
             self.assertTrue(s.is_attachment_var())
             self.assertFalse(s.is_transaction_var())
             #
@@ -499,11 +560,22 @@
                           m.transactions.get(c.transaction.info.id))
             self.assertEqual(s.name, 'TVAR')
             self.assertEqual(s.value, 'TEST_VALUE')
             self.assertFalse(s.is_attachment_var())
             self.assertTrue(s.is_transaction_var())
         c.close()
         c2.close()
+    def test_10_CompiledStatementInfo(self):
+        with Monitor(self.con) as m:
+            m.take_snapshot()
+            #
+            if self.version in [FB30, FB40]:
+                self.assertEqual(len(m.compiled_statements), 0)
+            else:
+                self.assertEqual(len(m.compiled_statements), 2)
+                s: CompiledStatementInfo = m.compiled_statements[0]
+                #
+                self.assertEqual(s.sql, "select * from mon$compiled_statements")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `firebird-lib-1.3.0/test/test_schema.py` & `firebird-lib-1.4.0/test/test_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,28 +187,46 @@
             self.assertFalse(s.closed)
         self.assertTrue(s.closed)
 
     def test_02_SchemaFromConnection(self):
         s = self.con.schema
         self.assertDictEqual(s.param_type_from,
                              {0: 'DATATYPE', 1: 'DOMAIN', 2: 'TYPE OF DOMAIN', 3: 'TYPE OF COLUMN'})
-        self.assertDictEqual(s.object_types,
-                             {0: 'RELATION', 1: 'VIEW', 2: 'TRIGGER', 3: 'COMPUTED_FIELD',
-                              4: 'VALIDATION', 5: 'PROCEDURE', 6: 'EXPRESSION_INDEX',
-                              7: 'EXCEPTION', 8: 'USER', 9: 'FIELD', 10: 'INDEX',
-                              11: 'CHARACTER_SET', 12: 'USER_GROUP', 13: 'ROLE',
-                              14: 'GENERATOR', 15: 'UDF', 16: 'BLOB_FILTER', 17: 'COLLATION',
-                              18:'PACKAGE', 19:'PACKAGE BODY'})
-        self.assertDictEqual(s.object_type_codes,
-                             {'INDEX': 10, 'EXCEPTION': 7, 'GENERATOR': 14, 'COLLATION': 17,
-                              'UDF': 15, 'EXPRESSION_INDEX': 6, 'FIELD': 9,
-                              'COMPUTED_FIELD': 3, 'TRIGGER': 2, 'RELATION': 0, 'USER': 8,
-                              'USER_GROUP': 12, 'BLOB_FILTER': 16, 'ROLE': 13,
-                              'VALIDATION': 4, 'PROCEDURE': 5, 'VIEW': 1, 'CHARACTER_SET':11,
-                              'PACKAGE':18, 'PACKAGE BODY':19})
+        if self.version in (FB30, FB40):
+            self.assertDictEqual(s.object_types,
+                                 {0: 'RELATION', 1: 'VIEW', 2: 'TRIGGER', 3: 'COMPUTED_FIELD',
+                                  4: 'VALIDATION', 5: 'PROCEDURE', 6: 'EXPRESSION_INDEX',
+                                  7: 'EXCEPTION', 8: 'USER', 9: 'FIELD', 10: 'INDEX',
+                                  11: 'CHARACTER_SET', 12: 'USER_GROUP', 13: 'ROLE',
+                                  14: 'GENERATOR', 15: 'UDF', 16: 'BLOB_FILTER', 17: 'COLLATION',
+                                  18:'PACKAGE', 19:'PACKAGE BODY'})
+        else: # Firebird 5.0
+            self.assertDictEqual(s.object_types,
+                                 {0: 'RELATION', 1: 'VIEW', 2: 'TRIGGER', 3: 'COMPUTED_FIELD',
+                                  4: 'VALIDATION', 5: 'PROCEDURE', 6: 'INDEX_EXPRESSION',
+                                  7: 'EXCEPTION', 8: 'USER', 9: 'FIELD', 10: 'INDEX',
+                                  11: 'CHARACTER_SET', 12: 'USER_GROUP', 13: 'ROLE',
+                                  14: 'GENERATOR', 15: 'UDF', 16: 'BLOB_FILTER', 17: 'COLLATION',
+                                  18:'PACKAGE', 19:'PACKAGE BODY', 37: 'INDEX_CONDITION'})
+        if self.version in (FB30, FB40):
+            self.assertDictEqual(s.object_type_codes,
+                                 {'INDEX': 10, 'EXCEPTION': 7, 'GENERATOR': 14, 'COLLATION': 17,
+                                  'UDF': 15, 'EXPRESSION_INDEX': 6, 'FIELD': 9,
+                                  'COMPUTED_FIELD': 3, 'TRIGGER': 2, 'RELATION': 0, 'USER': 8,
+                                  'USER_GROUP': 12, 'BLOB_FILTER': 16, 'ROLE': 13,
+                                  'VALIDATION': 4, 'PROCEDURE': 5, 'VIEW': 1, 'CHARACTER_SET':11,
+                                  'PACKAGE':18, 'PACKAGE BODY':19})
+        else: # Firebird 5.0
+            self.assertDictEqual(s.object_type_codes,
+                                 {'INDEX': 10, 'EXCEPTION': 7, 'GENERATOR': 14, 'COLLATION': 17,
+                                  'UDF': 15, 'INDEX_EXPRESSION': 6, 'FIELD': 9,
+                                  'COMPUTED_FIELD': 3, 'TRIGGER': 2, 'RELATION': 0, 'USER': 8,
+                                  'USER_GROUP': 12, 'BLOB_FILTER': 16, 'ROLE': 13,
+                                  'VALIDATION': 4, 'PROCEDURE': 5, 'VIEW': 1, 'CHARACTER_SET':11,
+                                  'PACKAGE':18, 'PACKAGE BODY':19, 'INDEX_CONDITION': 37})
         self.assertDictEqual(s.character_set_names,
                              {0: 'NONE', 1: 'BINARY', 2: 'ASCII7', 3: 'SQL_TEXT', 4: 'UTF-8',
                               5: 'SJIS', 6: 'EUCJ', 9: 'DOS_737', 10: 'DOS_437', 11: 'DOS_850',
                               12: 'DOS_865', 13: 'DOS_860', 14: 'DOS_863', 15: 'DOS_775',
                               16: 'DOS_858', 17: 'DOS_862', 18: 'DOS_864', 19: 'NEXT',
                               21: 'ANSI', 22: 'ISO-8859-2', 23: 'ISO-8859-3', 34: 'ISO-8859-4',
                               35: 'ISO-8859-5', 36: 'ISO-8859-6', 37: 'ISO-8859-7',
@@ -334,34 +352,50 @@
             self.assertEqual(len(s.sys_tables), 50)
             self.assertEqual(len(s.all_tables), 66)
             self.assertEqual(len(s.sys_procedures), 0)
             self.assertEqual(len(s.all_procedures), 11)
             self.assertEqual(len(s.constraints), 110)
             self.assertEqual(len(s.sys_functions), 0)
             self.assertEqual(len(s.all_functions), 6)
-        else:
+            self.assertEqual(len(s.sys_triggers), 57)
+            self.assertEqual(len(s.all_triggers), 65)
+        elif self.version == FB40:
             self.assertEqual(len(s.sys_domains), 297)
             self.assertEqual(len(s.all_domains), 312)
             self.assertEqual(len(s.sys_indices), 85)
             self.assertEqual(len(s.all_indices), 97)
             self.assertEqual(len(s.sys_tables), 54)
             self.assertEqual(len(s.all_tables), 70)
             self.assertEqual(len(s.sys_procedures), 1)
             self.assertEqual(len(s.all_procedures), 12)
             self.assertEqual(len(s.constraints), 113)
             self.assertEqual(len(s.sys_functions), 1)
             self.assertEqual(len(s.all_functions), 7)
+            self.assertEqual(len(s.sys_triggers), 57)
+            self.assertEqual(len(s.all_triggers), 65)
+        else:
+            self.assertEqual(len(s.sys_domains), 306)
+            self.assertEqual(len(s.all_domains), 321)
+            self.assertEqual(len(s.sys_indices), 86)
+            self.assertEqual(len(s.all_indices), 98)
+            self.assertEqual(len(s.sys_tables), 56)
+            self.assertEqual(len(s.all_tables), 72)
+            self.assertEqual(len(s.sys_procedures), 10)
+            self.assertEqual(len(s.all_procedures), 21)
+            self.assertEqual(len(s.constraints), 113)
+            self.assertEqual(len(s.sys_functions), 7)
+            self.assertEqual(len(s.all_functions), 13)
+            self.assertEqual(len(s.sys_triggers), 54)
+            self.assertEqual(len(s.all_triggers), 62)
         self.assertEqual(len(s.indices), 12)
         self.assertEqual(len(s.tables), 16)
         self.assertEqual(len(s.views), 1)
         self.assertEqual(len(s.sys_views), 0)
         self.assertEqual(len(s.all_views), 1)
         self.assertEqual(len(s.triggers), 8)
-        self.assertEqual(len(s.sys_triggers), 57)
-        self.assertEqual(len(s.all_triggers), 65)
         self.assertEqual(len(s.procedures), 11)
         self.assertEqual(len(s.roles), 2)
         self.assertEqual(len(s.dependencies), 168)
         self.assertEqual(len(s.functions), 6)
         self.assertEqual(len(s.files), 0)
         #
         self.assertIsInstance(s.collations[0], sm.Collation)
@@ -442,16 +476,18 @@
         self.assertListEqual(c.actions, ['comment'])
         self.assertTrue(c.is_sys_object())
         self.assertEqual(c.get_quoted_name(), 'ES_ES')
         self.assertListEqual(c.get_dependents(), [])
         self.assertListEqual(c.get_dependencies(), [])
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$263')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$283')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$337')
         self.assertEqual(c.owner_name, 'SYSDBA')
         #
         self.assertEqual(c.id, 10)
         self.assertEqual(c.character_set.name, 'ISO8859_1')
         self.assertIsNone(c.base_collation)
         self.assertEqual(c.attributes, 1)
         self.assertEqual(c.specific_attributes,
@@ -505,16 +541,18 @@
         self.assertListEqual(c.actions, ['alter', 'comment'])
         self.assertTrue(c.is_sys_object())
         self.assertEqual(c.get_quoted_name(), 'UTF8')
         self.assertListEqual(c.get_dependents(), [])
         self.assertListEqual(c.get_dependencies(), [])
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$166')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$186')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$240')
         self.assertEqual(c.owner_name, 'SYSDBA')
         #
         self.assertEqual(c.id, 4)
         self.assertEqual(c.bytes_per_character, 4)
         self.assertEqual(c.default_collate.name, 'UTF8')
         self.assertListEqual([x.name for x in c.collations],
                              ['UTF8', 'UCS_BASIC', 'UNICODE', 'UNICODE_CI', 'UNICODE_CI_AI'])
@@ -555,16 +593,18 @@
         self.assertIsInstance(d.dependent, sm.Procedure)
         self.assertEqual(d.depended_on_name, 'UNKNOWN_EMP_ID')
         self.assertEqual(d.depended_on_type, 7)
         self.assertIsInstance(d.depended_on, sm.DatabaseException)
         self.assertListEqual(c.get_dependencies(), [])
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$476')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$604')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$617')
         self.assertEqual(c.owner_name, 'SYSDBA')
         #
         self.assertEqual(c.id, 1)
         self.assertEqual(c.message, "Invalid employee number or project id.")
         #
         self.assertEqual(c.get_sql_for('create'),
                          "CREATE EXCEPTION UNKNOWN_EMP_ID 'Invalid employee number or project id.'")
@@ -620,16 +660,18 @@
         self.assertEqual(d.depended_on_type, 14)
         self.assertIsInstance(d.depended_on, sm.Sequence)
         self.assertListEqual(c.get_dependencies(), [])
         #
         self.assertEqual(c.id, 12)
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$429')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$600')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$613')
         self.assertEqual(c.owner_name, 'SYSDBA')
         self.assertEqual(c.inital_value, 0)
         self.assertEqual(c.increment, 1)
         self.assertEqual(c.value, 145)
         #
         self.assertEqual(c.get_sql_for('create'), "CREATE SEQUENCE EMP_NO_GEN")
         self.assertEqual(c.get_sql_for('drop'), "DROP SEQUENCE EMP_NO_GEN")
@@ -743,23 +785,24 @@
                          "ALTER TABLE T5 ALTER COLUMN ID RESTART")
         self.assertEqual(c.get_sql_for('alter', restart=100),
                          "ALTER TABLE T5 ALTER COLUMN ID RESTART WITH 100")
     def test_08_Index(self):
         s = Schema()
         s.bind(self.con)
         # System index
-        c = s.all_indices.get('RDB$INDEX_0')
+        c: Index = s.all_indices.get('RDB$INDEX_0')
         # common properties
         self.assertEqual(c.name, 'RDB$INDEX_0')
         self.assertIsNone(c.description)
         self.assertListEqual(c.actions, ['activate', 'recompute', 'comment'])
         self.assertTrue(c.is_sys_object())
         self.assertEqual(c.get_quoted_name(), 'RDB$INDEX_0')
         self.assertListEqual(c.get_dependents(), [])
         self.assertListEqual(c.get_dependencies(), [])
+        self.assertIsNone(c.condition)
         #
         self.assertEqual(c.table.name, 'RDB$RELATIONS')
         self.assertListEqual(c.segment_names, ['RDB$RELATION_NAME'])
         # user index
         c = s.all_indices.get('MAXSALX')
         # common properties
         self.assertEqual(c.name, 'MAXSALX')
@@ -771,14 +814,15 @@
         self.assertListEqual(c.get_dependencies(), [])
         #
         self.assertEqual(c.id, 3)
         self.assertEqual(c.table.name, 'JOB')
         self.assertEqual(c.index_type, IndexType.DESCENDING)
         self.assertIsNone(c.partner_index)
         self.assertIsNone(c.expression)
+        self.assertIsNone(c.condition)
         # startswith() is necessary, because Python 3 returns more precise value.
         self.assertTrue(str(c.statistics).startswith('0.0384615398943'))
         self.assertListEqual(c.segment_names, ['JOB_COUNTRY', 'MAX_SALARY'])
         self.assertEqual(len(c.segments), 2)
         for segment in c.segments:
             self.assertIsInstance(segment, sm.TableColumn)
         self.assertEqual(c.segments[0].name, 'JOB_COUNTRY')
@@ -857,16 +901,18 @@
         self.assertListEqual(c.actions, ['comment'])
         self.assertTrue(c.is_sys_object())
         self.assertEqual(c.get_quoted_name(), 'RDB$6')
         self.assertListEqual(c.get_dependents(), [])
         self.assertListEqual(c.get_dependencies(), [])
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$439')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$460')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$473')
         self.assertEqual(c.owner_name, 'SYSDBA')
         # User domain
         c = s.all_domains.get('PRODTYPE')
         # common properties
         self.assertEqual(c.name, 'PRODTYPE')
         self.assertIsNone(c.description)
         self.assertListEqual(c.actions, ['comment', 'create',
@@ -1166,18 +1212,22 @@
         #
         self.assertEqual(c.id, 131)
         self.assertEqual(c.dbkey_length, 8)
         if self.version == FB30:
             self.assertEqual(c.format, 1)
             self.assertEqual(c.security_class, 'SQL$440')
             self.assertEqual(c.default_class, 'SQL$DEFAULT54')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.format, 2)
             self.assertEqual(c.security_class, 'SQL$586')
             self.assertEqual(c.default_class, 'SQL$DEFAULT58')
+        else: # FB5
+            self.assertEqual(c.format, 2)
+            self.assertEqual(c.security_class, 'SQL$599')
+            self.assertEqual(c.default_class, 'SQL$DEFAULT60')
         self.assertEqual(c.table_type, RelationType.PERSISTENT)
         self.assertIsNone(c.external_file)
         self.assertEqual(c.owner_name, 'SYSDBA')
         self.assertEqual(c.flags, 1)
         self.assertEqual(c.primary_key.name, 'INTEG_27')
         self.assertListEqual([x.name for x in c.foreign_keys],
                              ['INTEG_28', 'INTEG_29'])
@@ -1319,24 +1369,34 @@
                                   ('DEPARTMENT', None, 0), ('EMPLOYEE', None, 0), ('EMPLOYEE', 'EMP_NO', 0),
                                   ('EMPLOYEE', 'FIRST_NAME', 0), ('EMPLOYEE', 'LAST_NAME', 0),
                                   ('EMPLOYEE', 'PHONE_EXT', 0), ('DEPARTMENT', 'LOCATION', 0),
                                   ('DEPARTMENT', 'PHONE_NO', 0)])
             self.assertEqual(c.id, 132)
             self.assertEqual(c.security_class, 'SQL$444')
             self.assertEqual(c.default_class, 'SQL$DEFAULT55')
-        else:
+        elif self.version == FB40:
             self.assertListEqual([(x.depended_on_name, x.field_name, x.depended_on_type) for x in d],
                                  [('DEPARTMENT', 'DEPT_NO', 0), ('EMPLOYEE', 'DEPT_NO', 0),
                                   ('DEPARTMENT', None, 0), ('EMPLOYEE', None, 0),
                                   ('EMPLOYEE', 'EMP_NO', 0), ('EMPLOYEE', 'LAST_NAME', 0),
                                   ('EMPLOYEE', 'PHONE_EXT', 0), ('DEPARTMENT', 'PHONE_NO', 0),
                                   ('EMPLOYEE', 'FIRST_NAME', 0), ('DEPARTMENT', 'LOCATION', 0)])
             self.assertEqual(c.id, 144)
             self.assertEqual(c.security_class, 'SQL$587')
             self.assertEqual(c.default_class, 'SQL$DEFAULT71')
+        else: # FB5
+            self.assertListEqual([(x.depended_on_name, x.field_name, x.depended_on_type) for x in d],
+                                 [('DEPARTMENT', 'DEPT_NO', 0), ('EMPLOYEE', 'DEPT_NO', 0),
+                                  ('DEPARTMENT', None, 0), ('EMPLOYEE', None, 0),
+                                  ('EMPLOYEE', 'EMP_NO', 0), ('EMPLOYEE', 'LAST_NAME', 0),
+                                  ('EMPLOYEE', 'PHONE_EXT', 0), ('DEPARTMENT', 'PHONE_NO', 0),
+                                  ('EMPLOYEE', 'FIRST_NAME', 0), ('DEPARTMENT', 'LOCATION', 0)])
+            self.assertEqual(c.id, 144)
+            self.assertEqual(c.security_class, 'SQL$600')
+            self.assertEqual(c.default_class, 'SQL$DEFAULT73')
         #
         self.assertEqual(c.sql, """SELECT
     emp_no, first_name, last_name, phone_ext, location, phone_no
     FROM employee, department
     WHERE employee.dept_no = department.dept_no""")
         self.assertEqual(c.dbkey_length, 16)
         self.assertEqual(c.format, 1)
@@ -1611,17 +1671,20 @@
         self.assertListEqual([(x.depended_on_name, x.field_name, x.depended_on_type) for x in d],
                              [('EMPLOYEE_PROJECT', 'PROJ_ID', 0), ('EMPLOYEE_PROJECT', 'EMP_NO', 0),
                               ('EMPLOYEE_PROJECT', None, 0)])
         #
         if self.version == FB30:
             self.assertEqual(c.id, 1)
             self.assertEqual(c.security_class, 'SQL$473')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.id, 2)
             self.assertEqual(c.security_class, 'SQL$612')
+        else: # FB5
+            self.assertEqual(c.id, 11)
+            self.assertEqual(c.security_class, 'SQL$625')
         self.assertEqual(c.source, """BEGIN
 	FOR SELECT proj_id
 		FROM employee_project
 		WHERE emp_no = :emp_no
 		INTO :proj_id
 	DO
 		SUSPEND;
@@ -2334,17 +2397,20 @@
         self.assertIsNone(c.package)
         self.assertIsNone(c.engine_mame)
         self.assertIsNone(c.private_flag)
         self.assertEqual(c.source, 'BEGIN\n  RETURN X+1;\nEND')
         if self.version == FB30:
             self.assertEqual(c.id, 3)
             self.assertEqual(c.security_class, 'SQL$588')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.id, 4)
             self.assertEqual(c.security_class, 'SQL$609')
+        else: # FB5
+            self.assertEqual(c.id, 10)
+            self.assertEqual(c.security_class, 'SQL$622')
         self.assertTrue(c.valid_blr)
         self.assertEqual(c.owner_name, 'SYSDBA')
         self.assertEqual(c.legacy_flag, 0)
         self.assertEqual(c.deterministic_flag, 0)
         #
         self.assertListEqual(c.actions, ['create', 'recreate', 'alter', 'create_or_alter', 'drop'])
         self.assertFalse(c.is_sys_object())
@@ -2601,16 +2667,18 @@
         self.assertEqual(c.get_sql_for('revoke', grant_option=True),
                          "REVOKE GRANT OPTION FOR EXECUTE ON PROCEDURE ALL_LANGS FROM PUBLIC")
         # get_privileges_of()
         u = UserInfo(user_name='PUBLIC')
         p = s.get_privileges_of(u)
         if self.version == FB30:
             self.assertEqual(len(p), 115)
-        else:
+        elif self.version == FB40:
             self.assertEqual(len(p), 119)
+        else: # FB5
+            self.assertEqual(len(p), 515)
         with self.assertRaises(ValueError) as cm:
             p = s.get_privileges_of('PUBLIC')
         self.assertTupleEqual(cm.exception.args,
                               ("Argument user_type required",))
         #
     def test_24_PrivilegeExtended(self):
         s = Schema()
@@ -3280,16 +3348,18 @@
         self.assertFalse(c.is_sys_object())
         self.assertListEqual(c.actions,
                              ['create', 'recreate', 'create_or_alter', 'alter', 'drop', 'comment'])
         self.assertEqual(c.get_quoted_name(), 'TEST')
         self.assertEqual(c.owner_name, 'SYSDBA')
         if self.version == FB30:
             self.assertEqual(c.security_class, 'SQL$575')
-        else:
+        elif self.version == FB40:
             self.assertEqual(c.security_class, 'SQL$622')
+        else: # FB5
+            self.assertEqual(c.security_class, 'SQL$635')
         self.assertEqual(c.header, """BEGIN
   PROCEDURE P1(I INT) RETURNS (O INT); -- public procedure
   FUNCTION F(X INT) RETURNS INT;
 END""")
         self.assertEqual(c.body, """BEGIN
   FUNCTION F1(I INT) RETURNS INT; -- private function
```

### Comparing `firebird-lib-1.3.0/test/test_trace.py` & `firebird-lib-1.4.0/test/test_trace.py`

 * *Files identical despite different names*

