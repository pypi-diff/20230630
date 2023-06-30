# Comparing `tmp/parsagon-0.7.3.tar.gz` & `tmp/parsagon-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.3.tar", last modified: Thu Jun 29 19:42:29 2023, max compression
+gzip compressed data, was "parsagon-0.7.4.tar", last modified: Fri Jun 30 06:02:48 2023, max compression
```

## Comparing `parsagon-0.7.3.tar` & `parsagon-0.7.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.775278 parsagon-0.7.3/
--rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-29 19:42:29.774702 parsagon-0.7.3/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.3/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1026 2023-06-29 19:41:23.000000 parsagon-0.7.3/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-29 19:42:29.775469 parsagon-0.7.3/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.759590 parsagon-0.7.3/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.3/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.766466 parsagon-0.7.3/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     4355 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.3/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      879 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    10517 2023-06-27 10:04:55.000000 parsagon-0.7.3/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     6885 2023-06-29 19:39:03.000000 parsagon-0.7.3/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1570 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.773783 parsagon-0.7.3/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.3/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.769867 parsagon-0.7.3/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      606 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      250 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.120802 parsagon-0.7.4/
+-rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-30 06:02:48.120453 parsagon-0.7.4/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.4/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1026 2023-06-30 06:02:23.000000 parsagon-0.7.4/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-30 06:02:48.120917 parsagon-0.7.4/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.110165 parsagon-0.7.4/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.4/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.114695 parsagon-0.7.4/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4355 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.4/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-06-30 00:46:35.000000 parsagon-0.7.4/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    11215 2023-06-30 05:36:14.000000 parsagon-0.7.4/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     7003 2023-06-30 05:58:11.000000 parsagon-0.7.4/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1570 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.119802 parsagon-0.7.4/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.4/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-06-29 05:25:58.000000 parsagon-0.7.4/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-30 06:02:48.117154 parsagon-0.7.4/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      606 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      250 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-30 06:02:48.000000 parsagon-0.7.4/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.3/PKG-INFO` & `parsagon-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.3
+Version: 0.7.4
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.3/README.md` & `parsagon-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/pyproject.toml` & `parsagon-0.7.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.3"
+version = "0.7.4"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.7.3/src/parsagon/api.py` & `parsagon-0.7.4/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/src/parsagon/custom_function.py` & `parsagon-0.7.4/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/src/parsagon/exceptions.py` & `parsagon-0.7.4/src/parsagon/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 class ParsagonException(Exception):
     """Base class for all exceptions in Parsagon. The CLI will use the to_string method to print the exception to the user."""
 
     def to_string(self, verbose):
         return str(self)
 
-    def __str__(self):
-        return self.to_string(True)
-
 
 class APIException(ParsagonException):
     def __init__(self, value, status_code):
         super().__init__(value)
         self.value = value
         self.status_code = status_code
```

### Comparing `parsagon-0.7.3/src/parsagon/executor.py` & `parsagon-0.7.4/src/parsagon/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.select import Select
 
 from parsagon.api import get_interaction_element_id, scrape_page
 from parsagon.custom_function import CustomFunction
+from parsagon.exceptions import ParsagonException
 
 logger = logging.getLogger(__name__)
 
 
 # A dictionary of custom function names to their descriptions for the user
 custom_functions_to_descriptions = {
     "scrape_data": "scrape data from the page",
@@ -121,14 +122,16 @@
 
         return lxml.html.tostring(root).decode()
 
     def get_elem_by_description(self, elem_type, description):
         logger.info(f'Looking for {elem_type.lower()}: "{description}"')
         visible_html = self.get_visible_html()
         elem_id = get_interaction_element_id(visible_html, elem_type, description)
+        if elem_id is None:
+            raise ParsagonException(f'Could not find an element matching "{description}". Perhaps try rephrasing your prompt.')
         return elem_id
 
     def _get_elem(self, elem_id):
         """
         Gets a selenium element by Parsagon ID (psgn-id).
         """
         assert elem_id is not None
@@ -275,14 +278,18 @@
         """
         self.driver.switch_to.window(window_id)
         logger.info("Scraping data...")
         html = self.get_scrape_html()
         result = scrape_page(html, schema)
         scraped_data = result["data"]
         nodes = result["nodes"]
+        if not scraped_data and not nodes:
+            raise ParsagonException(f"Parsagon could not find any data on the page that would fit the format {schema}. Perhaps try rephrasing your prompt.")
+        elif not nodes:
+            raise ParsagonException(f"Parsagon found the following data on the page for the format {schema}:\n\n{scraped_data}\n\nHowever, it could not find a plausible program to scrape this data. If the data above is incorrect, perhaps try rephrasing your prompt.")
         logger.info(f"Scraped data:\n{scraped_data}")
         custom_function = CustomFunction(
             "scrape_data",
             arguments={
                 "schema": schema,
             },
             examples=[
```

### Comparing `parsagon-0.7.3/src/parsagon/main.py` & `parsagon-0.7.4/src/parsagon/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,28 +125,29 @@
     if task:
         logger.info("Launched with task description:\n%s", task)
     else:
         task = input("Type what you want to do: ")
 
     logger.info("Analyzing task description...")
     program_sketches = get_program_sketches(task)
+    logger.info("Created a program based on task description. Now demonstrating what the program does:\n")
 
     full_program = program_sketches["full"]
     abridged_program = program_sketches["abridged"]
     logger.debug("Program:\n%s", abridged_program)
-    abridged_program += "\n\noutput = func()\nprint(f'Program finished and returned a value of:\\n{output}')\n"  # Make the program runnable
+    abridged_program += "\n\noutput = func()\nprint(f'Program finished and returned a value of:\\n{output}\\n')\n"  # Make the program runnable
 
     # Execute the abridged program to gather examples
     executor = Executor(headless=headless)
     executor.execute(abridged_program)
 
     # The user must select a name
     while True:
         if not program_name:
-            program_name = input("Name this program, or press enter without typing a name to DISCARD: ")
+            program_name = input("Name this program to save, or press enter without typing a name to DISCARD: ")
         if program_name:
             logger.info(f"Saving program as {program_name}")
             try:
                 pipeline = create_pipeline(program_name, task, full_program)
             except APIException as e:
                 if isinstance(e.value, list) and "Program with name already exists" in e.value:
                     logger.info("A program with this name already exists. Please choose another name.")
```

### Comparing `parsagon-0.7.3/src/parsagon/settings.py` & `parsagon-0.7.4/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/src/parsagon/tests/api_mocks.py` & `parsagon-0.7.4/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.7.4/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.3/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.4/src/parsagon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.3
+Version: 0.7.4
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.7.3/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.7.4/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

