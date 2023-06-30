# Comparing `tmp/rcdesign-0.4.8.tar.gz` & `tmp/rcdesign-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcdesign-0.4.8.tar", last modified: Tue Jan 24 07:19:48 2023, max compression
+gzip compressed data, was "rcdesign-0.4.9.tar", last modified: Tue Jan 24 07:39:13 2023, max compression
```

## Comparing `rcdesign-0.4.8.tar` & `rcdesign-0.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       90 2023-01-24 07:02:19.433600 rcdesign-0.4.8/.flake8
--rw-r--r--   0        0        0     1093 2023-01-19 11:14:14.566184 rcdesign-0.4.8/LICENSE.md
--rw-r--r--   0        0        0     4611 2023-01-24 06:43:33.009016 rcdesign-0.4.8/README.md
--rw-r--r--   0        0        0      180 2023-01-19 11:14:14.572184 rcdesign-0.4.8/mypy.ini
--rw-r--r--   0        0        0     1996 2023-01-19 11:14:14.573183 rcdesign-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       23 2023-01-24 06:43:35.892247 rcdesign-0.4.8/rcdesign/__about__.py
--rw-r--r--   0        0        0      142 2023-01-19 11:14:14.574184 rcdesign-0.4.8/rcdesign/__init__.py
--rw-r--r--   0        0        0     1259 2023-01-19 11:14:14.574184 rcdesign-0.4.8/rcdesign/__main__.py
--rw-r--r--   0        0        0      121 2023-01-19 11:14:14.574184 rcdesign-0.4.8/rcdesign/is456/__init__.py
--rw-r--r--   0        0        0     1784 2023-01-19 11:14:14.575184 rcdesign-0.4.8/rcdesign/is456/concrete.py
--rw-r--r--   0        0        0     1532 2023-01-19 11:14:14.575184 rcdesign-0.4.8/rcdesign/is456/design.py
--rw-r--r--   0        0        0    20696 2023-01-19 11:14:14.576185 rcdesign-0.4.8/rcdesign/is456/rebar.py
--rw-r--r--   0        0        0    21059 2023-01-24 07:10:08.187357 rcdesign-0.4.8/rcdesign/is456/section.py
--rw-r--r--   0        0        0     5079 2023-01-24 07:06:57.760946 rcdesign-0.4.8/rcdesign/is456/stressblock.py
--rw-r--r--   0        0        0     1085 2023-01-19 11:14:14.578186 rcdesign-0.4.8/rcdesign/utils.py
--rw-r--r--   0        0        0       75 2023-01-19 11:14:14.578186 rcdesign-0.4.8/requirements.txt
--rw-r--r--   0        0        0     6275 1970-01-01 00:00:00.000000 rcdesign-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0       90 2023-01-24 07:02:19.433600 rcdesign-0.4.9/.flake8
+-rw-r--r--   0        0        0     1093 2023-01-19 11:14:14.566184 rcdesign-0.4.9/LICENSE.md
+-rw-r--r--   0        0        0     4611 2023-01-24 07:34:53.246269 rcdesign-0.4.9/README.md
+-rw-r--r--   0        0        0      180 2023-01-19 11:14:14.572184 rcdesign-0.4.9/mypy.ini
+-rw-r--r--   0        0        0     1996 2023-01-19 11:14:14.573183 rcdesign-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-01-24 07:34:53.265600 rcdesign-0.4.9/rcdesign/__about__.py
+-rw-r--r--   0        0        0      142 2023-01-19 11:14:14.574184 rcdesign-0.4.9/rcdesign/__init__.py
+-rw-r--r--   0        0        0     1259 2023-01-19 11:14:14.574184 rcdesign-0.4.9/rcdesign/__main__.py
+-rw-r--r--   0        0        0      121 2023-01-19 11:14:14.574184 rcdesign-0.4.9/rcdesign/is456/__init__.py
+-rw-r--r--   0        0        0     1784 2023-01-19 11:14:14.575184 rcdesign-0.4.9/rcdesign/is456/concrete.py
+-rw-r--r--   0        0        0     1532 2023-01-19 11:14:14.575184 rcdesign-0.4.9/rcdesign/is456/design.py
+-rw-r--r--   0        0        0    20705 2023-01-24 07:23:56.264922 rcdesign-0.4.9/rcdesign/is456/rebar.py
+-rw-r--r--   0        0        0    21059 2023-01-24 07:10:08.187357 rcdesign-0.4.9/rcdesign/is456/section.py
+-rw-r--r--   0        0        0     5079 2023-01-24 07:06:57.760946 rcdesign-0.4.9/rcdesign/is456/stressblock.py
+-rw-r--r--   0        0        0     1085 2023-01-19 11:14:14.578186 rcdesign-0.4.9/rcdesign/utils.py
+-rw-r--r--   0        0        0       75 2023-01-19 11:14:14.578186 rcdesign-0.4.9/requirements.txt
+-rw-r--r--   0        0        0     6275 1970-01-01 00:00:00.000000 rcdesign-0.4.9/PKG-INFO
```

### Comparing `rcdesign-0.4.8/LICENSE.md` & `rcdesign-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/README.md` & `rcdesign-0.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 > (.venv) > _
 ```
 
 Install using `pip`
 ```bash
 $ (.venv) pip install -U rcdesign
 $ (.venv) python -c "from rcdesign import __version__;print(__version____)
