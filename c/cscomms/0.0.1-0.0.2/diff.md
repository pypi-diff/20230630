# Comparing `tmp/cscomms-0.0.1.tar.gz` & `tmp/cscomms-0.0.2.tar.gz`

## Comparing `cscomms-0.0.1.tar` & `cscomms-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cscomms-0.0.1/src/cscomms/__init__.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cscomms-0.0.1/src/cscomms/messaging.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cscomms-0.0.1/tests/distTest.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cscomms-0.0.1/LICENSE
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 cscomms-0.0.1/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 cscomms-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 cscomms-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cscomms-0.0.2/src/cscomms/__init__.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 cscomms-0.0.2/src/cscomms/messaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cscomms-0.0.2/tests/distTest.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cscomms-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 cscomms-0.0.2/README.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 cscomms-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 cscomms-0.0.2/PKG-INFO
```

### Comparing `cscomms-0.0.1/src/cscomms/messaging.py` & `cscomms-0.0.2/src/cscomms/messaging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import inspect
 import json
 from threading import Thread
 import os
 import tempfile
 import time
+import shutil
 
 # Internal class for functions the end user doesn't have to see
 class Internal:
   "Functions used internally, Its probably not the best idea to run these!"
   def __init__(self):
+    self.shutdown = False
     self.messagerInstance = Internal.messager()
   class messager:
     def __init__(self):
       self.connections = []
       self.tempFilePath = os.path.join(tempfile.gettempdir(), "python_messaging")
       if not os.path.exists(self.tempFilePath):
           os.makedirs(self.tempFilePath)
@@ -31,15 +33,18 @@
       oldData = file.read()
     while True:
       with open(data['filePath'], 'r') as file:
         fileContents = file.read()
         if fileContents != oldData:
           func(json.loads(fileContents))
           oldData = fileContents
-        time.sleep(interval)
+      if internalInstance.shutdown:
+        break  
+      time.sleep(interval)
+
   def make_listener(func, data, interval:float):
     listener = Thread(target=Internal.listener,args=(func, data, interval))
     listener.start()
 
 internalInstance = Internal()
 
 def listen(channel:int, interval:float=1.0):
@@ -54,15 +59,14 @@
     else:
       data = {
         'channel': channel,
         'filePath': f"{internalInstance.messagerInstance.tempFilePath}/{channel}.message"
       }
       internalInstance.messagerInstance.connections.append(data)
       Internal.make_listener(func, data, interval)
-      
   return inner
 
 def send(channel:int, message:dict):
   if Internal.Value_In_Dict(channel, internalInstance.messagerInstance.connections):
     for dict in internalInstance.messagerInstance.connections:
       if dict['channel'] == channel:
         data = dict
@@ -74,8 +78,28 @@
     data = {
       'channel': channel,
       'filePath': f"{internalInstance.messagerInstance.tempFilePath}/{channel}.message"
     }
     internalInstance.messagerInstance.connections.append(data)
     jsonMessage = json.dumps(message)
     with open(data['filePath'], 'w') as file:
-      file.write(jsonMessage)
+      file.write(jsonMessage)
+
+def cleanup():
+  """cleans up the storage location for the channels.
+  ---
+  # WARNING!!!
+  DO NOT run this while any other scripts using messages are running, as it will probably break those
+  """
+  internalInstance.shutdown = True
+  time.sleep(0.2)
+  shutil.rmtree(internalInstance.messagerInstance.tempFilePath)
+
+def init(channel:int):
+  "initialises a channel"
+  filePath = os.path.join(internalInstance.messagerInstance.tempFilePath, f"{channel}.message")
+  if not os.path.exists(internalInstance.messagerInstance.tempFilePath):
+    os.mkdir(internalInstance.messagerInstance.tempFilePath)
+  if not os.path.exists(filePath):
+    with open(filePath, 'w') as file:
+      file.write(" ")
+  return True
```

### Comparing `cscomms-0.0.1/LICENSE` & `cscomms-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cscomms-0.0.1/README.md` & `cscomms-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 
 # **Python Script Communication**
 
 This script provides functions for communication between scripts using message passing. It includes a decorator `listen` to mark a function as a message listener and a function `send` to send messages to specific channels.
 
 ## **Usage**
 
