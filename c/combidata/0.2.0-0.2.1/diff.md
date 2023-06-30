# Comparing `tmp/combidata-0.2.0.tar.gz` & `tmp/combidata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.0.tar", last modified: Tue Apr 11 20:55:05 2023, max compression
+gzip compressed data, was "combidata-0.2.1.tar", last modified: Fri Jun 30 14:19:17 2023, max compression
```

## Comparing `combidata-0.2.0.tar` & `combidata-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.039178 combidata-0.2.0/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    10026 2023-04-11 20:55:05.038179 combidata-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9245 2023-04-11 20:54:40.000000 combidata-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.007179 combidata-0.2.0/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.0/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.031177 combidata-0.2.0/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.0/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.0/combidata/classes/case.py
--rw-rw-rw-   0        0        0     1827 2023-03-02 18:36:48.000000 combidata-0.2.0/combidata/classes/combination.py
--rw-rw-rw-   0        0        0     5780 2023-04-10 17:49:35.000000 combidata-0.2.0/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.0/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.036179 combidata-0.2.0/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.0/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.0/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.0/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.0/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.025179 combidata-0.2.0/combidata.egg-info/
--rw-rw-rw-   0        0        0    10026 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 20:55:04.000000 combidata-0.2.0/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2023-04-11 20:52:22.000000 combidata-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 20:55:05.039178 combidata-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-04-11 20:54:40.000000 combidata-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 20:55:05.037178 combidata-0.2.0/tests/
--rw-rw-rw-   0        0        0     3111 2023-04-05 09:25:54.000000 combidata-0.2.0/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.850964 combidata-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    10465 2023-06-30 14:19:17.849966 combidata-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9684 2023-06-30 14:16:48.000000 combidata-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.793961 combidata-0.2.1/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.1/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.829962 combidata-0.2.1/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-04-01 06:03:08.000000 combidata-0.2.1/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     2161 2023-06-30 13:44:01.000000 combidata-0.2.1/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0     6255 2023-06-30 14:01:33.000000 combidata-0.2.1/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.1/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.844967 combidata-0.2.1/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.1/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-04-01 05:47:28.000000 combidata-0.2.1/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.1/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.1/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.820967 combidata-0.2.1/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10465 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-30 14:19:17.000000 combidata-0.2.1/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2023-06-30 14:16:48.000000 combidata-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:19:17.850964 combidata-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-06-30 14:16:48.000000 combidata-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:19:17.846969 combidata-0.2.1/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.1/tests/test_generator.py
```

### Comparing `combidata-0.2.0/LICENSE` & `combidata-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.0/PKG-INFO` & `combidata-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,19 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.1:
+1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
+2) Added logger begin
+3) And also fix bug with 'STOP' signal
+
 0.2.0:
 1) Ok, now its Beta ;)
 2) Fixed combination bug
 
 0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
@@ -294,10 +299,13 @@
 
 Telegram — https://t.me/sasisochka
 
 Linkedin — https://www.linkedin.com/in/yasasisochka/
 
 
 ## Acknowledgments
-A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone!
+A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone! And a special thanks to JetBrains for their best software and License for Open Source Development.
+
+
+[![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.png)](https://jb.gg/OpenSourceSupport)
 
 With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
```

### Comparing `combidata-0.2.0/README.md` & `combidata-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.1:
+1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
+2) Added logger begin
+3) And also fix bug with 'STOP' signal
+
 0.2.0:
 1) Ok, now its Beta ;)
 2) Fixed combination bug
 
 0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
@@ -276,10 +281,13 @@
 
 Telegram — https://t.me/sasisochka
 
 Linkedin — https://www.linkedin.com/in/yasasisochka/
 
 
 ## Acknowledgments
