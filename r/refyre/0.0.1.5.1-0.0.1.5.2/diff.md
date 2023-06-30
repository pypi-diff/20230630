# Comparing `tmp/refyre-0.0.1.5.1.tar.gz` & `tmp/refyre-0.0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refyre-0.0.1.5.1.tar", max compression
+gzip compressed data, was "refyre-0.0.1.5.2.tar", max compression
```

## Comparing `refyre-0.0.1.5.1.tar` & `refyre-0.0.1.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    10130 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/README.md
--rw-r--r--   0        0        0      924 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0    23582 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/Refyre.py
--rw-r--r--   0        0        0      135 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cli.py
--rw-r--r--   0        0        0     3731 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Association.py
--rw-r--r--   0        0        0     3813 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Broadcast.py
--rw-r--r--   0        0        0     2281 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Cache.py
--rw-r--r--   0        0        0    20658 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Cluster.py
--rw-r--r--   0        0        0      718 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/ClusterIterator.py
--rw-r--r--   0        0        0      237 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/cogs/VariableAction.py
--rw-r--r--   0        0        0     2767 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/cogs/VariableParser.py
--rw-r--r--   0        0        0       23 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/config/__init__.py
--rw-r--r--   0        0        0      355 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/config/log.py
--rw-r--r--   0        0        0      499 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/AliasManager.py
--rw-r--r--   0        0        0      363 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/CodeManager.py
--rw-r--r--   0        0        0     3543 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/RecipePreprocessor.py
--rw-r--r--   0        0        0      126 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/__init__.py
--rw-r--r--   0        0        0     1597 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/DataStack.py
--rw-r--r--   0        0        0      347 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/TorchStack.py
--rw-r--r--   0        0        0       34 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/__init__.py
--rw-r--r--   0        0        0      802 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/FileGraph.py
--rw-r--r--   0        0        0     2051 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/FileGraphNode.py
--rw-r--r--   0        0        0       73 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/__init__.py
--rw-r--r--   0        0        0     2375 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/reader/ExpressionGenerator.py
--rw-r--r--   0        0        0     6066 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/reader/Lexer.py
--rw-r--r--   0        0        0     3287 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/Parser.py
--rw-r--r--   0        0        0     3492 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/PatternGenerator.py
--rw-r--r--   0        0        0      221 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/__init__.py
--rw-r--r--   0        0        0      799 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/cogs/LexerToken.py
--rw-r--r--   0        0        0      618 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/cogs/lexer_utils.py
--rw-r--r--   0        0        0      153 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/__init__.py
--rw-r--r--   0        0        0      667 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/clone.py
--rw-r--r--   0        0        0      453 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/optional_imports.py
--rw-r--r--   0        0        0      903 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/regex.py
--rw-r--r--   0        0        0    10991 1970-01-01 00:00:00.000000 refyre-0.0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10130 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/README.md
+-rw-r--r--   0        0        0      924 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    23582 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/Refyre.py
+-rw-r--r--   0        0        0      135 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cli.py
+-rw-r--r--   0        0        0     3731 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/Association.py
+-rw-r--r--   0        0        0     3813 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/Broadcast.py
+-rw-r--r--   0        0        0     2281 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/Cache.py
+-rw-r--r--   0        0        0    20658 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/Cluster.py
+-rw-r--r--   0        0        0      718 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/ClusterIterator.py
+-rw-r--r--   0        0        0      237 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/cogs/VariableAction.py
+-rw-r--r--   0        0        0     2767 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/cluster/cogs/VariableParser.py
+-rw-r--r--   0        0        0       23 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/config/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/config/log.py
+-rw-r--r--   0        0        0      499 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/core/AliasManager.py
+-rw-r--r--   0        0        0      363 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/core/CodeManager.py
+-rw-r--r--   0        0        0     3356 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/core/RecipePreprocessor.py
+-rw-r--r--   0        0        0      126 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/core/__init__.py
+-rw-r--r--   0        0        0     1597 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/datastack/DataStack.py
+-rw-r--r--   0        0        0      347 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/datastack/TorchStack.py
+-rw-r--r--   0        0        0       34 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/datastack/__init__.py
+-rw-r--r--   0        0        0      802 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/graph/FileGraph.py
+-rw-r--r--   0        0        0     2051 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/graph/FileGraphNode.py
+-rw-r--r--   0        0        0       73 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/graph/__init__.py
+-rw-r--r--   0        0        0     2375 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/ExpressionGenerator.py
+-rw-r--r--   0        0        0     6066 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/Lexer.py
+-rw-r--r--   0        0        0     3287 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/Parser.py
+-rw-r--r--   0        0        0     3492 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/PatternGenerator.py
+-rw-r--r--   0        0        0      221 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/cogs/LexerToken.py
+-rw-r--r--   0        0        0      618 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/reader/cogs/lexer_utils.py
+-rw-r--r--   0        0        0      153 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/utils/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/utils/clone.py
+-rw-r--r--   0        0        0      453 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/utils/optional_imports.py
+-rw-r--r--   0        0        0      903 2023-06-30 04:08:28.579941 refyre-0.0.1.5.2/refyre/utils/regex.py
+-rw-r--r--   0        0        0    10991 1970-01-01 00:00:00.000000 refyre-0.0.1.5.2/PKG-INFO
```

### Comparing `refyre-0.0.1.5.1/README.md` & `refyre-0.0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/pyproject.toml` & `refyre-0.0.1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refyre"
-version = "0.0.1.5.1"
+version = "0.0.1.5.2"
 description = "Filesystem dominance is all you need."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/refyre"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
