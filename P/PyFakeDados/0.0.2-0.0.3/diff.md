# Comparing `tmp/PyFakeDados-0.0.2.tar.gz` & `tmp/PyFakeDados-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.2.tar", last modified: Fri Jun 30 13:17:57 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.3.tar", last modified: Fri Jun 30 15:03:20 2023, max compression
```

## Comparing `PyFakeDados-0.0.2.tar` & `PyFakeDados-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:17:57.751921 PyFakeDados-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2406 2023-06-30 13:17:57.751921 PyFakeDados-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 13:17:57.728196 PyFakeDados-0.0.2/PyFakeDados/
--rw-rw-rw-   0        0        0       21 2023-06-30 13:17:12.000000 PyFakeDados-0.0.2/PyFakeDados/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/bairro.py
--rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/cep.py
--rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/cnpj.py
--rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/cpf.py
--rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/ctps.py
--rw-rw-rw-   0        0        0      811 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/email.py
--rw-rw-rw-   0        0        0     3165 2023-06-30 13:07:23.000000 PyFakeDados-0.0.2/PyFakeDados/empresa.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/estado.py
--rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.2/PyFakeDados/inscricao_estudal.py
--rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/logradouro.py
--rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/municipio.py
--rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/nome.py
--rw-rw-rw-   0        0        0     2510 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/pessoa.py
--rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/pis.py
--rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/senha.py
--rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/site.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:17:57.749474 PyFakeDados-0.0.2/PyFakeDados/src/
--rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.2/PyFakeDados/src/estados.csv
--rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.2/PyFakeDados/src/municipios.csv
--rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/telefone.py
--rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.2/PyFakeDados/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:17:57.745995 PyFakeDados-0.0.2/PyFakeDados.egg-info/
--rw-rw-rw-   0        0        0     2406 2023-06-30 13:17:57.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      740 2023-06-30 13:17:57.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:17:57.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-30 13:17:57.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 13:17:57.000000 PyFakeDados-0.0.2/PyFakeDados.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1761 2023-06-30 12:15:43.000000 PyFakeDados-0.0.2/README.md
--rw-rw-rw-   0        0        0      848 2023-06-30 13:17:57.755197 PyFakeDados-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.842325 PyFakeDados-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3484 2023-06-30 15:03:20.842325 PyFakeDados-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.797071 PyFakeDados-0.0.3/PyFakeDados/
+-rw-rw-rw-   0        0        0       21 2023-06-30 15:02:53.000000 PyFakeDados-0.0.3/PyFakeDados/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/bairro.py
+-rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cep.py
+-rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cnpj.py
+-rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/cpf.py
+-rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/ctps.py
+-rw-rw-rw-   0        0        0      811 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/email.py
+-rw-rw-rw-   0        0        0     3165 2023-06-30 13:07:23.000000 PyFakeDados-0.0.3/PyFakeDados/empresa.py
+-rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/estado.py
+-rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.3/PyFakeDados/inscricao_estudal.py
+-rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/logradouro.py
+-rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/municipio.py
+-rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/nome.py
+-rw-rw-rw-   0        0        0     2510 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/pessoa.py
+-rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/pis.py
+-rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.3/PyFakeDados/rg.py
+-rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/senha.py
+-rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/site.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.838704 PyFakeDados-0.0.3/PyFakeDados/src/
+-rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.3/PyFakeDados/src/estados.csv
+-rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.3/PyFakeDados/src/municipios.csv
+-rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/telefone.py
+-rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.3/PyFakeDados/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 15:03:20.836687 PyFakeDados-0.0.3/PyFakeDados.egg-info/
+-rw-rw-rw-   0        0        0     3484 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 15:03:20.000000 PyFakeDados-0.0.3/PyFakeDados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.3/README.md
+-rw-rw-rw-   0        0        0      848 2023-06-30 15:03:20.851956 PyFakeDados-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.3/setup.py
```

### Comparing `PyFakeDados-0.0.2/LICENSE.txt` & `PyFakeDados-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PKG-INFO` & `PyFakeDados-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1
-Name: PyFakeDados
-Version: 0.0.2
-Summary: Generic generator fake data for application and api development.
-Home-page: https://github.com/juliansantosinfo/PyFakeDados
-Author: Julian de Almeida Santos
-Author-email: julian.santos.info@gmail.com
-License: GPLv3
-Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
-Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # PyFakeDados
 
 ![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
 
 PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
 
+O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
+
+A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
+
+Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
+
+Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
+
 ## Recursos
 
 PyFakeDados é capaz de gerar os seguintes tipos de dados:
 
 - Nome
 - Sobrenome
 - Nome completo
```

### Comparing `PyFakeDados-0.0.2/PyFakeDados/bairro.py` & `PyFakeDados-0.0.3/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/cep.py` & `PyFakeDados-0.0.3/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.3/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/cpf.py` & `PyFakeDados-0.0.3/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/email.py` & `PyFakeDados-0.0.3/PyFakeDados/email.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/empresa.py` & `PyFakeDados-0.0.3/PyFakeDados/empresa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/estado.py` & `PyFakeDados-0.0.3/PyFakeDados/estado.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.3/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/municipio.py` & `PyFakeDados-0.0.3/PyFakeDados/municipio.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/nome.py` & `PyFakeDados-0.0.3/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.3/PyFakeDados/pessoa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/src/estados.csv` & `PyFakeDados-0.0.3/PyFakeDados/src/estados.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/src/municipios.csv` & `PyFakeDados-0.0.3/PyFakeDados/src/municipios.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/telefone.py` & `PyFakeDados-0.0.3/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados/utils.py` & `PyFakeDados-0.0.3/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.2/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
@@ -16,14 +16,22 @@
 
 # PyFakeDados
 
 ![PyFakeDados](https://github.com/juliansantosinfo/PyFakeDados/logo.png)
 
 PyFakeDados é uma ferramenta em Python que auxilia desenvolvedores na geração de dados falsos (fake) aleatórios para bancos de dados de teste ou APIs. Com essa ferramenta, é possível gerar uma variedade de informações, como nomes, telefones, CPFs, e-mails, senhas e muito mais.
 
+O PyFakeDados oferece uma ampla gama de recursos para gerar dados em diversos formatos, como nomes, endereços, números de telefone, documentos como CPFs e CNPJs, e-mails, senhas, entre outros. Além disso, a ferramenta permite criar identidades completas de pessoas e empresas, fornecendo informações consistentes e realistas.
+
+A biblioteca é de fácil utilização e pode ser integrada facilmente a projetos em Python. Com uma simples chamada de função, você pode gerar quantidades massivas de dados falsos para preencher suas necessidades de teste. A diversidade dos dados gerados e a capacidade de personalização tornam o PyFakeDados uma ferramenta indispensável para qualquer desenvolvedor que precise de dados fictícios em seus projetos.
+
+Este repositório também fornece documentação completa sobre como usar a biblioteca e exemplos práticos para ajudá-lo a aproveitar ao máximo todas as funcionalidades do PyFakeDados.
+
+Experimente o PyFakeDados agora e torne o processo de geração de dados falsos mais eficiente e realista em seus projetos!
+
 ## Recursos
 
 PyFakeDados é capaz de gerar os seguintes tipos de dados:
 
 - Nome
 - Sobrenome
 - Nome completo
```

### Comparing `PyFakeDados-0.0.2/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.3/PyFakeDados.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 PyFakeDados/estado.py
 PyFakeDados/inscricao_estudal.py
 PyFakeDados/logradouro.py
 PyFakeDados/municipio.py
 PyFakeDados/nome.py
 PyFakeDados/pessoa.py
 PyFakeDados/pis.py
+PyFakeDados/rg.py
 PyFakeDados/senha.py
 PyFakeDados/site.py
 PyFakeDados/telefone.py
 PyFakeDados/utils.py
 PyFakeDados.egg-info/PKG-INFO
 PyFakeDados.egg-info/SOURCES.txt
 PyFakeDados.egg-info/dependency_links.txt
```

### Comparing `PyFakeDados-0.0.2/setup.cfg` & `PyFakeDados-0.0.3/setup.cfg`

 * *Files identical despite different names*

