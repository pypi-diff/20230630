# Comparing `tmp/xcyl-0.0.8.tar.gz` & `tmp/xcyl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcyl-0.0.8.tar", last modified: Mon Dec  5 17:57:55 2022, max compression
+gzip compressed data, was "xcyl-0.0.9.tar", last modified: Wed Mar  1 02:57:33 2023, max compression
```

## Comparing `xcyl-0.0.8.tar` & `xcyl-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:57:55.933609 xcyl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-05 17:57:52.000000 xcyl-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-05 17:57:55.933609 xcyl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-05 17:57:52.000000 xcyl-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 17:57:55.933609 xcyl-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2022-12-05 17:57:52.000000 xcyl-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:57:55.933609 xcyl-0.0.8/xcyl/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8398 2022-12-05 17:57:52.000000 xcyl-0.0.8/xcyl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:57:55.933609 xcyl-0.0.8/xcyl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2022-12-05 17:57:55.000000 xcyl-0.0.8/xcyl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-05 17:57:55.000000 xcyl-0.0.8/xcyl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:57:55.000000 xcyl-0.0.8/xcyl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-05 17:57:55.000000 xcyl-0.0.8/xcyl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-05 17:57:55.000000 xcyl-0.0.8/xcyl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:57:33.292562 xcyl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-01 02:57:29.000000 xcyl-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-01 02:57:33.292562 xcyl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-01 02:57:29.000000 xcyl-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 02:57:33.292562 xcyl-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-03-01 02:57:29.000000 xcyl-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:57:33.292562 xcyl-0.0.9/xcyl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8930 2023-03-01 02:57:29.000000 xcyl-0.0.9/xcyl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:57:33.292562 xcyl-0.0.9/xcyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-01 02:57:33.000000 xcyl-0.0.9/xcyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-01 02:57:33.000000 xcyl-0.0.9/xcyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 02:57:33.000000 xcyl-0.0.9/xcyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-01 02:57:33.000000 xcyl-0.0.9/xcyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-01 02:57:33.000000 xcyl-0.0.9/xcyl.egg-info/top_level.txt
```

### Comparing `xcyl-0.0.8/LICENSE` & `xcyl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xcyl-0.0.8/setup.py` & `xcyl-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `xcyl-0.0.8/xcyl/__init__.py` & `xcyl-0.0.9/xcyl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,12 +318,36 @@
 
 	def __getitem__(self, item):
 		return self.load_table(item)
 
 	def __setitem__(self, key, value):
 		self.add_frame(key, value)
 
+	def drop_table(self, table_name, backup=True):
+		just_enter = False
+		if self.exists is None:
+			just_enter = True
+			self.just_enter()
+
+		if table_name in self.table_names():
+			if backup:
+				self[table_name].to_csv(".backup_{0}.csv".format(table_name))
+
+			if just_enter:
+				current_cursor = self.connection.cursor()
+				current_cursor.execute("DROP table IF EXISTS {0};".format({0}))
+				current_cursor = None
+			else:
+				try:
+					self.dataframes.pop(table_name)
+				except: pass
+
+		if just_enter:
+			self.exit()
+
+		return
+
 	def to_xcylobj(self):
 		output = xcylobj("temp.xlsx")
 		for key, value in self.dataframes.items():
 			output[key] = value
 		return output
```

