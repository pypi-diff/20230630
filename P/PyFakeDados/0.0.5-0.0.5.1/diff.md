# Comparing `tmp/PyFakeDados-0.0.5.tar.gz` & `tmp/PyFakeDados-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.5.tar", last modified: Fri Jun 30 17:40:37 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.5.1.tar", last modified: Fri Jun 30 19:06:38 2023, max compression
```

## Comparing `PyFakeDados-0.0.5.tar` & `PyFakeDados-0.0.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.272130 PyFakeDados-0.0.5/
--rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3484 2023-06-30 17:40:37.272130 PyFakeDados-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.246177 PyFakeDados-0.0.5/PyFakeDados/
--rw-rw-rw-   0        0        0       21 2023-06-30 17:40:17.000000 PyFakeDados-0.0.5/PyFakeDados/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/bairro.py
--rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cep.py
--rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cnpj.py
--rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cpf.py
--rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/ctps.py
--rw-rw-rw-   0        0        0      849 2023-06-30 17:24:54.000000 PyFakeDados-0.0.5/PyFakeDados/email.py
--rw-rw-rw-   0        0        0     3183 2023-06-30 17:37:40.000000 PyFakeDados-0.0.5/PyFakeDados/empresa.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/estado.py
--rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.5/PyFakeDados/inscricao_estadual.py
--rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/logradouro.py
--rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/municipio.py
--rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/nome.py
--rw-rw-rw-   0        0        0     2587 2023-06-30 15:10:31.000000 PyFakeDados-0.0.5/PyFakeDados/pessoa.py
--rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/pis.py
--rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.5/PyFakeDados/rg.py
--rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/senha.py
--rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/site.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.268529 PyFakeDados-0.0.5/PyFakeDados/src/
--rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.5/PyFakeDados/src/estados.csv
--rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.5/PyFakeDados/src/municipios.csv
--rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/telefone.py
--rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.267058 PyFakeDados-0.0.5/PyFakeDados.egg-info/
--rw-rw-rw-   0        0        0     3484 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      759 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.5/README.md
--rw-rw-rw-   0        0        0      848 2023-06-30 17:40:37.274549 PyFakeDados-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.869212 PyFakeDados-0.0.5.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3486 2023-06-30 19:06:38.870066 PyFakeDados-0.0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.829006 PyFakeDados-0.0.5.1/PyFakeDados/
+-rw-rw-rw-   0        0        0       23 2023-06-30 19:01:18.000000 PyFakeDados-0.0.5.1/PyFakeDados/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/bairro.py
+-rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cep.py
+-rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cnpj.py
+-rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/cpf.py
+-rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/ctps.py
+-rw-rw-rw-   0        0        0      849 2023-06-30 17:24:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/email.py
+-rw-rw-rw-   0        0        0     5379 2023-06-30 18:58:05.000000 PyFakeDados-0.0.5.1/PyFakeDados/empresa.py
+-rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/estado.py
+-rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.5.1/PyFakeDados/inscricao_estadual.py
+-rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/logradouro.py
+-rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/municipio.py
+-rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/nome.py
+-rw-rw-rw-   0        0        0     2965 2023-06-30 18:29:17.000000 PyFakeDados-0.0.5.1/PyFakeDados/pessoa.py
+-rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/pis.py
+-rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.5.1/PyFakeDados/rg.py
+-rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/senha.py
+-rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/site.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.865958 PyFakeDados-0.0.5.1/PyFakeDados/src/
+-rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.5.1/PyFakeDados/src/estados.csv
+-rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.5.1/PyFakeDados/src/municipios.csv
+-rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/telefone.py
+-rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5.1/PyFakeDados/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 19:06:38.859601 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/
+-rw-rw-rw-   0        0        0     3486 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      759 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 19:06:38.000000 PyFakeDados-0.0.5.1/PyFakeDados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.5.1/README.md
+-rw-rw-rw-   0        0        0      848 2023-06-30 19:06:38.871083 PyFakeDados-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5.1/setup.py
```

### Comparing `PyFakeDados-0.0.5/LICENSE.txt` & `PyFakeDados-0.0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PKG-INFO` & `PyFakeDados-0.0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.5/PyFakeDados/bairro.py` & `PyFakeDados-0.0.5.1/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/cep.py` & `PyFakeDados-0.0.5.1/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.5.1/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/cpf.py` & `PyFakeDados-0.0.5.1/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/email.py` & `PyFakeDados-0.0.5.1/PyFakeDados/email.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/estado.py` & `PyFakeDados-0.0.5.1/PyFakeDados/estado.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.5.1/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/municipio.py` & `PyFakeDados-0.0.5.1/PyFakeDados/municipio.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/nome.py` & `PyFakeDados-0.0.5.1/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/rg.py` & `PyFakeDados-0.0.5.1/PyFakeDados/rg.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/src/estados.csv` & `PyFakeDados-0.0.5.1/PyFakeDados/src/estados.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/src/municipios.csv` & `PyFakeDados-0.0.5.1/PyFakeDados/src/municipios.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/telefone.py` & `PyFakeDados-0.0.5.1/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados/utils.py` & `PyFakeDados-0.0.5.1/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.5.1/PyFakeDados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.5/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.5.1/PyFakeDados.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/README.md` & `PyFakeDados-0.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.5/setup.cfg` & `PyFakeDados-0.0.5.1/setup.cfg`

 * *Files identical despite different names*

