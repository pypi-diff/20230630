# Comparing `tmp/python-aternos-3.0.0.tar.gz` & `tmp/python-aternos-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aternos-3.0.0.tar", last modified: Mon May 29 08:07:34 2023, max compression
+gzip compressed data, was "python-aternos-3.0.1.tar", last modified: Fri Jun 30 06:55:05 2023, max compression
```

## Comparing `python-aternos-3.0.0.tar` & `python-aternos-3.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.0/LICENSE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.0/NOTICE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7311 2023-05-29 08:07:34.706738 python-aternos-3.0.0/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6137 2023-05-29 08:02:27.000000 python-aternos-3.0.0/README.md
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.0/pyproject.toml
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/python_aternos/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.0/python_aternos/__init__.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.0/python_aternos/ataccount.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6857 2023-05-29 08:06:11.000000 python-aternos-3.0.0/python_aternos/atclient.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.0/python_aternos/atconf.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8868 2023-05-24 17:02:08.000000 python-aternos-3.0.0/python_aternos/atconnect.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.0/python_aternos/aterrors.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.0/python_aternos/atfile.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.0/python_aternos/atfm.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5800 2023-05-24 17:02:44.000000 python-aternos-3.0.0/python_aternos/atjsparse.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.0/python_aternos/atlog.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.0/python_aternos/atmd5.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3311 2023-05-24 15:57:21.000000 python-aternos-3.0.0/python_aternos/atplayers.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.0/python_aternos/atserver.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9942 2023-05-24 15:57:36.000000 python-aternos-3.0.0/python_aternos/atwss.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/python_aternos.egg-info/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7311 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/SOURCES.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/dependency_links.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       79 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/requires.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/top_level.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-05-29 08:07:34.706738 python-aternos-3.0.0/setup.cfg
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     1626 2023-05-29 08:05:32.000000 python-aternos-3.0.0/setup.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/tests/
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.0/tests/test_http.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.0/tests/test_js2py.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.0/tests/test_jsnode.py
--rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.0/tests/test_login.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.1/LICENSE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.1/NOTICE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7161 2023-06-30 06:55:05.988202 python-aternos-3.0.1/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5925 2023-06-30 05:54:30.000000 python-aternos-3.0.1/README.md
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.1/pyproject.toml
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/python_aternos/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.1/python_aternos/__init__.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.1/python_aternos/ataccount.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6926 2023-06-30 05:54:30.000000 python-aternos-3.0.1/python_aternos/atclient.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.1/python_aternos/atconf.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8889 2023-06-30 06:02:26.000000 python-aternos-3.0.1/python_aternos/atconnect.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.1/python_aternos/aterrors.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.1/python_aternos/atfile.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.1/python_aternos/atfm.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5849 2023-06-30 06:20:51.000000 python-aternos-3.0.1/python_aternos/atjsparse.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.1/python_aternos/atlog.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.1/python_aternos/atmd5.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3311 2023-05-24 15:57:21.000000 python-aternos-3.0.1/python_aternos/atplayers.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.1/python_aternos/atserver.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9974 2023-06-30 06:36:36.000000 python-aternos-3.0.1/python_aternos/atwss.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/python_aternos.egg-info/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7161 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/SOURCES.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/dependency_links.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      254 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/requires.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-06-30 06:55:05.000000 python-aternos-3.0.1/python_aternos.egg-info/top_level.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-06-30 06:55:05.988202 python-aternos-3.0.1/setup.cfg
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2043 2023-06-30 06:54:38.000000 python-aternos-3.0.1/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-06-30 06:55:05.988202 python-aternos-3.0.1/tests/
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.1/tests/test_http.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.1/tests/test_js2py.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.1/tests/test_jsnode.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.1/tests/test_login.py
```

### Comparing `python-aternos-3.0.0/LICENSE` & `python-aternos-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/NOTICE` & `python-aternos-3.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/PKG-INFO` & `python-aternos-3.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.0
+Version: 3.0.1
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -20,14 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: pypi
+Provides-Extra: docs
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <img src="https://i.ibb.co/3RXcXJ1/aternos-400.png" alt="Python Aternos Logo">
     <h1>
         Python Aternos
