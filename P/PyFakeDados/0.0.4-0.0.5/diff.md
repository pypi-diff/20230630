# Comparing `tmp/PyFakeDados-0.0.4.tar.gz` & `tmp/PyFakeDados-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFakeDados-0.0.4.tar", last modified: Fri Jun 30 15:11:48 2023, max compression
+gzip compressed data, was "PyFakeDados-0.0.5.tar", last modified: Fri Jun 30 17:40:37 2023, max compression
```

## Comparing `PyFakeDados-0.0.4.tar` & `PyFakeDados-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.056584 PyFakeDados-0.0.4/
--rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3484 2023-06-30 15:11:48.056584 PyFakeDados-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.010060 PyFakeDados-0.0.4/PyFakeDados/
--rw-rw-rw-   0        0        0       21 2023-06-30 15:11:10.000000 PyFakeDados-0.0.4/PyFakeDados/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/bairro.py
--rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cep.py
--rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cnpj.py
--rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/cpf.py
--rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/ctps.py
--rw-rw-rw-   0        0        0      811 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/email.py
--rw-rw-rw-   0        0        0     3165 2023-06-30 13:07:23.000000 PyFakeDados-0.0.4/PyFakeDados/empresa.py
--rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/estado.py
--rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.4/PyFakeDados/inscricao_estudal.py
--rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/logradouro.py
--rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/municipio.py
--rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/nome.py
--rw-rw-rw-   0        0        0     2587 2023-06-30 15:10:31.000000 PyFakeDados-0.0.4/PyFakeDados/pessoa.py
--rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/pis.py
--rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.4/PyFakeDados/rg.py
--rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/senha.py
--rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/site.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.053039 PyFakeDados-0.0.4/PyFakeDados/src/
--rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.4/PyFakeDados/src/estados.csv
--rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.4/PyFakeDados/src/municipios.csv
--rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/telefone.py
--rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.4/PyFakeDados/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:11:48.051034 PyFakeDados-0.0.4/PyFakeDados.egg-info/
--rw-rw-rw-   0        0        0     3484 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 15:11:47.000000 PyFakeDados-0.0.4/PyFakeDados.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.4/README.md
--rw-rw-rw-   0        0        0      848 2023-06-30 15:11:48.064285 PyFakeDados-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.272130 PyFakeDados-0.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3484 2023-06-30 17:40:37.272130 PyFakeDados-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.246177 PyFakeDados-0.0.5/PyFakeDados/
+-rw-rw-rw-   0        0        0       21 2023-06-30 17:40:17.000000 PyFakeDados-0.0.5/PyFakeDados/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/bairro.py
+-rw-rw-rw-   0        0        0     1711 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cep.py
+-rw-rw-rw-   0        0        0     1823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cnpj.py
+-rw-rw-rw-   0        0        0     1533 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/cpf.py
+-rw-rw-rw-   0        0        0      184 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/ctps.py
+-rw-rw-rw-   0        0        0      849 2023-06-30 17:24:54.000000 PyFakeDados-0.0.5/PyFakeDados/email.py
+-rw-rw-rw-   0        0        0     3183 2023-06-30 17:37:40.000000 PyFakeDados-0.0.5/PyFakeDados/empresa.py
+-rw-rw-rw-   0        0        0     1798 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/estado.py
+-rw-rw-rw-   0        0        0      170 2023-06-29 19:04:37.000000 PyFakeDados-0.0.5/PyFakeDados/inscricao_estadual.py
+-rw-rw-rw-   0        0        0      823 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/logradouro.py
+-rw-rw-rw-   0        0        0     1417 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/municipio.py
+-rw-rw-rw-   0        0        0     3360 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/nome.py
+-rw-rw-rw-   0        0        0     2587 2023-06-30 15:10:31.000000 PyFakeDados-0.0.5/PyFakeDados/pessoa.py
+-rw-rw-rw-   0        0        0      177 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/pis.py
+-rw-rw-rw-   0        0        0      657 2023-06-30 15:02:53.000000 PyFakeDados-0.0.5/PyFakeDados/rg.py
+-rw-rw-rw-   0        0        0      400 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/senha.py
+-rw-rw-rw-   0        0        0      411 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/site.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.268529 PyFakeDados-0.0.5/PyFakeDados/src/
+-rw-rw-rw-   0        0        0     1043 2023-06-29 20:04:40.000000 PyFakeDados-0.0.5/PyFakeDados/src/estados.csv
+-rw-rw-rw-   0        0        0   358545 2023-06-29 20:09:31.000000 PyFakeDados-0.0.5/PyFakeDados/src/municipios.csv
+-rw-rw-rw-   0        0        0     1886 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/telefone.py
+-rw-rw-rw-   0        0        0     2145 2023-06-30 11:15:54.000000 PyFakeDados-0.0.5/PyFakeDados/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 17:40:37.267058 PyFakeDados-0.0.5/PyFakeDados.egg-info/
+-rw-rw-rw-   0        0        0     3484 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      759 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 13:11:38.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 17:40:37.000000 PyFakeDados-0.0.5/PyFakeDados.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2841 2023-06-30 15:02:58.000000 PyFakeDados-0.0.5/README.md
+-rw-rw-rw-   0        0        0      848 2023-06-30 17:40:37.274549 PyFakeDados-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-29 17:33:57.000000 PyFakeDados-0.0.5/setup.py
```

### Comparing `PyFakeDados-0.0.4/LICENSE.txt` & `PyFakeDados-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PKG-INFO` & `PyFakeDados-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.4/PyFakeDados/bairro.py` & `PyFakeDados-0.0.5/PyFakeDados/bairro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/cep.py` & `PyFakeDados-0.0.5/PyFakeDados/cep.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/cnpj.py` & `PyFakeDados-0.0.5/PyFakeDados/cnpj.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/cpf.py` & `PyFakeDados-0.0.5/PyFakeDados/cpf.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/email.py` & `PyFakeDados-0.0.5/PyFakeDados/email.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     nome = remover_acentos(nome)
     nome = nome.lower().replace(" ", "")
     dominio = random.choice(dominios)
     email = f'{nome}@{nome}.{dominio}'
     return email
 
 def gerar_email_empresa(nome):