+### **Init**
+
+Function to initialise a channel (create the files). run this before using the channel!
+
+`init(channel)`
+
+- **channel**: an integer representing the channel to initialise
+
 ### **Listen**
 
 Decorator to make a function a message listener. The function needs a parameter for the message, which it will return as a dictionary.
 
 ```
 @listen(channel, interval=1.0)
 def listener_func(message):
     # Process the received message
-    ...
 ```
 
 - **channel**: An integer representing the channel to listen to.
 - **interval** (optional): The interval in seconds to check for new messages (default is 1.0 second).
 
 ### **Send**
 
@@ -26,21 +33,29 @@
 
 `send(channel, message, metadata={"source": main_file_name})`
 
 - **channel**: An integer representing the channel to send the message to.
 - **message**: A dictionary containing the message data.
 - **metadata** (optional): A dictionary containing additional metadata for the message. By default, it includes the source file name where the `send` function is called.
 
+### cleanup
+
+Function to clean up used files. WARNING! ONLY RUN THIS WHEN YOU ARE DONE USING THE PACKAGE! it WILL halt running scripts
+
+`cleanup()`
+
 ## **Example**
 
 Here's an example of how to use the script:
 
 ```
 from cscomms import messaging as cscomms
 
+cscomms.init(1)
+
 @cscomms.listen(channel=1, interval=0.5)
 def message_listener(message):
   print(message)
 
 cscomms.send(channel=1, message={"user": "username", "message": "message"})
 ```
```

### Comparing `cscomms-0.0.1/pyproject.toml` & `cscomms-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "cscomms"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="joploljojo3", email="jorisblaauw12@gmail.com" },
 ]
 description = "A python package for cross-script communication in a simple method"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cscomms-0.0.1/PKG-INFO` & `cscomms-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cscomms
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for cross-script communication in a simple method
 Project-URL: Homepage, https://example.com
 Project-URL: Bug Tracker, https://example.com
 Author-email: joploljojo3 <jorisblaauw12@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,23 +16,30 @@
 
 # **Python Script Communication**
 
 This script provides functions for communication between scripts using message passing. It includes a decorator `listen` to mark a function as a message listener and a function `send` to send messages to specific channels.
 
 ## **Usage**
 
+### **Init**
+
+Function to initialise a channel (create the files). run this before using the channel!
+
+`init(channel)`
+
+- **channel**: an integer representing the channel to initialise
+
 ### **Listen**
 
 Decorator to make a function a message listener. The function needs a parameter for the message, which it will return as a dictionary.
 
 ```
 @listen(channel, interval=1.0)
 def listener_func(message):
     # Process the received message
-    ...
 ```
 
 - **channel**: An integer representing the channel to listen to.
 - **interval** (optional): The interval in seconds to check for new messages (default is 1.0 second).
 
 ### **Send**
 
@@ -40,21 +47,29 @@
 
 `send(channel, message, metadata={"source": main_file_name})`
 
 - **channel**: An integer representing the channel to send the message to.
 - **message**: A dictionary containing the message data.
 - **metadata** (optional): A dictionary containing additional metadata for the message. By default, it includes the source file name where the `send` function is called.
 
+### cleanup
+
+Function to clean up used files. WARNING! ONLY RUN THIS WHEN YOU ARE DONE USING THE PACKAGE! it WILL halt running scripts
+
+`cleanup()`
+
 ## **Example**
 
 Here's an example of how to use the script:
 
 ```
 from cscomms import messaging as cscomms
 
+cscomms.init(1)
+
 @cscomms.listen(channel=1, interval=0.5)
 def message_listener(message):
   print(message)
 
 cscomms.send(channel=1, message={"user": "username", "message": "message"})
 ```
```