@@ -47,39 +50,38 @@
         </div>
     </h1>
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
+> **WARNING**
+>
+> Recently, Aternos started somehow detecting
+> API requests from this library.
+> Any automated access is prohibited according
+> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**.
+>
+> **USE AT YOUR OWN RISK**
+>
+> I will try to fix that as soon as possible.
+
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
  - Parsing server info by its ID
  - Starting/stoping server, restarting, confirming/cancelling launch
  - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
  - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
-> **Warning**
->
-> According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access,
-> beacuse they don't receive money from advertisting in this case.
->
-> I always try to hide automated python-aternos requests
-> using browser-specific headers/cookies,  
-> but you should make backups to restore your world
-> if Aternos detects violation of ToS and bans your account
-> (view issues [#16](https://github.com/DarkCat09/python-aternos/issues/16)
-> and [#46](https://github.com/DarkCat09/python-aternos/issues/46)).
-
 ## Install
 
 ### Common
 ```bash
 $ pip install python-aternos
 ```
 > **Note** for Windows users
@@ -104,25 +106,28 @@
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
 # Create object
-aternos = Client()
+atclient = Client()
 
 # Log in
 # with username and password
-aternos.login('example', 'test123')
+atclient.login('example', 'test123')
 # ----OR----
 # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+atclient.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
 # with session cookie
-aternos.login_with_session('ATERNOS_SESSION cookie value')
+atclient.login_with_session('ATERNOS_SESSION cookie value')
+
+# Get AternosAccount object
+aternos = atclient.account
 
 # Get servers list
 servs = aternos.list_servers()
 
 # Get the first server
 myserv = servs[0]
```

#### html2text {}

```diff
@@ -1,82 +1,81 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.0 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.1 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 :: Linux Classifier: Operating System :: MacOS Classifier: Intended Audience ::
 Developers Classifier: Topic :: Internet Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
-License-File: NOTICE
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
+Provides-Extra: pypi Provides-Extra: docs License-File: LICENSE License-File:
+NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
-- Saving session to the file and restoring - Changing username, email and
+aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
+Aternos started somehow detecting > API requests from this library. > Any
+automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
+/aternos.gmbh/en/aternos/terms#:~:
+text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
+to fix that as soon as possible. Python Aternos supports: - Logging in to
+account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
+Saving session to the file and restoring - Changing username, email and
 password - Parsing Minecraft servers list - Parsing server info by its ID -
 Starting/stoping server, restarting, confirming/cancelling launch - Updating
 server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
-Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
-> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
-aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access, > beacuse they
-don't receive money from advertisting in this case. > > I always try to hide
-automated python-aternos requests > using browser-specific headers/cookies, >
-but you should make backups to restore your world > if Aternos detects
-violation of ToS and bans your account > (view issues [#16](https://github.com/
-DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
-python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
-aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
-(https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
-it, and then execute: > `pip install --no-deps python-aternos` ### Development
-```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
-python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or its MD5
-hash. Then request the servers list using `list_servers()`. You can start/stop
-your Aternos server, calling `start()` or `stop()`. Here is an example how to
-use the API: ```python # Import from python_aternos import Client # Create
-object aternos = Client() # Log in # with username and password aternos.login
-('example', 'test123') # ----OR---- # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
-value') # Get servers list servs = aternos.list_servers() # Get the first
-server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
-also find server by IP testserv = None for serv in servs: if serv.address ==
-'test.aternos.org': testserv = serv if testserv is not None: # Prints the
-server software and its version # (for example, "Vanilla 1.12.2") print
-(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
-[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
-## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
-aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
-------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
-configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
-new Aternos security methods. Huge thanks to [lusm554](https://github.com/
-lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
-to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
-versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
-changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
-DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
-parser.| |v2.0.x|Documentation, automatically saving/restoring session,
-improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
-(including cookie refreshing fix). Support for captcha solving services (view
-[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
-interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+Managing files, settings, players (whitelist, operators, etc.) ## Install ###
+Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
+> Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
+pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
+install --no-deps python-aternos` ### Development ```bash $ git clone https://
+github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
+``` ## Usage To use Aternos API in your Python script, import it and login with
+your username and password or its MD5 hash. Then request the servers list using
+`list_servers()`. You can start/stop your Aternos server, calling `start()` or
+`stop()`. Here is an example how to use the API: ```python # Import from
+python_aternos import Client # Create object atclient = Client() # Log in #
+with username and password atclient.login('example', 'test123') # ----OR---- #
+with username and MD5 hashed password atclient.login_hashed('example',
+'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
+atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
+AternosAccount object aternos = atclient.account # Get servers list servs =
+aternos.list_servers() # Get the first server myserv = servs[0] # Start
+myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
+None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
+if testserv is not None: # Prints the server software and its version # (for
+example, "Vanilla 1.12.2") print(testserv.software, testserv.version) # Starts
+server testserv.start() ``` ## [More examples](https://github.com/DarkCat09/
+python-aternos/tree/main/examples) ## [Documentation](https://aternos.dc09.ru)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth) ## Changelog
+|Version|Description | |:-----:|:-----------| |v0.3|Implemented files API,
+added typization.| |v0.4|Implemented configuration API, some bugfixes.|
+|v0.5|The API was updated corresponding to new Aternos security methods. Huge
+thanks to [lusm554](https://github.com/lusm554).| |**v0.6/v1.0.0**|Code
+refactoring, websockets API and session saving to prevent detecting automation
+access.| |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
+|v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
+|**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-
+aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
+|v2.0.x|Documentation, automatically saving/restoring session, improvements in
+Files API.| |v2.1.x|Fixes in websockets API, atconnect (including cookie
+refreshing fix). Support for captcha solving services (view [#52](https://
+github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS interpreter
+support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
 implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
 backups.| ## Reversed API Specification Private Aternos API requests were
 captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
 main/aternos.har) and were imported to [a Postman Workspace](https://
 www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
 explore the API. Any help with improving this library is welcome. ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
```

### Comparing `python-aternos-3.0.0/README.md` & `python-aternos-3.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,39 +18,38 @@
         </div>
     </h1>
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
+> **WARNING**
+>
+> Recently, Aternos started somehow detecting
+> API requests from this library.
+> Any automated access is prohibited according
+> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**.
+>
+> **USE AT YOUR OWN RISK**
+>
+> I will try to fix that as soon as possible.
+
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
  - Parsing server info by its ID
  - Starting/stoping server, restarting, confirming/cancelling launch
  - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
  - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
-> **Warning**
->
-> According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access,
-> beacuse they don't receive money from advertisting in this case.
->
-> I always try to hide automated python-aternos requests
-> using browser-specific headers/cookies,  
-> but you should make backups to restore your world
-> if Aternos detects violation of ToS and bans your account
-> (view issues [#16](https://github.com/DarkCat09/python-aternos/issues/16)
-> and [#46](https://github.com/DarkCat09/python-aternos/issues/46)).
-
 ## Install
 
 ### Common
 ```bash
 $ pip install python-aternos
 ```
 > **Note** for Windows users
@@ -75,25 +74,28 @@
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
 # Create object
-aternos = Client()
+atclient = Client()
 
 # Log in
 # with username and password
-aternos.login('example', 'test123')
+atclient.login('example', 'test123')
 # ----OR----
 # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+atclient.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
 # with session cookie
-aternos.login_with_session('ATERNOS_SESSION cookie value')
+atclient.login_with_session('ATERNOS_SESSION cookie value')
+
+# Get AternosAccount object
+aternos = atclient.account
 
 # Get servers list
 servs = aternos.list_servers()
 
 # Get the first server
 myserv = servs[0]
```

#### html2text {}

```diff
@@ -1,66 +1,64 @@
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
-- Saving session to the file and restoring - Changing username, email and
+aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
+Aternos started somehow detecting > API requests from this library. > Any
+automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
+/aternos.gmbh/en/aternos/terms#:~:
+text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
+to fix that as soon as possible. Python Aternos supports: - Logging in to
+account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
+Saving session to the file and restoring - Changing username, email and
 password - Parsing Minecraft servers list - Parsing server info by its ID -
 Starting/stoping server, restarting, confirming/cancelling launch - Updating
 server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
-Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
-> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
-aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access, > beacuse they
-don't receive money from advertisting in this case. > > I always try to hide
-automated python-aternos requests > using browser-specific headers/cookies, >
-but you should make backups to restore your world > if Aternos detects
-violation of ToS and bans your account > (view issues [#16](https://github.com/
-DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
-python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
-aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
-(https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
-it, and then execute: > `pip install --no-deps python-aternos` ### Development
-```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
-python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or its MD5
-hash. Then request the servers list using `list_servers()`. You can start/stop
-your Aternos server, calling `start()` or `stop()`. Here is an example how to
-use the API: ```python # Import from python_aternos import Client # Create
-object aternos = Client() # Log in # with username and password aternos.login
-('example', 'test123') # ----OR---- # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
-value') # Get servers list servs = aternos.list_servers() # Get the first
-server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
-also find server by IP testserv = None for serv in servs: if serv.address ==
-'test.aternos.org': testserv = serv if testserv is not None: # Prints the
-server software and its version # (for example, "Vanilla 1.12.2") print
-(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
-[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
-## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
-aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
-------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
-configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
-new Aternos security methods. Huge thanks to [lusm554](https://github.com/
-lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
-to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
-versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
-changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
-DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
-parser.| |v2.0.x|Documentation, automatically saving/restoring session,
-improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
-(including cookie refreshing fix). Support for captcha solving services (view
-[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
-interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+Managing files, settings, players (whitelist, operators, etc.) ## Install ###
+Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
+> Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
+pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
+install --no-deps python-aternos` ### Development ```bash $ git clone https://
+github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
+``` ## Usage To use Aternos API in your Python script, import it and login with
+your username and password or its MD5 hash. Then request the servers list using
+`list_servers()`. You can start/stop your Aternos server, calling `start()` or
+`stop()`. Here is an example how to use the API: ```python # Import from
+python_aternos import Client # Create object atclient = Client() # Log in #
+with username and password atclient.login('example', 'test123') # ----OR---- #
+with username and MD5 hashed password atclient.login_hashed('example',
+'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
+atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
+AternosAccount object aternos = atclient.account # Get servers list servs =
+aternos.list_servers() # Get the first server myserv = servs[0] # Start
+myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
+None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
+if testserv is not None: # Prints the server software and its version # (for
+example, "Vanilla 1.12.2") print(testserv.software, testserv.version) # Starts
+server testserv.start() ``` ## [More examples](https://github.com/DarkCat09/
+python-aternos/tree/main/examples) ## [Documentation](https://aternos.dc09.ru)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth) ## Changelog
+|Version|Description | |:-----:|:-----------| |v0.3|Implemented files API,
+added typization.| |v0.4|Implemented configuration API, some bugfixes.|
+|v0.5|The API was updated corresponding to new Aternos security methods. Huge
+thanks to [lusm554](https://github.com/lusm554).| |**v0.6/v1.0.0**|Code
+refactoring, websockets API and session saving to prevent detecting automation
+access.| |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
+|v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
+|**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-
+aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
+|v2.0.x|Documentation, automatically saving/restoring session, improvements in
+Files API.| |v2.1.x|Fixes in websockets API, atconnect (including cookie
+refreshing fix). Support for captcha solving services (view [#52](https://
+github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS interpreter
+support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
 implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
 backups.| ## Reversed API Specification Private Aternos API requests were
 captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
 main/aternos.har) and were imported to [a Postman Workspace](https://
 www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
 explore the API. Any help with improving this library is welcome. ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
```

### Comparing `python-aternos-3.0.0/python_aternos/ataccount.py` & `python-aternos-3.0.1/python_aternos/ataccount.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atclient.py` & `python-aternos-3.0.1/python_aternos/atclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
     def login_with_session(self, session: str) -> None:
         """Log in using ATERNOS_SESSION cookie
 
         Args:
             session (str): Session cookie value
         """
 
+        self.atconn.parse_token()
+        self.atconn.generate_sec()
         self.atconn.session.cookies['ATERNOS_SESSION'] = session
 
     def logout(self) -> None:
         """Log out from the Aternos account"""
 
         self.atconn.request_cloudflare(
             f'{AJAX_URL}/account/logout',
```

### Comparing `python-aternos-3.0.0/python_aternos/atconf.py` & `python-aternos-3.0.1/python_aternos/atconf.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atconnect.py` & `python-aternos-3.0.1/python_aternos/atconnect.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 
 class AternosConnect:
     """Class for sending API requests,
     bypassing Cloudflare and parsing responses"""
 
     def __init__(self) -> None:
 
-        self.cf_init = partial(CloudScraper)
-        self.session = self.cf_init()
+        self.session = CloudScraper()
         self.sec = ''
         self.token = ''
         self.atcookie = ''
 
     def refresh_session(self) -> None:
         """Creates a new CloudScraper
         session object and copies all cookies.
         Required for bypassing Cloudflare"""
 
         old_cookies = self.session.cookies
-        self.session = self.cf_init()
+        captcha_kwarg = self.session.captcha
+        self.session = CloudScraper(captcha=captcha_kwarg)
         self.session.cookies.update(old_cookies)
         del old_cookies
 
     def parse_token(self) -> str:
         """Parses Aternos ajax token that
         is needed for most requests
```

### Comparing `python-aternos-3.0.0/python_aternos/aterrors.py` & `python-aternos-3.0.1/python_aternos/aterrors.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atfile.py` & `python-aternos-3.0.1/python_aternos/atfile.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atfm.py` & `python-aternos-3.0.1/python_aternos/atfm.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atjsparse.py` & `python-aternos-3.0.1/python_aternos/atjsparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,19 +131,23 @@
     def __init__(self) -> None:
         """Js2Py interpreter,
         uses js2py library to execute code"""
 
         super().__init__()
 
         ctx = js2py.EvalJs({'atob': atob})
-        ctx.execute('window.document = { };')
-        ctx.execute('window.Map = function(_i){ };')
-        ctx.execute('window.setTimeout = function(_f,_t){ };')
-        ctx.execute('window.setInterval = function(_f,_t){ };')
-        ctx.execute('window.encodeURIComponent = function(_s){ };')
+        ctx.execute('''
+        window.Map = function(_i){ };
+        window.setTimeout = function(_f,_t){ };
+        window.setInterval = function(_f,_t){ };
+        window.encodeURIComponent = function(_s){ };
+        window.document = { };
+        document.doctype = { };
+        document.getElementById = function(_s){ };
+        ''')
 
         self.ctx = ctx
 
     def exec_js(self, func: str) -> None:
         self.ctx.execute(self.to_ecma5(func))
 
     def get_var(self, name: str) -> Any:
```

### Comparing `python-aternos-3.0.0/python_aternos/atlog.py` & `python-aternos-3.0.1/python_aternos/atlog.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atplayers.py` & `python-aternos-3.0.1/python_aternos/atplayers.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atserver.py` & `python-aternos-3.0.1/python_aternos/atserver.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/python_aternos/atwss.py` & `python-aternos-3.0.1/python_aternos/atwss.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
 
 OneArgT = Callable[[Any], Coroutine[Any, Any, None]]
 TwoArgT = Callable[[Any, Tuple[Any, ...]], Coroutine[Any, Any, None]]
-FunctionT = Union[OneArgT, TwoArgT]
+FunctionT = Union[OneArgT, TwoArgT]  # pylint: disable=invalid-name
 ArgsTuple = Tuple[FunctionT, Tuple[Any, ...]]
 
 
 class Streams(enum.Enum):
 
     """WebSocket streams types"""
```

### Comparing `python-aternos-3.0.0/python_aternos.egg-info/PKG-INFO` & `python-aternos-3.0.1/python_aternos.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 3.0.0
+Version: 3.0.1
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -20,14 +20,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: pypi
+Provides-Extra: docs
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <img src="https://i.ibb.co/3RXcXJ1/aternos-400.png" alt="Python Aternos Logo">
     <h1>
         Python Aternos
@@ -47,39 +50,38 @@
         </div>
     </h1>
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
+> **WARNING**
+>
+> Recently, Aternos started somehow detecting
+> API requests from this library.
+> Any automated access is prohibited according
+> to [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**.
+>
+> **USE AT YOUR OWN RISK**
+>
+> I will try to fix that as soon as possible.
+
 Python Aternos supports:
 
  - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
  - Saving session to the file and restoring
  - Changing username, email and password
  - Parsing Minecraft servers list
  - Parsing server info by its ID
  - Starting/stoping server, restarting, confirming/cancelling launch
  - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
  - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
-> **Warning**
->
-> According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access,
-> beacuse they don't receive money from advertisting in this case.
->
-> I always try to hide automated python-aternos requests
-> using browser-specific headers/cookies,  
-> but you should make backups to restore your world
-> if Aternos detects violation of ToS and bans your account
-> (view issues [#16](https://github.com/DarkCat09/python-aternos/issues/16)
-> and [#46](https://github.com/DarkCat09/python-aternos/issues/46)).
-
 ## Install
 
 ### Common
 ```bash
 $ pip install python-aternos
 ```
 > **Note** for Windows users
@@ -104,25 +106,28 @@
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
 # Create object
-aternos = Client()
+atclient = Client()
 
 # Log in
 # with username and password
-aternos.login('example', 'test123')
+atclient.login('example', 'test123')
 # ----OR----
 # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+atclient.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
 # with session cookie
-aternos.login_with_session('ATERNOS_SESSION cookie value')
+atclient.login_with_session('ATERNOS_SESSION cookie value')
+
+# Get AternosAccount object
+aternos = atclient.account
 
 # Get servers list
 servs = aternos.list_servers()
 
 # Get the first server
 myserv = servs[0]
```

#### html2text {}

```diff
@@ -1,82 +1,81 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 3.0.0 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.1 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 :: Linux Classifier: Operating System :: MacOS Classifier: Intended Audience ::
 Developers Classifier: Topic :: Internet Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
-License-File: NOTICE
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: dev
+Provides-Extra: pypi Provides-Extra: docs License-File: LICENSE License-File:
+NOTICE
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
-aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
-- Saving session to the file and restoring - Changing username, email and
+aternos.org/)' private API and html parsing. > **WARNING** > > Recently,
+Aternos started somehow detecting > API requests from this library. > Any
+automated access is prohibited according > to [Terms of Service Â§5.2e](https:/
+/aternos.gmbh/en/aternos/terms#:~:
+text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
+> and results in **permanent ban**. > > **USE AT YOUR OWN RISK** > > I will try
+to fix that as soon as possible. Python Aternos supports: - Logging in to
+account with password (plain or hashed) or `ATERNOS_SESSION` cookie value -
+Saving session to the file and restoring - Changing username, email and
 password - Parsing Minecraft servers list - Parsing server info by its ID -
 Starting/stoping server, restarting, confirming/cancelling launch - Updating
 server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
 websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
-Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
-> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
-aternos/terms#:~:
-text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
-> you must not use any software or APIs for automated access, > beacuse they
-don't receive money from advertisting in this case. > > I always try to hide
-automated python-aternos requests > using browser-specific headers/cookies, >
-but you should make backups to restore your world > if Aternos detects
-violation of ToS and bans your account > (view issues [#16](https://github.com/
-DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
-python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
-aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
-(https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
-it, and then execute: > `pip install --no-deps python-aternos` ### Development
-```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
-python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or its MD5
-hash. Then request the servers list using `list_servers()`. You can start/stop
-your Aternos server, calling `start()` or `stop()`. Here is an example how to
-use the API: ```python # Import from python_aternos import Client # Create
-object aternos = Client() # Log in # with username and password aternos.login
-('example', 'test123') # ----OR---- # with username and MD5 hashed password
-aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
-value') # Get servers list servs = aternos.list_servers() # Get the first
-server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
-also find server by IP testserv = None for serv in servs: if serv.address ==
-'test.aternos.org': testserv = serv if testserv is not None: # Prints the
-server software and its version # (for example, "Vanilla 1.12.2") print
-(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
-[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
-## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
-aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
-------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
-configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
-new Aternos security methods. Huge thanks to [lusm554](https://github.com/
-lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
-to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
-versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
-changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
-DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
-parser.| |v2.0.x|Documentation, automatically saving/restoring session,
-improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
-(including cookie refreshing fix). Support for captcha solving services (view
-[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
-interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+Managing files, settings, players (whitelist, operators, etc.) ## Install ###
+Common ```bash $ pip install python-aternos ``` > **Note** for Windows users >
+> Install `lxml` package from [here](https://www.lfd.uci.edu/~gohlke/
+pythonlibs/#lxml) > if you have problems with it, and then execute: > `pip
+install --no-deps python-aternos` ### Development ```bash $ git clone https://
+github.com/DarkCat09/python-aternos.git $ cd python-aternos $ pip install -e .
+``` ## Usage To use Aternos API in your Python script, import it and login with
+your username and password or its MD5 hash. Then request the servers list using
+`list_servers()`. You can start/stop your Aternos server, calling `start()` or
+`stop()`. Here is an example how to use the API: ```python # Import from
+python_aternos import Client # Create object atclient = Client() # Log in #
+with username and password atclient.login('example', 'test123') # ----OR---- #
+with username and MD5 hashed password atclient.login_hashed('example',
+'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---- # with session cookie
+atclient.login_with_session('ATERNOS_SESSION cookie value') # Get
+AternosAccount object aternos = atclient.account # Get servers list servs =
+aternos.list_servers() # Get the first server myserv = servs[0] # Start
+myserv.start() # Stop myserv.stop() # You can also find server by IP testserv =
+None for serv in servs: if serv.address == 'test.aternos.org': testserv = serv
+if testserv is not None: # Prints the server software and its version # (for
+example, "Vanilla 1.12.2") print(testserv.software, testserv.version) # Starts
+server testserv.start() ``` ## [More examples](https://github.com/DarkCat09/
+python-aternos/tree/main/examples) ## [Documentation](https://aternos.dc09.ru)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth) ## Changelog
+|Version|Description | |:-----:|:-----------| |v0.3|Implemented files API,
+added typization.| |v0.4|Implemented configuration API, some bugfixes.|
+|v0.5|The API was updated corresponding to new Aternos security methods. Huge
+thanks to [lusm554](https://github.com/lusm554).| |**v0.6/v1.0.0**|Code
+refactoring, websockets API and session saving to prevent detecting automation
+access.| |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
+|v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
+|**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-
+aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
+|v2.0.x|Documentation, automatically saving/restoring session, improvements in
+Files API.| |v2.1.x|Fixes in websockets API, atconnect (including cookie
+refreshing fix). Support for captcha solving services (view [#52](https://
+github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS interpreter
+support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
 implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
 backups.| ## Reversed API Specification Private Aternos API requests were
 captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
 main/aternos.har) and were imported to [a Postman Workspace](https://
 www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
 explore the API. Any help with improving this library is welcome. ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
```

### Comparing `python-aternos-3.0.0/python_aternos.egg-info/SOURCES.txt` & `python-aternos-3.0.1/python_aternos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/setup.py` & `python-aternos-3.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name='python-aternos',
-    version='3.0.0',
+    version='3.0.1',
     author='Chechkenev Andrey (@DarkCat09)',
     author_email='aacd0709@mail.ru',
     description='An unofficial Aternos API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DarkCat09/python-aternos',
     project_urls={
@@ -30,17 +30,34 @@
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Intended Audience :: Developers',
         'Topic :: Internet',
         'Typing :: Typed',
     ],
     install_requires=[
-        'lxml>=4.8.0',
-        'cloudscraper>=1.2.60',
-        'js2py>=0.71',
-        'websockets>=10.1',
-        'regex>=2022.3.15',
+        'cloudscraper==1.2.71',
+        'Js2Py==0.74',
+        'lxml==4.9.2',
+        'regex==2023.6.3',
+        'websockets==11.0.3',
     ],
+    extras_require={
+        'dev': [
+            'autopep8==2.0.2',
+            'pycodestyle==2.10.0',
+            'mypy==1.4.1',
+            'pylint==2.17.4',
+            'requests-mock==1.11.0',
+            'types-requests==2.31.0.1',
+        ],
+        'pypi': [
+            'build==0.10.0',
+            'twine==4.0.2',
+        ],
+        'docs': [
+            'mkdocs==1.4.3',
+        ]
+    },
     packages=['python_aternos'],
     python_requires=">=3.7",
     include_package_data=True,
 )
```

### Comparing `python-aternos-3.0.0/tests/test_http.py` & `python-aternos-3.0.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/tests/test_js2py.py` & `python-aternos-3.0.1/tests/test_js2py.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/tests/test_jsnode.py` & `python-aternos-3.0.1/tests/test_jsnode.py`

 * *Files identical despite different names*

### Comparing `python-aternos-3.0.0/tests/test_login.py` & `python-aternos-3.0.1/tests/test_login.py`

 * *Files identical despite different names*

