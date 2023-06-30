# Comparing `tmp/pycsbinarywriter-0.1.0.tar.gz` & `tmp/pycsbinarywriter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsbinarywriter-0.1.0.tar", max compression
+gzip compressed data, was "pycsbinarywriter-0.1.1.tar", max compression
```

## Comparing `pycsbinarywriter-0.1.0.tar` & `pycsbinarywriter-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1072 2022-06-15 23:10:16.533160 pycsbinarywriter-0.1.0/LICENSE
--rw-r--r--   0        0        0      721 2023-06-23 19:07:53.543053 pycsbinarywriter-0.1.0/README.md
--rw-r--r--   0        0        0       48 2023-06-23 21:58:59.304345 pycsbinarywriter-0.1.0/pycsbinarywriter/__init__.py
--rw-r--r--   0        0        0      152 2023-06-23 21:58:22.228527 pycsbinarywriter-0.1.0/pycsbinarywriter/consts.py
--rw-r--r--   0        0        0     2895 2023-06-23 21:54:32.701665 pycsbinarywriter-0.1.0/pycsbinarywriter/csharpserializable.py
--rw-r--r--   0        0        0      106 2022-06-15 22:52:03.367104 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/__init__.py
--rw-r--r--   0        0        0     2093 2023-06-23 19:45:47.670489 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/cstype.py
--rw-r--r--   0        0        0     3917 2023-06-23 21:53:32.829965 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/decimal.py
--rw-r--r--   0        0        0     2489 2023-06-23 21:43:21.333176 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/seven_bit_int.py
--rw-r--r--   0        0        0     1615 2023-06-23 21:58:22.152527 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/simple.py
--rw-r--r--   0        0        0     4412 2023-06-23 21:43:11.093234 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/strings.py
--rw-r--r--   0        0        0      148 2021-01-26 00:59:15.550467 pycsbinarywriter-0.1.0/pycsbinarywriter/test/__init__.py
--rw-r--r--   0        0        0     5411 2023-06-23 21:58:22.224527 pycsbinarywriter-0.1.0/pycsbinarywriter/test/simple.py
--rw-r--r--   0        0        0     1565 2022-06-15 22:58:01.038200 pycsbinarywriter-0.1.0/pycsbinarywriter/test/strings.py
--rw-r--r--   0        0        0      800 2023-06-23 19:36:17.833631 pycsbinarywriter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 pycsbinarywriter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-15 23:10:16.533160 pycsbinarywriter-0.1.1/LICENSE
+-rw-r--r--   0        0        0      721 2023-06-23 19:07:53.543053 pycsbinarywriter-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2023-06-23 21:58:59.304345 pycsbinarywriter-0.1.1/pycsbinarywriter/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-23 21:58:22.228527 pycsbinarywriter-0.1.1/pycsbinarywriter/consts.py
+-rw-r--r--   0        0        0     2895 2023-06-23 21:54:32.701665 pycsbinarywriter-0.1.1/pycsbinarywriter/csharpserializable.py
+-rw-r--r--   0        0        0      106 2022-06-15 22:52:03.367104 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-23 19:45:47.670489 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/cstype.py
+-rw-r--r--   0        0        0     3917 2023-06-23 21:53:32.829965 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/decimal.py
+-rw-r--r--   0        0        0     2396 2023-06-30 09:55:32.199290 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/seven_bit_int.py
+-rw-r--r--   0        0        0     1615 2023-06-23 21:58:22.152527 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/simple.py
+-rw-r--r--   0        0        0     4412 2023-06-23 21:43:11.093234 pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/strings.py
+-rw-r--r--   0        0        0      199 2023-06-30 10:02:19.849602 pycsbinarywriter-0.1.1/pycsbinarywriter/test/__init__.py
+-rw-r--r--   0        0        0      612 2023-06-30 10:20:36.254326 pycsbinarywriter-0.1.1/pycsbinarywriter/test/int7_regressions.py
+-rw-r--r--   0        0        0     5411 2023-06-30 09:47:11.645829 pycsbinarywriter-0.1.1/pycsbinarywriter/test/simple.py
+-rw-r--r--   0        0        0     1565 2022-06-15 22:58:01.038200 pycsbinarywriter-0.1.1/pycsbinarywriter/test/strings.py
+-rw-r--r--   0        0        0      800 2023-06-30 10:22:40.849828 pycsbinarywriter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 pycsbinarywriter-0.1.1/PKG-INFO
```

### Comparing `pycsbinarywriter-0.1.0/LICENSE` & `pycsbinarywriter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/README.md` & `pycsbinarywriter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/csharpserializable.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/csharpserializable.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/cstype.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/cstype.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/decimal.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/decimal.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/seven_bit_int.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/seven_bit_int.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 
     def unpack(self, data: bytes, start: int = 0) -> Optional[int]:
         o = 0
         shf = 0
         self.bytesRead = 0
         for i in range(5):
             b = ord(data[start+i:start+i+1])
-            # print(b, hex(b)[2:].zfill(2), bin(b)[2:].zfill(8), 'END' if (b & 128) == 0 else 'CONT')
             self.bytesRead += 1
             o |= (b & 127) << shf
             shf += 7
             if not (b & 128):
                 return o
         raise Exception('Bad 7bit (ran out of bytes)')
 
     def pack(self, value: int) -> bytes:
         o = b''
         while value >= 0x80:
-            o += bytes([value | 0x80])
+            o += bytes([(value | 0x80) & 0xFF])
             value >>= 7
         return o + bytes([value])
 
     def calcsize(self) -> int:
         return -1
 
     def unpackFrom(self, f: BinaryIO) -> Optional[int]:
```

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/simple.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/simple.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/strings.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/cstypes/strings.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/test/simple.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/test/simple.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pycsbinarywriter/test/strings.py` & `pycsbinarywriter-0.1.1/pycsbinarywriter/test/strings.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.1.0/pyproject.toml` & `pycsbinarywriter-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycsbinarywriter"
-version = "0.1.0"
+version = "0.1.1"
 description = "Helpers for parsing and writing binary data created by dotnet System.IO.BinaryWriters."
 authors = ["Rob Nelson <nexisentertainment@gmail.com>"]
 license = "MIT"
 readme="README.md"
 repository="https://gitlab.com/N3X15/pycsbinarywriter"
 
 [tool.poetry.dependencies]
```

### Comparing `pycsbinarywriter-0.1.0/PKG-INFO` & `pycsbinarywriter-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycsbinarywriter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Helpers for parsing and writing binary data created by dotnet System.IO.BinaryWriters.
 Home-page: https://gitlab.com/N3X15/pycsbinarywriter
 License: MIT
 Author: Rob Nelson
 Author-email: nexisentertainment@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

