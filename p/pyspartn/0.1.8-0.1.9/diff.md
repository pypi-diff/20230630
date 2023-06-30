# Comparing `tmp/pyspartn-0.1.8.tar.gz` & `tmp/pyspartn-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.1.8.tar", last modified: Wed Jun 28 06:43:15 2023, max compression
+gzip compressed data, was "pyspartn-0.1.9.tar", last modified: Fri Jun 30 09:15:01 2023, max compression
```

## Comparing `pyspartn-0.1.8.tar` & `pyspartn-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-28 06:43:15.340652 pyspartn-0.1.8/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.8/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    16543 2023-06-28 06:43:15.340447 pyspartn-0.1.8/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    13464 2023-06-28 06:39:26.000000 pyspartn-0.1.8/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2445 2023-06-28 06:39:26.000000 pyspartn-0.1.8/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-28 06:43:15.340717 pyspartn-0.1.8/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-28 06:43:15.335939 pyspartn-0.1.8/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-28 06:43:15.338664 pyspartn-0.1.8/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2023-06-06 06:30:11.000000 pyspartn-0.1.8/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2023-06-28 06:39:26.000000 pyspartn-0.1.8/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.8/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2023-06-12 06:49:18.000000 pyspartn-0.1.8/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     6991 2023-06-28 06:39:26.000000 pyspartn-0.1.8/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    17920 2023-06-28 06:39:26.000000 pyspartn-0.1.8/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)     9670 2023-06-28 06:39:26.000000 pyspartn-0.1.8/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.8/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.8/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    18755 2023-06-06 06:30:11.000000 pyspartn-0.1.8/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-28 06:43:15.339513 pyspartn-0.1.8/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    16543 2023-06-28 06:43:15.000000 pyspartn-0.1.8/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2023-06-28 06:43:15.000000 pyspartn-0.1.8/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-28 06:43:15.000000 pyspartn-0.1.8/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2023-06-28 06:43:15.000000 pyspartn-0.1.8/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2023-06-28 06:43:15.000000 pyspartn-0.1.8/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-28 06:43:15.340007 pyspartn-0.1.8/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.8/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     5882 2023-06-28 06:39:26.000000 pyspartn-0.1.8/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)    30348 2023-06-28 06:39:26.000000 pyspartn-0.1.8/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-30 09:15:01.896412 pyspartn-0.1.9/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.1.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2023-03-28 07:19:43.000000 pyspartn-0.1.9/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    16543 2023-06-30 09:15:01.896239 pyspartn-0.1.9/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    13464 2023-06-28 06:39:26.000000 pyspartn-0.1.9/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2445 2023-06-30 09:14:40.000000 pyspartn-0.1.9/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-30 09:15:01.896483 pyspartn-0.1.9/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-30 09:15:01.891698 pyspartn-0.1.9/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-30 09:15:01.894341 pyspartn-0.1.9/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2023-06-06 06:30:11.000000 pyspartn-0.1.9/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2023-06-30 09:14:40.000000 pyspartn-0.1.9/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.1.9/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2441 2023-06-12 06:49:18.000000 pyspartn-0.1.9/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     7586 2023-06-30 09:14:40.000000 pyspartn-0.1.9/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    18304 2023-06-30 09:14:40.000000 pyspartn-0.1.9/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)     9670 2023-06-28 06:39:26.000000 pyspartn-0.1.9/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.1.9/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     8642 2023-04-13 07:54:16.000000 pyspartn-0.1.9/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    18755 2023-06-06 06:30:11.000000 pyspartn-0.1.9/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-30 09:15:01.895470 pyspartn-0.1.9/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    16543 2023-06-30 09:15:01.000000 pyspartn-0.1.9/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2023-06-30 09:15:01.000000 pyspartn-0.1.9/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-30 09:15:01.000000 pyspartn-0.1.9/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2023-06-30 09:15:01.000000 pyspartn-0.1.9/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2023-06-30 09:15:01.000000 pyspartn-0.1.9/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-30 09:15:01.895964 pyspartn-0.1.9/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.1.9/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     6138 2023-06-30 09:14:40.000000 pyspartn-0.1.9/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)    30376 2023-06-30 09:14:40.000000 pyspartn-0.1.9/tests/test_stream.py
```

### Comparing `pyspartn-0.1.8/LICENSE` & `pyspartn-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/PKG-INFO` & `pyspartn-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
```

### Comparing `pyspartn-0.1.8/README.md` & `pyspartn-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/pyproject.toml` & `pyspartn-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "SPARTN protocol parser"
-version = "0.1.8"
+version = "0.1.9"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: MacOS X",
```

### Comparing `pyspartn-0.1.8/src/pyspartn/__init__.py` & `pyspartn-0.1.9/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn/exceptions.py` & `pyspartn-0.1.9/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn/socket_stream.py` & `pyspartn-0.1.9/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn/spartnhelpers.py` & `pyspartn-0.1.9/src/pyspartn/spartnhelpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,26 +208,31 @@
     return "b'{}'".format("".join(f"\\x{b:02x}" for b in val))
 
 
 def convert_timetag(timetag16: int, basedate: datetime = datetime.now()) -> int:
     """
     Convert 16-bit timetag to 32-bit format.
 
-    32-bit timetag format represents total seconds since TIMEBASE (2010-01-01).
-    16-bit timetag format represents seconds past nearest half day date. It
-    requires knowledge of the nearest half day date to convert unambiguously to
-    a 32-bit timetag equlvalent.
-
-    e.g. if nearest half day date is "2023-06-27 12:00:00", a timetag16
-    of 32580 represents "2023-06-27 00:00:00" + 12*3600 + 32580,
-    or "2023-06-20 21:03:00"
-    ("2023-06-20 21:03:00" - "2010-01-01 00:00:00") = 425595780 seconds
+    32-bit timetag represents total seconds since TIMEBASE (2010-01-01 00:00:00).
+
+    16-bit timetag represents seconds past 'base date' (the datetime the SPARTN
+    message was originally sent) to the nearest half-day. It requires knowledge
+    of this base date to convert unambiguously to a 32-bit timetag equlvalent, e.g.
+
+    If base date to nearest half day was "2023-06-27 12:00:00", a timetag16 of
+    32580 represents a datetime of:
+
+    (2023-06-27 00:00:00 + 12 hours + 32580 seconds) = 2023-06-27 21:03:00"
+
+    To convert to 32-bit timetage, calculate number of seconds since TIMEBASE:
+
+    (2023-06-27 21:03:00 - 2010-01-01 00:00:00) = 425595780 seconds
 
     :param int timetag16: 16-bit gnssTimeTag
-    :param int basedate: date to nearest half day (if none, will use today's date)
+    :param datetime basedate: original processing datetime to nearest half day
     :return: 32-bit gnssTimeTag
     :rtype: int
     """
 
     base16 = datetime(basedate.year, basedate.month, basedate.day, 0, 0, 0)
     secs = timetag16
     if basedate.hour >= 12:
@@ -244,7 +249,24 @@
     :param str datafield: datafield e.g. 'SF054'
     :return: datafield description e.g. "Ionosphere equation type"
     :rtype: str
     """
 
     (_, _, desc) = SPARTN_DATA_FIELDS[datafield[0:5]]
     return desc
+
+
+def enc2float(value: int, res: float, rngmin: float) -> float:
+    """
+    Convert encoded floating point value to float.
+
+    SPARTN protocol stores floating point numbers in
+    encoded integer format.
+
+    :param int value: encoded value
+    :param float res: resolution
+    :param float rngmin: minimum range value
+    :return: floating point value
+    :rtype: float
+    """
+
+    return (value * res) + rngmin
```

### Comparing `pyspartn-0.1.8/src/pyspartn/spartnmessage.py` & `pyspartn-0.1.9/src/pyspartn/spartnmessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,14 +153,20 @@
         if self._validate & VALCRC:
             if not valid_crc(core, self.crc, self.crcType):
                 raise SPARTNMessageError(f"Invalid CRC {self.crc}")
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
 
+        # ***********************************************************************************
+        # TODO temporary override of decode flag for message types that cannot yet be decoded
+        if self.msgType in (0, 3, 4, 120) and self._decode is True:
+            self._decode = False
+        # ***********************************************************************************
+
         # decrypt payload if encrypted
         if self.eaf and self._decode:
             iv = self._get_iv()
             self._payload = decrypt(payload, self._key, iv)
         else:
             self._payload = payload
```

### Comparing `pyspartn-0.1.8/src/pyspartn/spartnreader.py` & `pyspartn-0.1.9/src/pyspartn/spartnreader.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn/spartntypes_core.py` & `pyspartn-0.1.9/src/pyspartn/spartntypes_core.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn/spartntypes_get.py` & `pyspartn-0.1.9/src/pyspartn/spartntypes_get.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.1.9/src/pyspartn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.1.8
+Version: 0.1.9
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
```

### Comparing `pyspartn-0.1.8/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.1.9/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/tests/test_socket.py` & `pyspartn-0.1.9/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.1.8/tests/test_static.py` & `pyspartn-0.1.9/tests/test_static.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 *** NB: must be saved in UTF-8 format ***
 
 @author: semuadmin
 """
 
 import os
 import unittest
