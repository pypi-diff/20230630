# Comparing `tmp/pydwm1001-0.6.0.tar.gz` & `tmp/pydwm1001-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwm1001-0.6.0.tar", last modified: Fri Jun 30 00:07:25 2023, max compression
+gzip compressed data, was "pydwm1001-0.7.0.tar", last modified: Fri Jun 30 00:13:35 2023, max compression
```

## Comparing `pydwm1001-0.6.0.tar` & `pydwm1001-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.637481 pydwm1001-0.6.0/
--rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.6.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:07:25.637357 pydwm1001-0.6.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.6.0/README.md
--rw-r--r--   0 adam       (501) staff       (20)     4485 2023-06-30 00:05:33.000000 pydwm1001-0.6.0/dwm1001.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.636868 pydwm1001-0.6.0/pydwm1001.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      229 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        9 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        8 2023-06-30 00:07:25.000000 pydwm1001-0.6.0/pydwm1001.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      640 2023-06-30 00:05:33.000000 pydwm1001-0.6.0/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-30 00:07:25.637524 pydwm1001-0.6.0/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:07:25.637021 pydwm1001-0.6.0/tests/
--rw-r--r--   0 adam       (501) staff       (20)     2782 2023-06-29 00:33:31.000000 pydwm1001-0.6.0/tests/test_dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812601 pydwm1001-0.7.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1111 2023-06-21 00:05:54.000000 pydwm1001-0.7.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:13:35.812494 pydwm1001-0.7.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      103 2023-06-21 00:05:43.000000 pydwm1001-0.7.0/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     4488 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/dwm1001.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812237 pydwm1001-0.7.0/pydwm1001.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      637 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      229 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        9 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        8 2023-06-30 00:13:35.000000 pydwm1001-0.7.0/pydwm1001.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      640 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-30 00:13:35.812638 pydwm1001-0.7.0/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-30 00:13:35.812335 pydwm1001-0.7.0/tests/
+-rw-r--r--   0 adam       (501) staff       (20)     2788 2023-06-30 00:12:46.000000 pydwm1001-0.7.0/tests/test_dwm1001.py
```

### Comparing `pydwm1001-0.6.0/LICENSE` & `pydwm1001-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwm1001-0.6.0/PKG-INFO` & `pydwm1001-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.6.0/dwm1001.py` & `pydwm1001-0.7.0/dwm1001.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @dataclass
 class TagPosition:
     x_m: float
     y_m: float
     z_m: float
     quality: int
 
-    def almost_equal(self, other: "TagPosition") -> bool:
+    def is_almost_equal(self, other: "TagPosition") -> bool:
         return (
             math.isclose(self.x_m, other.x_m)
             and math.isclose(self.y_m, other.y_m)
             and math.isclose(self.z_m, other.z_m)
             and self.quality == other.quality
         )
```

### Comparing `pydwm1001-0.6.0/pydwm1001.egg-info/PKG-INFO` & `pydwm1001-0.7.0/pydwm1001.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwm1001
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Python library for interfacing with DWM1001
 Author-email: Adam Morrissett <morrissettal2@vcu.edu>
 Project-URL: Homepage, https://github.com/the-hive-lab/pydwm1001
 Project-URL: Bug Tracker, https://github.com/the-hive-lab/pydwm1001/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydwm1001-0.6.0/pyproject.toml` & `pydwm1001-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydwm1001"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Adam Morrissett", email="morrissettal2@vcu.edu" },
 ]
 description = "A Python library for interfacing with DWM1001"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pydwm1001-0.6.0/tests/test_dwm1001.py` & `pydwm1001-0.7.0/tests/test_dwm1001.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.assertAlmostEqual(position.z_m, 7.89)
         self.assertEqual(position.quality, 42)
 
     def test_almost_equal(self) -> None:
         position1 = dwm1001.TagPosition(1.23, 4.56, 7.89, 42)
         position2 = dwm1001.TagPosition(1.23, 4.56, 7.89, 42)
 
-        self.assertTrue(position1.almost_equal(position2))
+        self.assertTrue(position1.is_almost_equal(position2))
 
 
 class TestPassiveTag(unittest.TestCase):
     def test_construction(self) -> None:
         serial_handle = MockSerial()
         dwm1001.PassiveTag(serial_handle)
 
@@ -62,15 +62,15 @@
         passive_tag = dwm1001.PassiveTag(serial_handle)
         passive_tag.start_position_reporting()
 
         tag_id, tag_position = passive_tag.wait_for_position_report()
         self.assertEqual(tag_id, "TEST1")
 
         expected_position = dwm1001.TagPosition(1.23, 4.56, 7.89, 20)
-        self.assertTrue(tag_position.almost_equal(expected_position))
+        self.assertTrue(tag_position.is_almost_equal(expected_position))
 
     def test_wait_for_position_report_short(self) -> None:
         serial_handle = MockSerial(b"POS,1,TEST1,1.23,4.56,7.89")
         passive_tag = dwm1001.PassiveTag(serial_handle)
         passive_tag.start_position_reporting()
 
         self.assertRaises(dwm1001.ParsingError, passive_tag.wait_for_position_report)
```