-A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone!
+A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone! And a special thanks to JetBrains for their best software and License for Open Source Development.
+
+
+[![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.png)](https://jb.gg/OpenSourceSupport)
 
 With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
```

### Comparing `combidata-0.2.0/combidata/classes/case.py` & `combidata-0.2.1/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.0/combidata/classes/combination.py` & `combidata-0.2.1/combidata/classes/combination.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def step_not_done(current_step_name, combi):
     if isinstance(combi, list):
         for combination in combi:
-            if combination.step_done != current_step_name or combination.step_done == "STOP":
+            if combination.step_done != current_step_name and combination.step_done != "STOP":
                 return True
     else:
-        if combi.step_done != current_step_name or combi.step_done == "STOP":
+        if combi.step_done != current_step_name and combi.step_done != "STOP":
             return True
     return False
 
 
 class Combination:
     """
     test_seed: formed in ST_COMBINE process
@@ -49,8 +49,16 @@
 
     def run(self):
         self.workflow = list(self.workflow) if isinstance(self.workflow, list) else self.workflow  # todo beautify
         workflow = self.workflow.pop(0) if isinstance(self.workflow, list) else self.workflow
         for current_step in workflow:
             while step_not_done(current_step.name, self):
                 if self.step_done != current_step.name:
-                    current_step.activate(self)
+                    try:
+                        current_step.activate(self)
+                    except Exception as e:
+                        self.step_done = "STOP"
+                        if logger := self.tools.get("logger"):
+                            logger.end_test(self.tools.get("id"), str(e))
+                        else:
+                            raise e
+
```

### Comparing `combidata-0.2.0/combidata/classes/data_generator.py` & `combidata-0.2.1/combidata/classes/data_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,28 +72,37 @@
                  types_for_generation: None | str | list = None,
                  amount: int = None):
         assert amount is None or (isinstance(amount, int) and amount > 0), "amount must be integer > 0"
         assert banned_fields is None or isinstance(banned_fields, list), "banned_fields must be list instance"
         assert possible_fields is None or isinstance(possible_fields, list), "possible_fields must be list instance"
         assert banned_fields is None or possible_fields is None, "You can't use banned_fields and possible_fields arguments simultaneously"
 
-        if possible_modes is not None:
-            for key, value in possible_modes.items():
+        modes_for_gen = copy.deepcopy(possible_modes)
+
+        if modes_for_gen is not None:
+            for key, value in modes_for_gen.items():
                 if isinstance(value, str):
-                    possible_modes[key] = [value]
+                    modes_for_gen[key] = [value]
+
+
 
         self.init_lib = {}
         for field_name, field in library["cases"].items():
             self.init_lib[field_name] = {}
             for field_mode, case in field.items():
                 self.init_lib[field_name].update(
                     {field_mode: (case if isinstance(case, Case) else Case(case, field_name, field_mode))})
-                if possible_modes is not None and field_name in possible_modes.keys() and field_mode not in possible_modes[
-                    field_name]:
-                    self.init_lib[field_name][field_mode].type_of_case = "OFF"
+                if modes_for_gen is not None:
+                    if field_name in modes_for_gen.keys() and field_mode not in modes_for_gen[field_name]:
+                        self.init_lib[field_name][field_mode].type_of_case = "OFF"
+                    elif requirements := self.init_lib[field_name][field_mode].requirements:
+                        for rec_field, rec_modes in requirements.items():
+                            if rec_field in modes_for_gen.keys() and not rec_modes & set(modes_for_gen[rec_field]):
+                                self.init_lib[field_name][field_mode].type_of_case = "OFF"
+                                break
 
         if possible_fields is not None or banned_fields is not None:
             banned_fields = banned_fields if possible_fields is None else [field for field in self.init_lib.keys() if
                                                                            field not in possible_fields]
             for field in banned_fields:
                 del self.init_lib[field]
```

### Comparing `combidata-0.2.0/combidata/processes/combine.py` & `combidata-0.2.1/combidata/processes/combine.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.0/combidata/processes/form.py` & `combidata-0.2.1/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.0/combidata/processes/genetate.py` & `combidata-0.2.1/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.0/combidata.egg-info/PKG-INFO` & `combidata-0.2.1/combidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,19 @@
 
 
 The core functionality of the Combidata library is provided by the `DataGenerator` class, which takes in test flags and a dictionary containing all cases, forms, and workflows. 
 The `DataGenerator` creates `Combination` instances from the possible cases. 
 The `run` function in each `Combination` instance processes all steps in the specified workflow.
 
 ## New features
+0.2.1:
+1) So, we have greate problem with possible_modes and other parameters. I patched it but problem still here.
+2) Added logger begin
+3) And also fix bug with 'STOP' signal
+
 0.2.0:
 1) Ok, now its Beta ;)
 2) Fixed combination bug
 
 0.1.9:
 1) Now you can use 'types_for_generation' in initialisation of 'DataGenerator'
 
@@ -294,10 +299,13 @@
 
 Telegram — https://t.me/sasisochka
 
 Linkedin — https://www.linkedin.com/in/yasasisochka/
 
 
 ## Acknowledgments
-A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone!
+A special thanks to the community for their support, contributions, and valuable feedback. Your input helps make Combidata a better tool for everyone! And a special thanks to JetBrains for their best software and License for Open Source Development.
+
+
+[![JetBrains Black Box Logo logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_square.png)](https://jb.gg/OpenSourceSupport)
 
 With Combidata, you can easily generate test data for your applications and systems, ensuring that they are robust and reliable under various conditions. Start using Combidata today to improve the quality of your testing and development process!
```

### Comparing `combidata-0.2.0/pyproject.toml` & `combidata-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.0"
+version="0.2.1"
```

### Comparing `combidata-0.2.0/setup.py` & `combidata-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.0",
+    version="0.2.1",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.0/tests/test_generator.py` & `combidata-0.2.1/tests/test_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import random
 from pprint import pprint
 
 import pytest
 from combidata.classes.case import Case
 
 from combidata.classes.combination import Combination
 
 from combidata import ST_COMBINE, ST_GENERATE, ST_FORM, DataGenerator, Process
 from re_generate import re_generate
 
 
-
-
 def code_generator(combination, example_token):
     # just for test
     return "12GG233"
 
+
 def gen_comb(combination: Combination):
     new_comb = DataGenerator(library, amount=1).get_one()
     new_comb.run()
     return new_comb.generated_data
 
+
 def gen_smile():
     return ":)"
 
+
 def gen_value(value):
     return value
 
 
 library = {
     "cases": {},
     "workflow": (ST_COMBINE, ST_GENERATE, ST_FORM),
@@ -94,16 +96,14 @@
         "value": "Hi",
         "gen_func": gen_value,
         "options": {"value": "value"},
         "name": "Exp Hi"
     },
 }
 
-
-
 generator = DataGenerator(library, amount=100)
 generator.run()
 
 
 @pytest.mark.parametrize("combination_name", generator.combinations.keys())
 def test(combination_name):
     combination = generator.combinations[combination_name]
@@ -120,7 +120,18 @@
     seed = combination.test_seed
     print()
     print(seed)
     gen_seed: Combination = DataGenerator(library, possible_modes=seed, amount=1).get_one()
     gen_seed.run()
     gen_seed = gen_seed.test_seed
     assert seed == gen_seed
+
+@pytest.mark.parametrize("combination_name", generator.combinations.keys())
+def test3(combination_name):
+    combination = generator.combinations[combination_name]
+    seed = combination.test_seed
+    key = random.choice(list(seed.keys()))
+    seed = {key: seed[key]}
+    print(seed)
+    semi_gen = DataGenerator(library, possible_modes=seed, amount=100)
+    semi_gen.run()
+
```

