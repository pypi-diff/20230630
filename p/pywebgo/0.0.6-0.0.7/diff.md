# Comparing `tmp/pywebgo-0.0.6.tar.gz` & `tmp/pywebgo-0.0.7.tar.gz`

## Comparing `pywebgo-0.0.6.tar` & `pywebgo-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.6/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.6/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.6/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.7/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.7/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.7/PKG-INFO
```

### Comparing `pywebgo-0.0.6/.github/workflows/python-publish.yml` & `pywebgo-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/src/pywebgo/controller.py` & `pywebgo-0.0.7/src/pywebgo/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,24 +24,25 @@
     - :class:`bool` teardown --> closes the browser after execution if true
     - :class:`float` wait --> time delay for executing each action
     - :class:`ElementsHandler` elem_handler --> instance of ElementsHandler class to manage elements
     - :class:`DataHandler` data_handler --> instance of DataHandler class to manage data associated with the elements
     """
 
     def __init__(self, urls: list, teardown: bool = True, wait: float = 0,
-                 options: list = None, retry_attempts: int = 1):
+                 options: list = None, retry_attempts: int = 1, detach: bool = False):
         """
         Initialize a new instance of the WebController class.
 
         :param urls: non-linked web pages to traverse through
         :param teardown: closes the browser after execution if true
         :param wait: time delay for executing each action
         """
         chrome_options = webdriver.ChromeOptions()
         chrome_options.add_experimental_option("excludeSwitches", ["disable-popup-blocking"])
+        chrome_options.add_experimental_option("detach", detach)
         if options:
             for option in options:
                 chrome_options.add_argument(option)
 
         super(WebController, self).__init__(chrome_options=chrome_options)
 
         # ---- Private Variables ----- #
```

### Comparing `pywebgo-0.0.6/src/pywebgo/data.py` & `pywebgo-0.0.7/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/src/pywebgo/elements.py` & `pywebgo-0.0.7/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/src/pywebgo/utils.py` & `pywebgo-0.0.7/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/.gitignore` & `pywebgo-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/LICENSE` & `pywebgo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.6/pyproject.toml` & `pywebgo-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.6/PKG-INFO` & `pywebgo-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.6
+Version: 0.0.7
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