-    nome = remover_acentos(nome)
-    nome = nome.lower().replace(" ", "")
+    nome = ''.join(f"{i}" for i in nome.split()[:-1])
+    nome = remover_acentos(nome).lower().replace(" ", "")
     provedor = nome
     dominio = random.choice(dominios)
     email = f'contato@{nome}.{dominio}'
     return email
 
 def gerar_email_pessoa(nome):
     nome = remover_acentos(nome)
```

### Comparing `PyFakeDados-0.0.4/PyFakeDados/empresa.py` & `PyFakeDados-0.0.5/PyFakeDados/empresa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import random
 from PyFakeDados.cep import gerar_cep
 from PyFakeDados.estado import gerar_estado, gerar_uf, busca_nome_uf
 from PyFakeDados.municipio import gerar_municipio
 from PyFakeDados.bairro import gerar_bairro
 from PyFakeDados.logradouro import gerar_logradouro, gerar_numero
 from PyFakeDados.telefone import gerar_telefone_fixo, gerar_telefone_celular
-from PyFakeDados.email import gerar_email
+from PyFakeDados.email import gerar_email_empresa
 from PyFakeDados.site import gerar_site
 from PyFakeDados.cnpj import gerar_cnpj
-from PyFakeDados.inscricao_estudal import gerar_inscricao_estadual
+from PyFakeDados.inscricao_estadual import gerar_inscricao_estadual
 from PyFakeDados.utils import gerar_data
 from PyFakeDados.pessoa import gerar_pessoa
 
 LISTA_SEGMENTOS = ['Consultoria', 'Indústria', 'Comércio', 'Energia', 'Engenharia', 'Logística',
                    'Transportadora', 'Agro', 'Farmacêutica', 'Cerâmica', 'Madeireira', 'Marcenaria', 'Construtora', 'Metalurgica']
 
 
