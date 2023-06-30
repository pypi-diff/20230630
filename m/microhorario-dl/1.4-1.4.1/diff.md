# Comparing `tmp/microhorario-dl-1.4.tar.gz` & `tmp/microhorario-dl-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microhorario-dl-1.4.tar", last modified: Thu May 25 10:39:31 2023, max compression
+gzip compressed data, was "microhorario-dl-1.4.1.tar", last modified: Fri Jun 30 14:44:28 2023, max compression
```

## Comparing `microhorario-dl-1.4.tar` & `microhorario-dl-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1074 2023-05-25 10:21:46.000000 microhorario-dl-1.4/LICENSE
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3840 2023-05-25 10:39:31.843625 microhorario-dl-1.4/PKG-INFO
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3179 2023-05-25 10:21:46.000000 microhorario-dl-1.4/README.md
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       84 2023-05-25 10:21:46.000000 microhorario-dl-1.4/pyproject.toml
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       38 2023-05-25 10:39:31.843625 microhorario-dl-1.4/setup.cfg
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1087 2023-05-25 10:37:24.000000 microhorario-dl-1.4/setup.py
-drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/
-drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/microhorario_dl/
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8114 2023-05-25 10:37:24.000000 microhorario-dl-1.4/src/microhorario_dl/__init__.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     6882 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/consultas.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1419 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/ementa.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1660 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/exceptions.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8357 2023-05-25 10:31:47.000000 microhorario-dl-1.4/src/microhorario_dl/models.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3833 2023-05-25 10:34:26.000000 microhorario-dl-1.4/src/microhorario_dl/parser.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1004 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/payloads.py
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      615 2023-05-25 10:21:46.000000 microhorario-dl-1.4/src/microhorario_dl/utils.py
-drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-05-25 10:39:31.843625 microhorario-dl-1.4/src/microhorario_dl.egg-info/
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3840 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/PKG-INFO
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      505 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)        1 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       30 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/requires.txt
--rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       16 2023-05-25 10:39:31.000000 microhorario-dl-1.4/src/microhorario_dl.egg-info/top_level.txt
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1074 2023-05-25 10:21:46.000000 microhorario-dl-1.4.1/LICENSE
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3842 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/PKG-INFO
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3179 2023-05-25 10:21:46.000000 microhorario-dl-1.4.1/README.md
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       84 2023-05-25 10:21:46.000000 microhorario-dl-1.4.1/pyproject.toml
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       38 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/setup.cfg
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1089 2023-06-29 13:50:47.000000 microhorario-dl-1.4.1/setup.py
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/src/
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/src/microhorario_dl/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8116 2023-06-29 13:50:47.000000 microhorario-dl-1.4.1/src/microhorario_dl/__init__.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     9087 2023-06-30 14:39:43.000000 microhorario-dl-1.4.1/src/microhorario_dl/consultas.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     1419 2023-05-25 10:21:46.000000 microhorario-dl-1.4.1/src/microhorario_dl/ementa.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     2059 2023-06-29 18:50:02.000000 microhorario-dl-1.4.1/src/microhorario_dl/exceptions.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     8357 2023-05-25 10:31:47.000000 microhorario-dl-1.4.1/src/microhorario_dl/models.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     4320 2023-06-30 14:13:07.000000 microhorario-dl-1.4.1/src/microhorario_dl/parser.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     2463 2023-06-30 14:39:43.000000 microhorario-dl-1.4.1/src/microhorario_dl/payloads.py
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      615 2023-05-25 10:21:46.000000 microhorario-dl-1.4.1/src/microhorario_dl/utils.py
+drwxrwxr-x   0 leinadium  (1000) leinadium  (1000)        0 2023-06-30 14:44:28.682526 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)     3842 2023-06-30 14:44:28.000000 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/PKG-INFO
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)      505 2023-06-30 14:44:28.000000 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/SOURCES.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)        1 2023-06-30 14:44:28.000000 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/dependency_links.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       30 2023-06-30 14:44:28.000000 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/requires.txt
+-rw-rw-r--   0 leinadium  (1000) leinadium  (1000)       16 2023-06-30 14:44:28.000000 microhorario-dl-1.4.1/src/microhorario_dl.egg-info/top_level.txt
```

### Comparing `microhorario-dl-1.4/LICENSE` & `microhorario-dl-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microhorario-dl-1.4/PKG-INFO` & `microhorario-dl-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microhorario-dl
-Version: 1.4
+Version: 1.4.1
 Summary: PUC-Rio Microhorario Downloader
 Home-page: https://github.com/Leinadium/microhorario-dl
 Author: Daniel Guimarães <github@Leinadium>
 Author-email: daniel.sch.guima@gmail.com
 Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
 Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `microhorario-dl-1.4/README.md` & `microhorario-dl-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `microhorario-dl-1.4/setup.py` & `microhorario-dl-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='microhorario-dl',
