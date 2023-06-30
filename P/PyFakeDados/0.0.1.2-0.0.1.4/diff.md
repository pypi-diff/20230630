# Comparing `tmp/PyFakeDados-0.0.1.2.tar.gz` & `tmp/PyFakeDados-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.1.2.tar", last modified: Fri Jun 30 01:37:14 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.1.4.tar", last modified: Fri Jun 30 01:39:18 2023, max compression
```

## Comparing `PyFakeDados-0.0.1.2.tar` & `PyFakeDados-0.0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:37:14.171638 PyFakeDados-0.0.1.2/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)    35148 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.2/LICENSE.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      770 2023-06-30 01:37:14.171638 PyFakeDados-0.0.1.2/PKG-INFO
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:37:14.167638 PyFakeDados-0.0.1.2/PyFakeDados/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       23 2023-06-30 01:37:12.000000 PyFakeDados-0.0.1.2/PyFakeDados/__init__.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      857 2023-06-29 22:47:13.000000 PyFakeDados-0.0.1.2/PyFakeDados/bairro.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1650 2023-06-30 00:07:20.000000 PyFakeDados-0.0.1.2/PyFakeDados/cep.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1771 2023-06-29 23:29:37.000000 PyFakeDados-0.0.1.2/PyFakeDados/cnpj.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1487 2023-06-29 23:59:11.000000 PyFakeDados-0.0.1.2/PyFakeDados/cpf.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      177 2023-06-30 00:10:57.000000 PyFakeDados-0.0.1.2/PyFakeDados/ctps.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      774 2023-06-30 00:00:44.000000 PyFakeDados-0.0.1.2/PyFakeDados/email.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2385 2023-06-29 23:32:21.000000 PyFakeDados-0.0.1.2/PyFakeDados/empresa.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1715 2023-06-29 23:00:47.000000 PyFakeDados-0.0.1.2/PyFakeDados/estado.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      164 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.2/PyFakeDados/inscricao_estudal.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      798 2023-06-29 22:57:01.000000 PyFakeDados-0.0.1.2/PyFakeDados/logradouro.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1256 2023-06-29 23:17:05.000000 PyFakeDados-0.0.1.2/PyFakeDados/municipio.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3278 2023-06-30 00:32:32.000000 PyFakeDados-0.0.1.2/PyFakeDados/nome.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2277 2023-06-30 00:56:56.000000 PyFakeDados-0.0.1.2/PyFakeDados/pessoa.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      170 2023-06-30 00:12:54.000000 PyFakeDados-0.0.1.2/PyFakeDados/pis.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      389 2023-06-30 00:36:02.000000 PyFakeDados-0.0.1.2/PyFakeDados/senha.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      388 2023-06-30 00:01:25.000000 PyFakeDados-0.0.1.2/PyFakeDados/site.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1809 2023-06-29 23:17:13.000000 PyFakeDados-0.0.1.2/PyFakeDados/telefone.py
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2072 2023-06-30 00:57:48.000000 PyFakeDados-0.0.1.2/PyFakeDados/utils.py
-drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:37:14.171638 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      770 2023-06-30 01:37:14.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/PKG-INFO
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      669 2023-06-30 01:37:14.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-06-30 01:37:14.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-06-30 01:31:53.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/not-zip-safe
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       19 2023-06-30 01:37:14.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/requires.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       12 2023-06-30 01:37:14.000000 PyFakeDados-0.0.1.2/PyFakeDados.egg-info/top_level.txt
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      205 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.2/README.md
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      775 2023-06-30 01:37:14.171638 PyFakeDados-0.0.1.2/setup.cfg
--rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       38 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.2/setup.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:39:18.786738 PyFakeDados-0.0.1.4/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)    35148 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.4/LICENSE.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      770 2023-06-30 01:39:18.786738 PyFakeDados-0.0.1.4/PKG-INFO
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:39:18.786738 PyFakeDados-0.0.1.4/PyFakeDados/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       23 2023-06-30 01:39:16.000000 PyFakeDados-0.0.1.4/PyFakeDados/__init__.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      857 2023-06-29 22:47:13.000000 PyFakeDados-0.0.1.4/PyFakeDados/bairro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1650 2023-06-30 00:07:20.000000 PyFakeDados-0.0.1.4/PyFakeDados/cep.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1771 2023-06-29 23:29:37.000000 PyFakeDados-0.0.1.4/PyFakeDados/cnpj.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1487 2023-06-29 23:59:11.000000 PyFakeDados-0.0.1.4/PyFakeDados/cpf.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      177 2023-06-30 00:10:57.000000 PyFakeDados-0.0.1.4/PyFakeDados/ctps.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      774 2023-06-30 00:00:44.000000 PyFakeDados-0.0.1.4/PyFakeDados/email.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2385 2023-06-29 23:32:21.000000 PyFakeDados-0.0.1.4/PyFakeDados/empresa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1715 2023-06-29 23:00:47.000000 PyFakeDados-0.0.1.4/PyFakeDados/estado.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      164 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.4/PyFakeDados/inscricao_estudal.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      798 2023-06-29 22:57:01.000000 PyFakeDados-0.0.1.4/PyFakeDados/logradouro.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1256 2023-06-29 23:17:05.000000 PyFakeDados-0.0.1.4/PyFakeDados/municipio.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     3278 2023-06-30 00:32:32.000000 PyFakeDados-0.0.1.4/PyFakeDados/nome.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2277 2023-06-30 00:56:56.000000 PyFakeDados-0.0.1.4/PyFakeDados/pessoa.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      170 2023-06-30 00:12:54.000000 PyFakeDados-0.0.1.4/PyFakeDados/pis.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      389 2023-06-30 00:36:02.000000 PyFakeDados-0.0.1.4/PyFakeDados/senha.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      388 2023-06-30 00:01:25.000000 PyFakeDados-0.0.1.4/PyFakeDados/site.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     1809 2023-06-29 23:17:13.000000 PyFakeDados-0.0.1.4/PyFakeDados/telefone.py
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)     2072 2023-06-30 00:57:48.000000 PyFakeDados-0.0.1.4/PyFakeDados/utils.py
+drwxrwxr-x   0 juliansantos  (1000) juliansantos  (1000)        0 2023-06-30 01:39:18.786738 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      770 2023-06-30 01:39:18.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      669 2023-06-30 01:39:18.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-06-30 01:39:18.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)        1 2023-06-30 01:31:53.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       10 2023-06-30 01:39:18.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/requires.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       12 2023-06-30 01:39:18.000000 PyFakeDados-0.0.1.4/PyFakeDados.egg-info/top_level.txt
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      205 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.4/README.md
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)      765 2023-06-30 01:39:18.790738 PyFakeDados-0.0.1.4/setup.cfg
+-rw-rw-r--   0 juliansantos  (1000) juliansantos  (1000)       38 2023-06-29 22:25:25.000000 PyFakeDados-0.0.1.4/setup.py
```

### Comparing `PyFakeDados-0.0.1.2/LICENSE.txt` & `PyFakeDados-0.0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PKG-INFO` & `PyFakeDados-0.0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.1.2
+Version: 0.0.1.4
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/bairro.py` & `PyFakeDados-0.0.1.4/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/cep.py` & `PyFakeDados-0.0.1.4/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.1.4/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/cpf.py` & `PyFakeDados-0.0.1.4/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/email.py` & `PyFakeDados-0.0.1.4/PyFakeDados/email.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/empresa.py` & `PyFakeDados-0.0.1.4/PyFakeDados/empresa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/estado.py` & `PyFakeDados-0.0.1.4/PyFakeDados/estado.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.1.4/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/municipio.py` & `PyFakeDados-0.0.1.4/PyFakeDados/municipio.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/nome.py` & `PyFakeDados-0.0.1.4/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.1.4/PyFakeDados/pessoa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/telefone.py` & `PyFakeDados-0.0.1.4/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados/utils.py` & `PyFakeDados-0.0.1.4/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.1.4/PyFakeDados.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.1.2
+Version: 0.0.1.4
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `PyFakeDados-0.0.1.2/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.1.4/PyFakeDados.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.1.2/setup.cfg` & `PyFakeDados-0.0.1.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,13 @@
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	requests
-	unidecode
+	Unidecode
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

