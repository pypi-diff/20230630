# Comparing `tmp/rubiran-2.0.1.tar.gz` & `tmp/rubiran-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.1.tar", last modified: Sat Feb 18 18:53:05 2023, max compression
+gzip compressed data, was "rubiran-2.0.2.tar", last modified: Fri Jun 30 12:28:34 2023, max compression
```

## Comparing `rubiran-2.0.1.tar` & `rubiran-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 18:53:05.135638 rubiran-2.0.1/
--rw-rw-rw-   0        0        0     1086 2022-10-17 13:06:02.000000 rubiran-2.0.1/LICENCE
--rw-rw-rw-   0        0        0     1533 2023-02-18 18:53:05.135638 rubiran-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      167 2022-10-19 11:05:05.000000 rubiran-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-18 18:53:05.097788 rubiran-2.0.1/rubiran/
--rw-rw-rw-   0        0        0      810 2022-12-26 07:21:57.000000 rubiran-2.0.1/rubiran/An_Wb.py
--rw-rw-rw-   0        0        0     1532 2023-02-18 18:50:19.000000 rubiran-2.0.1/rubiran/How.py
--rw-rw-rw-   0        0        0     2416 2023-02-18 15:38:01.000000 rubiran-2.0.1/rubiran/Socket.py
--rw-rw-rw-   0        0        0        0 2023-02-18 16:02:02.000000 rubiran-2.0.1/rubiran/Untitled-1.py
--rw-rw-rw-   0        0        0       28 2022-10-18 18:06:54.000000 rubiran-2.0.1/rubiran/__init__.py
--rw-rw-rw-   0        0        0    73915 2022-10-21 13:45:33.000000 rubiran-2.0.1/rubiran/client.py
--rw-rw-rw-   0        0        0     1208 2022-09-27 11:51:32.000000 rubiran-2.0.1/rubiran/encryption.py
-drwxrwxrwx   0        0        0        0 2023-02-18 18:53:05.135638 rubiran-2.0.1/rubiran.egg-info/
--rw-rw-rw-   0        0        0     1533 2023-02-18 18:53:04.000000 rubiran-2.0.1/rubiran.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-02-18 18:53:05.000000 rubiran-2.0.1/rubiran.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 18:53:04.000000 rubiran-2.0.1/rubiran.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-02-18 18:53:04.000000 rubiran-2.0.1/rubiran.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-18 18:53:05.151269 rubiran-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1710 2023-02-18 18:50:28.000000 rubiran-2.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.582064 rubiran-2.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.2/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1472 2023-06-30 12:28:34.586064 rubiran-2.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.486064 rubiran-2.0.2/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.2/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1532 2023-06-30 12:24:26.000000 rubiran-2.0.2/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.2/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.2/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53687 2023-06-30 12:17:54.000000 rubiran-2.0.2/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.2/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-30 12:28:34.566064 rubiran-2.0.2/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1472 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-06-30 12:28:34.000000 rubiran-2.0.2/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-30 12:28:34.590064 rubiran-2.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1710 2023-06-30 12:25:19.000000 rubiran-2.0.2/setup.py
```

### Comparing `rubiran-2.0.1/LICENCE` & `rubiran-2.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.1/PKG-INFO` & `rubiran-2.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1
-Name: rubiran
-Version: 2.0.1
-Summary: Another example of the library making the Rubik's robot
-Home-page: https://rubika.ir/python_java_source
-Author: mamadcoder
-Author-email: mamadcoder@gmail.com
-License: MIT
-Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-
-
-## An example:
-``` python
-from rubiran import rubiran
-
-bot = rubiran("Auth Account")
-
-gap = "guids"
-
-bot.sendMessage(gap,"pyrubika")
-```
-
-
-### How to import the Rubik's library
-
-``` bash
-from rubiran import rubiran
-```
-
-### How to install the library
-
-``` bash
-pip install rubiran
-```
-
-### My ID in Rubika
-
-``` bash
-@mamadcoder1
-```
-## And My ID Channel in Rubika
-
-``` bash
-@python_java_source 
-```
+Metadata-Version: 2.1
+Name: rubiran
+Version: 2.0.2
+Summary: Another example of the library making the Rubik's robot
+Home-page: https://rubika.ir/python_java_source
+Author: mamadcoder
+Author-email: mamadcoder@gmail.com
+License: MIT
+Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+
+
+## An example:
+``` python
+from rubiran import rubiran
+
+bot = rubiran("Auth Account")
+
+gap = "guids"
+
+bot.sendMessage(gap,"pyrubika")
+```
+
+
+### How to import the Rubik's library
+
+``` bash
+from rubiran import rubiran
+```
+
+### How to install the library
+
+``` bash
+pip install rubiran
+```
+
+### My ID in Rubika
+
+``` bash
+@mamadcoder1
+```
+## And My ID Channel in Rubika
+
+``` bash
+@python_java_source 
+```
```

### Comparing `rubiran-2.0.1/rubiran/An_Wb.py` & `rubiran-2.0.2/rubiran/An_Wb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from requests import get, post
 
 class SetClines:
 	web = {
-		"app_name"    : "Main",
-		"app_version" : "4.0.7",
-		"platform"    : "Web",
-		"package"     : "web.rubika.ir",
-		"lang_code"   : "fa"
+		"app_name": "Main",
+		"app_version": "4.3.3",
+		"platform": "Web",
+		"package": "web.rubika.ir",
+		"lang_code": "fa"
 	}
 
 	android = {
 	    "app_name":"Main",
-		"app_version":"2.9.5",
+		"app_version":"3.3.2",
 		"platform":"Android",
-		"package":"ir.resaneh1.iptv",
+		"package":"app.rbmain.a",
 		"lang_code":"fa"
 	}
 
 
 class Server:
 	matnadress = []
 	m = get("https://getdcmess.iranlms.ir/").json()["data"]["API"]