```

### Comparing `refyre-0.0.1.5.1/refyre/Refyre.py` & `refyre-0.0.1.5.2/refyre/Refyre.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cli.py` & `refyre-0.0.1.5.2/refyre/cli.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/Association.py` & `refyre-0.0.1.5.2/refyre/cluster/Association.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/Broadcast.py` & `refyre-0.0.1.5.2/refyre/cluster/Broadcast.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/Cache.py` & `refyre-0.0.1.5.2/refyre/cluster/Cache.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/Cluster.py` & `refyre-0.0.1.5.2/refyre/cluster/Cluster.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/ClusterIterator.py` & `refyre-0.0.1.5.2/refyre/cluster/ClusterIterator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/cogs/VariableAction.py` & `refyre-0.0.1.5.2/refyre/cluster/cogs/VariableAction.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/cluster/cogs/VariableParser.py` & `refyre-0.0.1.5.2/refyre/cluster/cogs/VariableParser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/core/RecipePreprocessor.py` & `refyre-0.0.1.5.2/refyre/core/RecipePreprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 from refyre import Refyre
 from refyre.config import logger
 
 from pip._internal import main as pip_main
 import subprocess
 import shutil
 
-def create_virtualenv_and_install_requirements(venv_path, requirements_file):
-    # Create the virtual environment
-    venv_builder = venv.EnvBuilder(with_pip=True)
-    venv_builder.create(venv_path)
+def create_virtualenv_and_install_requirements(directory, requirements_file):
+    """
+    Create a virtual environment in the specified directory using venv.Builder.
+
+    Args:
+        directory (str): The directory path where the virtual environment will be created.
+    """
+    # Create the directory if it doesn't exist
+    Path(directory).mkdir(parents=True, exist_ok=True)
 
-    # Activate the virtual environment
-    activate_script = (
-        Path(venv_path) / "Scripts" / "activate" if sys.platform == "win32"
-        else Path(venv_path) / "bin" / "activate"
-    )
-    activate_cmd = f"source {activate_script} && python -m pip"
-    
-    # Install the requirements using pip within the virtual environment
-    logger.debug("installing reqs")
-    pip_install_cmd = f"{activate_cmd} install -r {requirements_file}"
-    subprocess.run(pip_install_cmd, shell=True, check=True)
+    # Set up the builder
+    builder = venv.EnvBuilder(with_pip=True)
+
+    # Create the virtual environment
+    builder.create(directory)
 
 class RecipePreprocessor:
     def __new__(self, recipe_path):
         '''
             Performs all the recipe path preprocessing, and then 
             returns the Refyre instance
             to manage.
```

### Comparing `refyre-0.0.1.5.1/refyre/datastack/DataStack.py` & `refyre-0.0.1.5.2/refyre/datastack/DataStack.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/graph/FileGraph.py` & `refyre-0.0.1.5.2/refyre/graph/FileGraph.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/graph/FileGraphNode.py` & `refyre-0.0.1.5.2/refyre/graph/FileGraphNode.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/ExpressionGenerator.py` & `refyre-0.0.1.5.2/refyre/reader/ExpressionGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/Lexer.py` & `refyre-0.0.1.5.2/refyre/reader/Lexer.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/Parser.py` & `refyre-0.0.1.5.2/refyre/reader/Parser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/PatternGenerator.py` & `refyre-0.0.1.5.2/refyre/reader/PatternGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/cogs/LexerToken.py` & `refyre-0.0.1.5.2/refyre/reader/cogs/LexerToken.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/reader/cogs/lexer_utils.py` & `refyre-0.0.1.5.2/refyre/reader/cogs/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/utils/clone.py` & `refyre-0.0.1.5.2/refyre/utils/clone.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/refyre/utils/regex.py` & `refyre-0.0.1.5.2/refyre/utils/regex.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5.1/PKG-INFO` & `refyre-0.0.1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refyre
-Version: 0.0.1.5.1
+Version: 0.0.1.5.2
 Summary: Filesystem dominance is all you need.
 Home-page: https://github.com/flockfysh/refyre
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.8
```