-from datetime import datetime, timedelta
+from datetime import datetime
 
 from pyspartn.spartnhelpers import (
     att2name,
     att2idx,
     bitsval,
     valid_crc,
     escapeall,
     encrypt,
     decrypt,
     convert_timetag,
     numbitsset,
     datadesc,
+    enc2float,
 )
 from pyspartn.spartntypes_core import TIMEBASE
 from pyspartn.exceptions import SPARTNMessageError
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
@@ -168,11 +169,17 @@
 
     def testdatadesc(self):  # test datadesc
         res = datadesc("SF054")
         self.assertEqual(res, "Ionosphere equation type")
         res = datadesc("SF043_01")
         self.assertEqual(res, "Area average vertical hydrostatic delay")
 
+    def testenc2float(self):  # test enc2float
+        res = enc2float(1332, 0.1, -90)
+        self.assertAlmostEqual(res, 43.20000000000002, 6)
+        res = enc2float(2033, 0.1, -180)
+        self.assertAlmostEqual(res, 23.30000000000001, 6)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `pyspartn-0.1.8/tests/test_stream.py` & `pyspartn-0.1.9/tests/test_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Return captured output and restore stdout.
         """
 
         sys.stdout = self._saved_stdout
         return self._strout.getvalue().strip()
 
     def testSerialize(self):  # test serialize()
-        msg1 = SPARTNReader.parse(self.spartntransport)
+        msg1 = SPARTNReader.parse(self.spartntransport, decode=False)
         msg2 = SPARTNMessage(transport=self.spartntransport)
         res = msg1.serialize()
         self.assertEqual(res, self.spartntransport)
         res1 = msg2.serialize()
         self.assertEqual(res1, self.spartntransport)
 
     def testsetattr(self):  # test immutability
@@ -68,15 +68,15 @@
         )
         with self.assertRaisesRegex(SPARTNMessageError, EXPECTED_ERROR):
             msg = SPARTNReader.parse(self.spartntransport)
             msg.eaf = 0
 
     def testrepr(self):  # test repr, check eval recreates original object
         EXPECTED_RESULT = "SPARTNMessage(transport=b's\\x00\\x12\\xe2\\x00|\\x10[\\x12H\\xf5\\t\\xa0\\xb4+\\x99\\x02\\x15\\xe2\\x05\\x85\\xb7\\x83\\xc5\\xfd\\x0f\\xfe\\xdf\\x18\\xbe\\x7fv \\xc3`\\x82\\x98\\x10\\x07\\xdc\\xeb\\x82\\x7f\\xcf\\xf8\\x9e\\xa3ta\\xad')"
-        msg1 = SPARTNReader.parse(self.spartntransport)
+        msg1 = SPARTNReader.parse(self.spartntransport, decode=False)
         self.assertEqual(repr(msg1), EXPECTED_RESULT)
         msg2 = eval(repr(msg1))
         self.assertEqual(str(msg1), str(msg2))
 
     def testpayload(self):  # test payload
         EXPECTED_RESULT = b"\xf5\x09\xa0\xb4\x2b\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7f\x76\x20\xc3\x60\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3"
         msg = SPARTNReader.parse(self.spartntransport)
```