-$ 0.4.8
+$ 0.4.9
 ```
 
 Run the two built-in examples problem and study the output.
 ```bash
 $ (.venv) python -m rcdesign
 ```
 
@@ -123,14 +123,14 @@
 1. Bug reports
 2. Additional features
 3. Documentation
 4. Additional examples
 
 ## Links
 - Documentation: [Documentation](https://rcdesign.readthedocs.io/en/latest/)
-- PyPI release: [0.4.8](https://pypi.org/project/rcdesign/)
+- PyPI release: [0.4.9](https://pypi.org/project/rcdesign/)
 - Github repository: https://github.com/satish-annigeri/rcdesign
 
 ## References
 1. IS 456:2000 Indian Standard Code of Practice for Plain and Reinforced Concrete (Fourth Revision), Bureau of Indian Standards, New Delhi, 2000.
 2. SP:24 (S&T)-1983 Explanatory Handbook on Indian Standard Code of Practice for Plain and Reinforced Concrete (IS 456:1978), Bureau of Indian Standards, New Delhi, 1984.
 3. SP 16:1980 Design Aids for Reinforced Concrete to IS:456-1978, Bureau of Indian Standards, New Delhi, 1980.
```

### Comparing `rcdesign-0.4.8/pyproject.toml` & `rcdesign-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/__main__.py` & `rcdesign-0.4.9/rcdesign/__main__.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/is456/concrete.py` & `rcdesign-0.4.9/rcdesign/is456/concrete.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/is456/design.py` & `rcdesign-0.4.9/rcdesign/is456/design.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/is456/rebar.py` & `rcdesign-0.4.9/rcdesign/is456/rebar.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
         area = 0.0
         for bar_dia in self.bars:
             area += bar_dia**2
         self.__Asv = pi / 4 * area
         return self.__Asv
 
     @property
-    def Asv(self):
+    def Asv(self) -> float:
         return self._Asv()
 
     def Vus(self, d: float = 0.0) -> float:
         V_us = self.rebar.fd * self.Asv
         alpha_rad = self._alpha_deg * pi / 180
         if self._sv == 0:  # Single group of parallel bars
             V_us *= sin(alpha_rad)
```

### Comparing `rcdesign-0.4.8/rcdesign/is456/section.py` & `rcdesign-0.4.9/rcdesign/is456/section.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/is456/stressblock.py` & `rcdesign-0.4.9/rcdesign/is456/stressblock.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/rcdesign/utils.py` & `rcdesign-0.4.9/rcdesign/utils.py`

 * *Files identical despite different names*

### Comparing `rcdesign-0.4.8/PKG-INFO` & `rcdesign-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcdesign
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Python package for reinforced concrete analysis and design as per IS 456:2000
 Author-email: Satish Annigeri <satish.annigeri@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -73,15 +73,15 @@
 > (.venv) > _
 ```
 
 Install using `pip`
 ```bash
 $ (.venv) pip install -U rcdesign
 $ (.venv) python -c "from rcdesign import __version__;print(__version____)
-$ 0.4.8
+$ 0.4.9
 ```
 
 Run the two built-in examples problem and study the output.
 ```bash
 $ (.venv) python -m rcdesign
 ```
 
@@ -164,14 +164,14 @@
 1. Bug reports
 2. Additional features
 3. Documentation
 4. Additional examples
 
 ## Links
 - Documentation: [Documentation](https://rcdesign.readthedocs.io/en/latest/)
-- PyPI release: [0.4.8](https://pypi.org/project/rcdesign/)
+- PyPI release: [0.4.9](https://pypi.org/project/rcdesign/)
 - Github repository: https://github.com/satish-annigeri/rcdesign
 
 ## References
 1. IS 456:2000 Indian Standard Code of Practice for Plain and Reinforced Concrete (Fourth Revision), Bureau of Indian Standards, New Delhi, 2000.
 2. SP:24 (S&T)-1983 Explanatory Handbook on Indian Standard Code of Practice for Plain and Reinforced Concrete (IS 456:1978), Bureau of Indian Standards, New Delhi, 1984.
 3. SP 16:1980 Design Aids for Reinforced Concrete to IS:456-1978, Bureau of Indian Standards, New Delhi, 1980.
```

