# Comparing `tmp/velesresearch-0.0.8.tar.gz` & `tmp/velesresearch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velesresearch-0.0.8.tar", max compression
+gzip compressed data, was "velesresearch-0.0.9.tar", max compression
```

## Comparing `velesresearch-0.0.8.tar` & `velesresearch-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-13 15:18:11.932737 velesresearch-0.0.8/LICENSE
--rw-r--r--   0        0        0     1946 2023-06-13 15:18:11.932737 velesresearch-0.0.8/README.md
--rw-r--r--   0        0        0      825 2023-06-13 15:18:26.591014 velesresearch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      186 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/__init__.py
--rw-r--r--   0        0        0      794 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/options.py
--rw-r--r--   0        0        0      572 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/questiontypes.py
--rw-r--r--   0        0        0     6686 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/structure.py
--rw-r--r--   0        0        0     2330 2023-06-13 15:18:11.936737 velesresearch-0.0.8/velesresearch/tools.py
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 velesresearch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-13 23:54:29.183025 velesresearch-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1964 2023-06-13 23:54:29.183025 velesresearch-0.0.9/README.md
+-rw-r--r--   0        0        0      864 2023-06-13 23:54:41.239157 velesresearch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/__init__.py
+-rw-r--r--   0        0        0     4097 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/generator.py
+-rw-r--r--   0        0        0      794 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/options.py
+-rw-r--r--   0        0        0      572 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/questiontypes.py
+-rw-r--r--   0        0        0     6781 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/structure.py
+-rw-r--r--   0        0        0     2551 2023-06-13 23:54:29.187025 velesresearch-0.0.9/velesresearch/tools.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 velesresearch-0.0.9/PKG-INFO
```

### Comparing `velesresearch-0.0.8/LICENSE` & `velesresearch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.8/README.md` & `velesresearch-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,9 +48,9 @@
 You can install the current version of Veles with:
 ``` bash
 pip install velesresearch
 ```
 
 You can install development version (unstable) with:
 ``` bash
-pip install https://github.com/jakub-jedrusiak/VelesResearch.git
+pip install velesresearch@git+https://github.com/jakub-jedrusiak/VelesResearch.git
 ```
```

### Comparing `velesresearch-0.0.8/pyproject.toml` & `velesresearch-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "velesresearch"
-version = "0.0.8"
+version = "0.0.9"
 description = "Veles is a free and open source python survey tool for researchers."
 license = "GPL-3.0-or-later"
 authors = ["Jakub Jędrusiak <kuba23031999@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jakub-jedrusiak/VelesResearch"
 documentation = "https://jakub-jedrusiak.github.io/VelesDocs"
 packages = [{include = "velesresearch"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.24.3"
 pydantic = "^1.10.9"
+pynpm = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 pytest = "^7.3.2"
 coverage = "^7.2.7"
 pylint-pydantic = "^0.1.8"
+ipykernel = "^6.23.2"
 
 [tool.pylint]
 load-plugins = "pylint_pydantic"
 
 [tool.pylint.'MESSAGES CONTROL']
 extension-pkg-whitelist = "pydantic"
```

### Comparing `velesresearch-0.0.8/velesresearch/options.py` & `velesresearch-0.0.9/velesresearch/options.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.8/velesresearch/questiontypes.py` & `velesresearch-0.0.9/velesresearch/questiontypes.py`

 * *Files identical despite different names*

### Comparing `velesresearch-0.0.8/velesresearch/structure.py` & `velesresearch-0.0.9/velesresearch/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 "Structural elements of the survey"
+from __future__ import annotations
+from os import getcwd
+from pathlib import Path
 from collections.abc import Sequence
-from json import JSONEncoder, dumps
+from json import JSONEncoder
 from pydantic import BaseModel, validator
 import numpy as np
 from .options import QuestionOptions, PageOptions, SurveyOptions
+from .generator import install_npm_deps, generate_survey, build_survey
 
 
 class Question(BaseModel):
     "General question class"
     label: str
     question_text: str
     answers: str | Sequence[str]
@@ -65,14 +69,15 @@
             for question in self.questions:
                 if question.label == index:
                     return question
 
 
 class Survey(BaseModel):
     "General survey class"
+    label: str
     pages: Page | Sequence[Page]
     title: str | None = None
     description: str | None = None
     options: SurveyOptions | None = None
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -86,20 +91,19 @@
             labels = []
             for page in pages:
                 labels.append(page.label)
             if len(labels) != len(set(labels)):
                 raise ValueError("Pages labels in survey must be unique")
         return pages
 
-    def create(self):
-        "Saves survey to survey.json file"
-        json = dumps(obj=self, cls=SurveyEncoder, indent=2)
-        survey_file = open("survey.json", "w", encoding="utf-8")
-        survey_file.write(json)
-        survey_file.close()
+    def create(self, path: str | Path = getcwd()):
+        "Create survey"
+        install_npm_deps(path=path)
+        generate_survey(self, path=path)
+        build_survey(path=path)
 
     def __str__(self):
         survey = "Survey:\n"
         for i in enumerate(self.pages):
             survey += f"  {i[0] + 1}. {i[1].label}\n"
         return survey
```

### Comparing `velesresearch-0.0.8/velesresearch/tools.py` & `velesresearch-0.0.9/velesresearch/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 "Functions and wrappers for creating survey structure"
 from collections.abc import Sequence
+from pathlib import Path
 from pydantic import validate_arguments
 import numpy as np
 from .structure import Question, Page, Survey
 from .options import QuestionOptions, PageOptions, SurveyOptions
 
 
 @validate_arguments
@@ -58,21 +59,28 @@
         title=title,
         description=description,
         options=options,
     )
 
 
 def survey(
+    label: str,
     *pages: Page | Sequence[Page],
     title: str | None = None,
     description: str | None = None,
     options: SurveyOptions | None = None,
-    create_file: bool = True,
+    create: bool | str | Path = True,
 ) -> Survey:
     "Create Survey object from pages, create json file"
     pages_list = list(np.concatenate([pages]).flat)
     survey_obj = Survey(
-        pages=pages_list, title=title, description=description, options=options
+        label=label,
+        pages=pages_list,
+        title=title,
+        description=description,
+        options=options,
     )
-    if create_file:
+    if create and isinstance(create, bool):
         survey_obj.create()
+    elif isinstance(create, str) or isinstance(create, Path):
+        survey_obj.create(Path(create))
     return survey_obj
```

### Comparing `velesresearch-0.0.8/PKG-INFO` & `velesresearch-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: velesresearch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Veles is a free and open source python survey tool for researchers.
 Home-page: https://github.com/jakub-jedrusiak/VelesResearch
 License: GPL-3.0-or-later
 Author: Jakub Jędrusiak
 Author-email: kuba23031999@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pynpm (>=0.1.2,<0.2.0)
 Project-URL: Documentation, https://jakub-jedrusiak.github.io/VelesDocs
 Project-URL: Repository, https://github.com/jakub-jedrusiak/VelesResearch
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="/figs/Veles-logo-white.svg">
@@ -66,10 +67,10 @@
 You can install the current version of Veles with:
 ``` bash
 pip install velesresearch
 ```
 
 You can install development version (unstable) with:
 ``` bash
-pip install https://github.com/jakub-jedrusiak/VelesResearch.git
+pip install velesresearch@git+https://github.com/jakub-jedrusiak/VelesResearch.git
 ```
```