@@ -56,15 +56,15 @@
     socios = []
 
     nome = gerar_nome_empresa(segmento)
     cnpj = gerar_cnpj()
     inscricao_estadual = gerar_inscricao_estadual()
     data_abertura = gerar_data()
     site = gerar_site(nome)
-    email = gerar_email(nome)
+    email = gerar_email_empresa(nome)
     cep = gerar_cep(uf)
     endereco = gerar_logradouro()
     numero = gerar_numero()
     bairro = gerar_bairro()
     municipio = gerar_municipio(uf)
     estado = busca_nome_uf(uf)
     telefone = gerar_telefone_fixo(uf)
@@ -72,15 +72,15 @@
 
     if not nome.endswith("S.A.") and not nome.endswith("S/A") :
         socios = [gerar_pessoa() for socio in range(1, random.randint(1,5))]
 
     empresa = {
         "nome": nome,
         "cnpj": cnpj,
-        "inscricao_estudal": inscricao_estadual,
+        "inscricao_estadual": inscricao_estadual,
         "data_abertura": data_abertura.strftime("%d/%m/%Y"),
         "site": site,
         "email": email,
         "cep": cep,
         "endereco": endereco,
         "numero": numero,
         "bairro": bairro,
```

### Comparing `PyFakeDados-0.0.4/PyFakeDados/estado.py` & `PyFakeDados-0.0.5/PyFakeDados/estado.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/logradouro.py` & `PyFakeDados-0.0.5/PyFakeDados/logradouro.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/municipio.py` & `PyFakeDados-0.0.5/PyFakeDados/municipio.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/nome.py` & `PyFakeDados-0.0.5/PyFakeDados/nome.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/pessoa.py` & `PyFakeDados-0.0.5/PyFakeDados/pessoa.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/rg.py` & `PyFakeDados-0.0.5/PyFakeDados/rg.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/src/estados.csv` & `PyFakeDados-0.0.5/PyFakeDados/src/estados.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/src/municipios.csv` & `PyFakeDados-0.0.5/PyFakeDados/src/municipios.csv`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/telefone.py` & `PyFakeDados-0.0.5/PyFakeDados/telefone.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados/utils.py` & `PyFakeDados-0.0.5/PyFakeDados/utils.py`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/PyFakeDados.egg-info/PKG-INFO` & `PyFakeDados-0.0.5/PyFakeDados.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFakeDados
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generic generator fake data for application and api development.
 Home-page: https://github.com/juliansantosinfo/PyFakeDados
 Author: Julian de Almeida Santos
 Author-email: julian.santos.info@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/juliansantosinfo/PyFakeDados
 Keywords: fakedados,fake,dados,gerador,pessoa,empresa,documento
```

### Comparing `PyFakeDados-0.0.4/PyFakeDados.egg-info/SOURCES.txt` & `PyFakeDados-0.0.5/PyFakeDados.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 PyFakeDados/cep.py
 PyFakeDados/cnpj.py
 PyFakeDados/cpf.py
 PyFakeDados/ctps.py
 PyFakeDados/email.py
 PyFakeDados/empresa.py
 PyFakeDados/estado.py
-PyFakeDados/inscricao_estudal.py
+PyFakeDados/inscricao_estadual.py
 PyFakeDados/logradouro.py
 PyFakeDados/municipio.py
 PyFakeDados/nome.py
 PyFakeDados/pessoa.py
 PyFakeDados/pis.py
 PyFakeDados/rg.py
 PyFakeDados/senha.py
```

### Comparing `PyFakeDados-0.0.4/README.md` & `PyFakeDados-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PyFakeDados-0.0.4/setup.cfg` & `PyFakeDados-0.0.5/setup.cfg`

 * *Files identical despite different names*