```

### Comparing `rubiran-2.0.1/rubiran/How.py` & `rubiran-2.0.2/rubiran/How.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.1    
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.2    
 
 {color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2022 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
 """
```

### Comparing `rubiran-2.0.1/rubiran/Socket.py` & `rubiran-2.0.2/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.1/rubiran.egg-info/PKG-INFO` & `rubiran-2.0.2/rubiran.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1
-Name: rubiran
-Version: 2.0.1
-Summary: Another example of the library making the Rubik's robot
-Home-page: https://rubika.ir/python_java_source
-Author: mamadcoder
-Author-email: mamadcoder@gmail.com
-License: MIT
-Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-
-
-## An example:
-``` python
-from rubiran import rubiran
-
-bot = rubiran("Auth Account")
-
-gap = "guids"
-
-bot.sendMessage(gap,"pyrubika")
-```
-
-
-### How to import the Rubik's library
-
-``` bash
-from rubiran import rubiran
-```
-
-### How to install the library
-
-``` bash
-pip install rubiran
-```
-
-### My ID in Rubika
-
-``` bash
-@mamadcoder1
-```
-## And My ID Channel in Rubika
-
-``` bash
-@python_java_source 
-```
+Metadata-Version: 2.1
+Name: rubiran
+Version: 2.0.2
+Summary: Another example of the library making the Rubik's robot
+Home-page: https://rubika.ir/python_java_source
+Author: mamadcoder
+Author-email: mamadcoder@gmail.com
+License: MIT
+Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+
+
+## An example:
+``` python
+from rubiran import rubiran
+
+bot = rubiran("Auth Account")
+
+gap = "guids"
+
+bot.sendMessage(gap,"pyrubika")
+```
+
+
+### How to import the Rubik's library
+
+``` bash
+from rubiran import rubiran
+```
+
+### How to install the library
+
+``` bash
+pip install rubiran
+```
+
+### My ID in Rubika
+
+``` bash
+@mamadcoder1
+```
+## And My ID Channel in Rubika
+
+``` bash
+@python_java_source 
+```
```

### Comparing `rubiran-2.0.1/setup.py` & `rubiran-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ``` bash
 @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.1",
+    version = "2.0.2",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

