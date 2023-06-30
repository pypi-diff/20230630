# Comparing `tmp/windbg_copilot-1.0.8.tar.gz` & `tmp/windbg_copilot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.8.tar", last modified: Wed Apr 19 06:31:10 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.9.tar", last modified: Wed Apr 19 07:04:23 2023, max compression
```

## Comparing `windbg_copilot-1.0.8.tar` & `windbg_copilot-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2979 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-04-19 06:30:34.000000 windbg_copilot-1.0.8/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.868481 windbg_copilot-1.0.8/windbg_copilot/
--rw-rw-rw-   0        0        0       82 2023-04-19 06:29:21.000000 windbg_copilot-1.0.8/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-19 06:30:47.000000 windbg_copilot-1.0.8/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7034 2023-04-19 06:29:08.000000 windbg_copilot-1.0.8/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-19 06:31:10.899656 windbg_copilot-1.0.8/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2979 2023-04-19 06:31:09.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 06:31:09.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 06:31:10.000000 windbg_copilot-1.0.8/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 07:04:23.287484 windbg_copilot-1.0.9/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2979 2023-04-19 07:04:23.287484 windbg_copilot-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-04-19 06:30:34.000000 windbg_copilot-1.0.9/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-19 07:04:23.287484 windbg_copilot-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:04:23.257736 windbg_copilot-1.0.9/windbg_copilot/
+-rw-rw-rw-   0        0        0       82 2023-04-19 06:29:21.000000 windbg_copilot-1.0.9/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-19 07:03:56.000000 windbg_copilot-1.0.9/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7111 2023-04-19 07:00:51.000000 windbg_copilot-1.0.9/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:04:23.287484 windbg_copilot-1.0.9/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2979 2023-04-19 07:04:22.000000 windbg_copilot-1.0.9/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-19 07:04:23.000000 windbg_copilot-1.0.9/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:04:22.000000 windbg_copilot-1.0.9/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-19 07:04:22.000000 windbg_copilot-1.0.9/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 07:04:22.000000 windbg_copilot-1.0.9/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.8/LICENSE.txt` & `windbg_copilot-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.8/PKG-INFO` & `windbg_copilot-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.8
+Version: 1.0.9
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

### Comparing `windbg_copilot-1.0.8/README.md` & `windbg_copilot-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.8/setup.cfg` & `windbg_copilot-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.8/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.9/windbg_copilot/windbg_copilot.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,27 @@
         prompt=prompt+"\n give debugging suggestions for above output."
     elif option=="chat":
         prompt==prompt
     elif option=="ask":
         prompt==prompt
 
     openai.api_key = os.getenv("OPENAI_API_KEY")
-    response=openai.ChatCompletion.create(
-    model="gpt-3.5-turbo",
-    messages=[
-            {"role": "system", "content": "You are a Windows debugger copilot."},
-            {"role": "user", "content": "How to start debugging a memory dump?"},
-            {"role": "assistant", "content": "You may run !analyze -v"},
-            {"role": "user", "content": prompt}
-        ]
-    )
+    try:
+        response=openai.ChatCompletion.create(
+        model="gpt-3.5-turbo",
+        messages=[
+                {"role": "system", "content": "You are a Windows debugger copilot."},
+                {"role": "user", "content": "How to start debugging a memory dump?"},
+                {"role": "assistant", "content": "You may run !analyze -v"},
+                {"role": "user", "content": prompt}
+            ]
+        )
+    except Exception as e:
+        print(str(e))
+        return str(e)
     # response=openai.Completion.create(
     # model="gpt-3.5-turbo",
     # prompt=output,
     # max_tokens=4096,
     # temperature=0
     # )
     text = response.choices[0].message.content.strip()
@@ -125,17 +129,15 @@
     result = ""
     while not re.search("LOADING DONE", result):
         result = reader.getoutput()  # ignore initial output
 
     def dbg(command):
         process.stdin.write(command+"\r\n")
         process.stdin.flush()
-        result = ""
-        while result == "":
-            result = reader.getoutput(0.2)
+        result = reader.getoutput(1.5)
         return result
 
     # dump_type = ""
 
     result = dbg("||")
     print(result)
     # speak(result)
@@ -153,18 +155,18 @@
     # chat(result,"explain")
     # chat(result,"suggest")
 
     conversation=""
     while True:
         # Prompt the user for input
         
-        speak("Please enter your input.")
+        # speak("Please enter your input.")
         user_input = input("\n"+'kd> ')
         
-        speak(user_input)
+        # speak(user_input)
         if user_input.startswith("!chat"):
             text=chat(user_input,"chat")
             speak(text)
         elif user_input.startswith("!explain"):
             # Print the output of cdb.exe
             text=chat(conversation,"explain")
             speak(text)
@@ -197,7 +199,8 @@
             # Send the user input to cdb.exe
             result = dbg(user_input)
             conversation += "\n"+result
             print("\n"+result)
 
 
 
+start()
```

### Comparing `windbg_copilot-1.0.8/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.9/windbg_copilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.8
+Version: 1.0.9
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

