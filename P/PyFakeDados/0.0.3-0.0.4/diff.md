# Comparing `tmp/PyFakeDados-0.0.3.tar.gz` & `tmp/PyFakeDados-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.3.tar", last modified: Fri Jun 30 15:03:20 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.4.tar", last modified: Fri Jun 30 15:11:48 2023, max compression
```

## Comparing `PyFakeDados-0.0.3.tar` & `PyFakeDados-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.842325 PyFakeDados-0.0.3/
--rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3484 2023-06-30 15:03:20.842325 PyFakeDados-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.797071 PyFakeDados-0.0.3/PyFakeDados/
--rw-rw-rw-   0        0        0       21 2023-06-30 15:02:53.000000 PyFakeDados-0.0.3/PyFakeDados/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/bairro.py
--rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cep.py
--rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cnpj.py
--rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cpf.py
--rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/ctps.py
--rw-rw-rw-   0        0        0      811 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/email.py
--rw-rw-rw-   0        0        0     3165 2023-06-30 13:07:23.000000 PyFakeDados-0.0.3/PyFakeDados/empresa.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/estado.py
--rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.3/PyFakeDados/inscricao_estudal.py
--rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/logradouro.py
--rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/municipio.py
--rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/nome.py
--rw-rw-rw-   0        0        0     2510 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/pessoa.py
--rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/pis.py
--rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.3/PyFakeDados/rg.py
--rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/senha.py
--rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/site.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.838704 PyFakeDados-0.0.3/PyFakeDados/src/
--rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.3/PyFakeDados/src/estados.csv
--rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.3/PyFakeDados/src/municipios.csv
--rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/telefone.py
--rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.836687 PyFakeDados-0.0.3/PyFakeDados.egg-info/
--rw-rw-rw-   0        0        0     3484 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.3/README.md
--rw-rw-rw-   0        0        0      848 2023-06-30 15:03:20.851956 PyFakeDados-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.056584 PyFakeDados-0.0.4/
+-rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3484 2023-06-30 15:11:48.056584 PyFakeDados-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.010060 PyFakeDados-0.0.4/PyFakeDados/
+-rw-rw-rw-   0        0        0       21 2023-06-30 15:11:10.000000 PyFakeDados-0.0.4/PyFakeDados/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/bairro.py
+-rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cep.py
+-rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cnpj.py
+-rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cpf.py
+-rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/ctps.py
+-rw-rw-rw-   0        0        0      811 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/email.py
+-rw-rw-rw-   0        0        0     3165 2023-06-30 13:07:23.000000 PyFakeDados-0.0.4/PyFakeDados/empresa.py
+-rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/estado.py
+-rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.4/PyFakeDados/inscricao_estudal.py
+-rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/logradouro.py
+-rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/municipio.py
+-rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/nome.py
+-rw-rw-rw-   0        0        0     2587 2023-06-30 15:10:31.000000 PyFakeDados-0.0.4/PyFakeDados/pessoa.py
+-rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/pis.py
+-rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.4/PyFakeDados/rg.py
+-rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/senha.py
+-rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/site.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.053039 PyFakeDados-0.0.4/PyFakeDados/src/
+-rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.4/PyFakeDados/src/estados.csv
+-rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.4/PyFakeDados/src/municipios.csv
+-rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/telefone.py
+-rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.051034 PyFakeDados-0.0.4/PyFakeDados.egg-info/
+-rw-rw-rw-   0        0        0     3484 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.4/README.md
+-rw-rw-rw-   0        0        0      848 2023-06-30 15:11:48.064285 PyFakeDados-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.4/setup.py
```

### Comparing `PyFakeDados-0.0.3/LICENSE.txt` & `PyFakeDados-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PKG-INFO` & `PyFakeDados-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.3/PyFakeDados/bairro.py` & `PyFakeDados-0.0.4/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/cep.py` & `PyFakeDados-0.0.4/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.4/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/cpf.py` & `PyFakeDados-0.0.4/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/email.py` & `PyFakeDados-0.0.4/PyFakeDados/email.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/empresa.py` & `PyFakeDados-0.0.4/PyFakeDados/empresa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/estado.py` & `PyFakeDados-0.0.4/PyFakeDados/estado.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.4/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/municipio.py` & `PyFakeDados-0.0.4/PyFakeDados/municipio.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/nome.py` & `PyFakeDados-0.0.4/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.4/PyFakeDados/pessoa.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from PyFakeDados.bairro import gerar_bairro
 from PyFakeDados.logradouro import gerar_logradouro, gerar_numero
 from PyFakeDados.telefone import gerar_telefone_fixo, gerar_telefone_celular
 from PyFakeDados.email import gerar_email, gerar_email_pessoa
 from PyFakeDados.senha import gerar_senha, gerar_senha_numerica
 from PyFakeDados.site import gerar_site
 from PyFakeDados.cpf import gerar_cpf
+from PyFakeDados.rg import gerar_rg
 from PyFakeDados.ctps import gerar_ctps
 from PyFakeDados.pis import gerar_pis
 from PyFakeDados.utils import gerar_data, gerar_data_nascimento
 
 def gerar_pessoa(uf=None, mask=False, idade=None, recem_nascido=False):
 
     if uf is None:
@@ -32,14 +33,15 @@
 
     pessoa = {}
     data_nascimento = gerar_data_nascimento(idade)
     
     sexo = gerar_sexo()
     nome, mae, pai = gerar_nome_com_filiacao()
     cpf = gerar_cpf(mask=mask)
+    rg = gerar_rg()
     ctps = gerar_ctps()
     pis = gerar_pis()
     data_nascimento = data_nascimento
     site = gerar_site(nome)
     email = gerar_email_pessoa(nome)
     senha = gerar_senha_numerica()
     senha_forte = gerar_senha(16)
@@ -54,14 +56,15 @@
 
     pessoa = {
         "sexo": sexo,
         "nome": nome,
         "mae": mae,
         "pai": pai,
         "cpf": cpf,
+        "rg": rg,
         "ctps": ctps,
         "pis": pis,
         "data_nascimento": data_nascimento.strftime("%d/%m/%Y"),
         "site": site,
         "email": email,
         "senha": senha,
         "senha_forte": senha_forte,
```

### Comparing `PyFakeDados-0.0.3/PyFakeDados/rg.py` & `PyFakeDados-0.0.4/PyFakeDados/rg.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/src/estados.csv` & `PyFakeDados-0.0.4/PyFakeDados/src/estados.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/src/municipios.csv` & `PyFakeDados-0.0.4/PyFakeDados/src/municipios.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/telefone.py` & `PyFakeDados-0.0.4/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados/utils.py` & `PyFakeDados-0.0.4/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.4/PyFakeDados.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.3/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.4/PyFakeDados.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/README.md` & `PyFakeDados-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.3/setup.cfg` & `PyFakeDados-0.0.4/setup.cfg`

 * *Files identical despite different names*

