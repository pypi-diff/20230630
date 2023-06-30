# Comparing `tmp/nicknames-0.1.3.tar.gz` & `tmp/nicknames-0.1.4.tar.gz`

## Comparing `nicknames-0.1.3.tar` & `nicknames-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 nicknames-0.1.3/test_package.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 nicknames-0.1.3/src/nicknames/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.3/src/nicknames/_version.py
--rw-r--r--   0        0        0    22717 2020-02-02 00:00:00.000000 nicknames-0.1.3/src/nicknames/names.csv
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.3/.gitignore
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.3/hatch_build.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nicknames-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.3/../README.md
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 nicknames-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 nicknames-0.1.4/test_package.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/_compat.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/_version.py
+-rw-r--r--   0        0        0    22788 2020-02-02 00:00:00.000000 nicknames-0.1.4/src/nicknames/names.csv
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nicknames-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 nicknames-0.1.4/hatch_build.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 nicknames-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 nicknames-0.1.4/../README.md
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nicknames-0.1.4/PKG-INFO
```

### Comparing `nicknames-0.1.3/test_package.py` & `nicknames-0.1.4/test_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import pytest
-
 from nicknames import NickNamer, default_lookup
 
 
 @pytest.fixture
 def csv_contents():
     return """
 alex,al
```

### Comparing `nicknames-0.1.3/src/nicknames/__init__.py` & `nicknames-0.1.4/src/nicknames/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import csv
-from importlib.resources import path
 from pathlib import Path
 from typing import Dict, Iterable, Set, Union
 
-from nicknames._version import __version__  # noqa: F401
+from nicknames._compat import load_resource
+from nicknames._version import __version__ as __version__
 
 _LookupTable = Dict[str, Set[str]]
 _PathLike = Union[str, Path]
 
 
 class NickNamer:
     def __init__(
@@ -131,15 +131,15 @@
     You could use this to tweak the default lookup table:
 
     >>> lookup = default_nicknames_lookup()
     >>> del lookup["alexander]
     >>> nn = NickNamer(nickname_lookup=lookup)
     >>> assert nn.nicknames_of("alexander") == set()
     """
-    with path(__package__, "names.csv") as f:
+    with load_resource(__package__, "names.csv") as f:
         return _lookup_from_csv(f)
 
 
 def _lookup_from_csv(path: _PathLike, reader_kwargs={}) -> _LookupTable:
     path = Path(path)
     with path.open("r") as f:
         lines = csv.reader(f, **reader_kwargs)
```

### Comparing `nicknames-0.1.3/src/nicknames/names.csv` & `nicknames-0.1.4/src/nicknames/names.csv`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,16 @@
 carrie,cassie
 carthaette,etta,etty
 casey,k.c.
 casper,jasper
 cassandra,sandy,cassie,sandra
 cassidy,cassie,cass
 caswell,cass
-catherine,kathy,katy,lena,kittie,kit,trina,cathy,kay,cassie
-cathleen,kathy,katy,lena,kittie,kit,trina,cathy,kay,cassie
+catherine,kathy,katy,lena,kittie,kit,trina,cathy,kay,cassie,casey
+cathleen,kathy,katy,lena,kittie,kit,trina,cathy,kay,cassie,casey
 cathy,kathy,cathleen,catherine
 cecilia,cissy,celia
 cedric,ced,rick,ricky
 celeste,lessie,celia
 celinda,linda,lynn,lindy
 charity,chat
 charles,charlie,chuck,carl,chick
@@ -448,25 +448,26 @@
 gum,monty
 gus,gussie
 gustavus,gus,gussie
 gwen,wendy
 gwendolyn,gwen,wendy
 hamilton,ham
 hannah,nan,nanny,anna
-harold,hal,harry
+harold,hal,harry,hap,haps
 harriet,hattie
-harry,harold,henry
+harrison,harry,hap,haps
+harry,harold,henry,hap,haps
 haseltine,hassie
 heather,hetty
 helen,lena,ella,ellen,ellie
 helena,eileen,lena,nell,nellie,eleanor,elaine,ellen,aileen
 helene,lena,ella,ellen,ellie
 heloise,lois,eloise,elouise
 henrietta,hank,etta,etty,retta,nettie
-henry,hank,hal,harry
+henry,hank,hal,harry,hap,haps
 hephsibah,hipsie
 hepsibah,hipsie
 herbert,bert,herb
 herman,harman,dutch
 hermione,hermie
 hester,hessy,esther,hetty
 hezekiah,hy,hez,kiah
@@ -497,15 +498,15 @@
 isaiah,zadie,zay
 isidore,izzy
 iva,ivy
 ivan,john
 jackson,jack
 jacob,jaap,jake,jay
 jacobus,jacob
-jacqueline,jackie,jack
+jacqueline,jackie,jack,jacqui
 jahoda,hody,hodie,hoda
 jakob,jake
 james,jimmy,jim,jamie,jimmie,jem
 jamie,james
 jane,janie,jessie,jean,jennie
 janet,jan,jessie
 janice,jan
```

### Comparing `nicknames-0.1.3/hatch_build.py` & `nicknames-0.1.4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.3/pyproject.toml` & `nicknames-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -36,22 +36,28 @@
 
 [tool.hatch.version]
 path = "src/nicknames/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "black",
-  "flake8",
-  "isort",
   "pytest",
+  "ruff",
 ]
 
 [tool.hatch.envs.default.scripts]
 # Run these in the repo root to get ALL python files
-flake8 = "python -m flake8 --max-line-length=88 .."
-black = "python -m black --check .."
-isort = "python -m isort --check-only --diff .."
+lint = "python -m black --check .. && python -m ruff .."
+fmt = "python -m black .. && python -m ruff --fix .."
 test = "pytest"
+test-CI = "pytest -Werror"
 sync = "python ../normalize.py && python ../sql/generate_sql.py"
 
 # Instructs hatch to call hatch_build.py during build step
 [tool.hatch.build.hooks.custom]
+
+[tool.ruff]
+select = [
+  "E",  # pyflakes
+  "F",  # pyflakes
+  "I",  # isort
+]
```

### Comparing `nicknames-0.1.3/../README.md` & `nicknames-0.1.4/../README.md`

 * *Files identical despite different names*

### Comparing `nicknames-0.1.3/PKG-INFO` & `nicknames-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: nicknames
-Version: 0.1.3
+Version: 0.1.4
 Summary: Hand-curated dataset of English given names and nicknames
 Project-URL: Homepage, https://github.com/carltonnorthern/nicknames
 Project-URL: Bug Tracker, https://github.com/carltonnorthern/nicknames/issues
 Author-email: Carlton Northern <carlton.northern@gmail.com>
+License-Expression: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