-    version='1.4',
+    version='1.4.1',
     description='PUC-Rio Microhorario Downloader',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Leinadium/microhorario-dl',
     author='Daniel Guimarães <github@Leinadium>',
     author_email='daniel.sch.guima@gmail.com',
     classifiers=[
```

### Comparing `microhorario-dl-1.4/src/microhorario_dl/__init__.py` & `microhorario-dl-1.4.1/src/microhorario_dl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 como Selenium.
 
 A ferramenta utiliza chamadas HTTP (GET e POST) para interagir
 com o microhorário e baixar todas as disciplinas
 """
 
 __author__ = "Daniel Guimarães (github.com/Leinadium)"
-__version__ = "1.4"
+__version__ = "1.4.1"
 __copyright__ = "Copyright (c) 2022 Daniel Guimarães"
 __license__ = "MIT"
 
 from time import sleep
 
 from .consultas import consulta_inicial, consulta_intermediaria, consulta_final
 from .parser import converte_para_json
```

### Comparing `microhorario-dl-1.4/src/microhorario_dl/consultas.py` & `microhorario-dl-1.4.1/src/microhorario_dl/consultas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 import requests
+from warnings import warn
 from bs4 import BeautifulSoup
 
 # typing modules
 from typing import Dict, Any, Optional, Match, Union
 from bs4.element import Tag
+from requests import Response
 
 # local modules
-from .payloads import PAYLOAD_FINAL, PAYLOAD_INTERMEDIARIO
+from .payloads import PayloadMicrohorario
 from .utils import URL_CONSULTA, URL_INICIAL, USER_AGENT, pegar_sessao_da_url
-from .exceptions import EmptyTagValueError, TagNotFoundError, NotCSVError, PatternNotFoundError
+from .exceptions import EmptyTagValueError, TagNotFoundError, NotCSVError, PatternNotFoundError, WebExceptionError
 
 
 def de_opcoes_para_dicionario(t: Tag) -> Dict[str, str]:
     """Converte todas as opções dentro de uma tag de seleção em um dicionario.
 
     Em vez de pegar o `value` da opção como chave, é feito um regex na string.
     """
@@ -24,14 +26,50 @@
             ident = m.group('ident')
             nome = m.group('nome')
             if (ident is not None) and (nome is not None):
                 ret[ident] = nome
     return ret
 
 
+def consulta_excecao(conteudo: str) -> Response:
+    """
+    Caso a primeira consulta foi redirecionada para a página de erro.
+    Caso isso tenha acontecido, tenta ver se o "Horários e Salas" está disponível.
+    Nesse caso, retorna a requisição para a página de consulta.
+    """
+    # faz o parsing do conteudo
+    soup = BeautifulSoup(conteudo, features='html.parser')
+    span_msg: Tag = soup.find(id='lblMensagem')     # pega a tag de span
+    if span_msg is None:
+        raise WebExceptionError("Exceção não possui mensagem de erro")
+
+    # coleta a tag <a> dentro do conteudo
+    tag_links_msg: list[Tag] = span_msg.find_all('a')
+    if len(tag_links_msg) == 0:
+        raise WebExceptionError("Exceção não possui link de redirecionamento")
+    tag_link_msg: Tag = tag_links_msg[0]
+
+    link_correto = tag_link_msg.get('href')
+
+    # verifica se o link é o correto
+    if link_correto is None or "WebMicroHorarioConsulta" not in link_correto:
+        raise WebExceptionError("Link de redirecionamento não é o esperado")
+
+    # altera o modo e avisa
+    PayloadMicrohorario.altera_modo()
+    warn("Microhorário indisponível, utilizando 'Horarios e Salas' como alternativa. "
+         "A quantidade de créditos e as alocações (vagas por turma) estarão indisponíveis.")
+
+    # faz a requisição para o link correto
+    return requests.get(
+        url=link_correto,
+        headers={"User-Agent": USER_AGENT}
+    )
+
+
 def consulta_inicial() -> Dict[str, Any]:
     """
     Faz a primeira consulta no site do microhorario
 
     A primeira consulta é responsável por coletar os cookies necessários,
     as variáveis para o ASP.NET, a sessão do usuário,
     e também o nome dos departamentos e destinos.
@@ -56,22 +94,27 @@
                 if valor is None:
                     raise EmptyTagValueError(nome)
                 else:
                     return valor
 
     r = requests.get(
         url=URL_INICIAL,
-        headers={"User-Agent": USER_AGENT}
+        headers={"User-Agent": USER_AGENT},
+        allow_redirects=True
     )
 
     # pegando os cookies (juntando com os redirects)
     cookies: dict = r.cookies.get_dict()
     for r_history in r.history:
         cookies.update(r_history.cookies.get_dict())
 
+    # se foi redirecionado para uma excecao, tenta acessar o link correto
+    if "WebExcecao" in r.url:
+        r = consulta_excecao(r.text)
+
     # pegando propriedades do ASP.NET
     soup = BeautifulSoup(r.text, features='html.parser')
     view_state_generator: Tag = soup.find(id='__VIEWSTATEGENERATOR')
     event_validation: Tag = soup.find(id='__EVENTVALIDATION')
     view_state: Tag = soup.find(id='__VIEWSTATE')
 
     # pegando destinos
@@ -121,39 +164,40 @@
     """
     def regex_ou_aborta(nome: str, pattern: str, string: str) -> str:
         m: Match = re.search(pattern, string)
         if m is None:
             raise PatternNotFoundError(nome=nome, regex=pattern)
         return m.group(1)
 
-    payload: dict = PAYLOAD_INTERMEDIARIO
+    payload: dict = PayloadMicrohorario.intermediario()
     payload.update(dados_iniciais['dados'])     # adiciona as variaveis coletadas no dados iniciais
 
     cookies = dados_iniciais.get('cookies')
     sessao = dados_iniciais.get('sessao')
 
     r = requests.post(
         url=URL_CONSULTA,
         cookies=cookies,
         params={'sessao': sessao},
         headers={
             'User-Agent': USER_AGENT,
             'Accept': 'text/plain',
-            'Content-Type': 'application/x-www-form-urlencoded'
+            'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8',
+            'Origin': "http://microhorario.rdc.puc-rio.br",     # noqa
         },
         data=payload
     )
 
     # pegando as novas informacoes
     return {
         'cookies': cookies,
         'sessao': sessao,
         'dados': {
             '__VIEWSTATEGENERATOR': regex_ou_aborta(
-                nome='',
+                nome='VIEWSTATEGENERATOR',
                 pattern=r'__VIEWSTATEGENERATOR\|([0-9a-zA-Z+\/=]+)\|',
                 string=r.text
             ),
             '__EVENTVALIDATION': regex_ou_aborta(
                 nome='EVENTVALIDATION',
                 pattern=r'__EVENTVALIDATION\|([0-9a-zA-Z+\/=]+)\|',
                 string=r.text
@@ -163,40 +207,46 @@
                 pattern=r'__VIEWSTATE\|([0-9a-zA-Z+\/=]+)\|',
                 string=r.text
             )
         }
     }
 
 
-def consulta_final(dados_intermediarios: Dict[str, Union[Tag, str]]) -> str:
+def consulta_final(dados_intermediarios: Dict[str, Union[Tag, str, dict]]) -> str:
     """
     Faz a consulta final, para obter o CSV com todas as disciplinas no microhorario.
 
     Usando as variáveis de ASP.NET fornecidas na consulta intermediaria, é feito um POST
     pedindo o CSV referente àquela consulta.
 
     :param dados_intermediarios: dados da consulta intermediaria
 
     :return: o texto do csv baixado
     """
     # preparando os dados
-    payload: dict = PAYLOAD_FINAL
+    payload: dict = PayloadMicrohorario.final()
     payload.update(dados_intermediarios.get('dados'))     # adiciona as variaveis coletadas no dados iniciais
 
     cookies = dados_intermediarios.get('cookies')
     sessao = dados_intermediarios.get('sessao')
 
     # preparando a consulta
     r = requests.post(
         url=URL_CONSULTA,
         cookies=cookies,
         headers={
+            'Host': "microhorario.rdc.puc-rio.br",
             'User-Agent': USER_AGENT,
-            'Accept': 'text/csv',
-            'Content-Type': 'application/x-www-form-urlencoded'
+            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8',
+            'Accept-Language': "en-US,en;q=0.5",
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Origin': "http://microhorario.rdc.puc-rio.br",  # noqa
+            'Connection': 'keep-alive',
+            'Referer': f"{URL_CONSULTA}?sessao={sessao}",
+            'Upgrade-Insecure-Requests': '1',
         },
         params={'sessao': sessao},
         data=payload
     )
 
     if 'text/csv' not in r.headers.get('Content-Type'):
         raise NotCSVError
```

### Comparing `microhorario-dl-1.4/src/microhorario_dl/ementa.py` & `microhorario-dl-1.4.1/src/microhorario_dl/ementa.py`

 * *Files identical despite different names*

### Comparing `microhorario-dl-1.4/src/microhorario_dl/exceptions.py` & `microhorario-dl-1.4.1/src/microhorario_dl/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Attributes:
         tag -- Nome da tag não encontrada
     """
 
     def __init__(self, tag: str):
         self.tag = tag
-        super().__init__(f'Tag {tag} não encontrada' % tag)
+        super().__init__(f'Tag {tag} não encontrada')
 
 
 class EmptyTagValueError(BaseParsingError):
     """Excecção levantada quando a tag HTML não tem `value` configurada
 
     Attributes:
         tag -- Nome da tag sem `value`
@@ -58,7 +58,19 @@
     headers ou o payload da consulta estão incorretos.
     """
 
     def __init__(self):
         super().__init__("Consulta final não retornou um CSV")
 
 
+class WebExceptionError(BaseParsingError):
+    """Exceção levantada quando a consulta inicial
+    retorna uma página de erro.
+
+    Isso pode acontecer quando os
+    headers ou o payload da consulta estão incorretos.
+    """
+
+    def __init__(self, mensagem: str = ""):
+        if not mensagem:
+            mensagem = "Primeira consulta retornou uma página de erro"
+        super().__init__(mensagem)
```

### Comparing `microhorario-dl-1.4/src/microhorario_dl/models.py` & `microhorario-dl-1.4.1/src/microhorario_dl/models.py`

 * *Files identical despite different names*

### Comparing `microhorario-dl-1.4/src/microhorario_dl/parser.py` & `microhorario-dl-1.4.1/src/microhorario_dl/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,19 +68,28 @@
     for linha in linhas:
         if re_disciplina.match(linha) is None:
             continue     # pula a linha que nao tem informacao
 
         # splitando em brancos e retirando tambem o ';' final se tiver
         linha_split = linha.strip(' \n\r;').split(';')
 
+        if len(linha_split) == 11:
+            # caso especifico quando cai no Horarios e Salas (microhorario desligado)
+            # nao existe a linha de 'créditos', 'destino' e 'vaga'
+            linha_split.insert(3, '-1')     # creditos
+            linha_split.insert(5, '--')     # destino
+            linha_split.insert(6, '--')     # vaga
+
         if len(linha_split) == 14:
-            linha_split.pop(11)    # removendo horas de extensao
+            # removendo horas de extensao (atualização nova do microhorario)
+            linha_split.pop(11)
 
         if len(linha_split) != 13:
-            warnings.warn(f"Linha iniciada em {linha_split[0]} está inválida")
+            warnings.warn(f"Linha iniciada em {linha_split[0]} está inválida: contém {len(linha_split)} elementos,"
+                          f"esperado: 14, 13 ou 11")
             continue     # pula a linha que a informacao esta corrompida
 
         codigo = linha_split[0].strip()
         nome = linha_split[1].strip()
         professor = linha_split[2].strip()
         creditos = linha_split[3].strip()
         turma = linha_split[4].strip()
```

### Comparing `microhorario-dl-1.4/src/microhorario_dl/utils.py` & `microhorario-dl-1.4.1/src/microhorario_dl/utils.py`

 * *Files identical despite different names*

### Comparing `microhorario-dl-1.4/src/microhorario_dl.egg-info/PKG-INFO` & `microhorario-dl-1.4.1/src/microhorario_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microhorario-dl
-Version: 1.4
+Version: 1.4.1
 Summary: PUC-Rio Microhorario Downloader
 Home-page: https://github.com/Leinadium/microhorario-dl
 Author: Daniel Guimarães <github@Leinadium>
 Author-email: daniel.sch.guima@gmail.com
 Project-URL: Bug Reports, https://github.com/Leinadium/microhorario-dl/issues
 Project-URL: Source, https://github.com/Leinadium/microhorario-dl/
 Classifier: Development Status :: 3 - Alpha
```

