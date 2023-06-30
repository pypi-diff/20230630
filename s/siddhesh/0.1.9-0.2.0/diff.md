# Comparing `tmp/siddhesh-0.1.9.tar.gz` & `tmp/siddhesh-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siddhesh-0.1.9.tar", last modified: Fri Jun 30 09:29:55 2023, max compression
+gzip compressed data, was "siddhesh-0.2.0.tar", last modified: Fri Jun 30 09:46:18 2023, max compression
```

## Comparing `siddhesh-0.1.9.tar` & `siddhesh-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.528981 siddhesh-0.1.9/
--rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      767 2023-06-30 09:29:55.525946 siddhesh-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 09:29:55.529946 siddhesh-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-06-30 09:29:42.000000 siddhesh-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.508267 siddhesh-0.1.9/siddhesh/
--rw-rw-rw-   0        0        0     1359 2023-06-30 09:22:08.000000 siddhesh-0.1.9/siddhesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 09:29:55.523795 siddhesh-0.1.9/siddhesh.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 09:29:55.000000 siddhesh-0.1.9/siddhesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:46:18.707695 siddhesh-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 10:44:11.000000 siddhesh-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-06-30 09:46:18.706515 siddhesh-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1885 2023-03-30 12:36:34.000000 siddhesh-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:46:18.708707 siddhesh-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-30 09:46:09.000000 siddhesh-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:46:18.656443 siddhesh-0.2.0/siddhesh/
+-rw-rw-rw-   0        0        0     1673 2023-06-30 09:45:53.000000 siddhesh-0.2.0/siddhesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:46:18.703461 siddhesh-0.2.0/siddhesh.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-30 09:46:18.000000 siddhesh-0.2.0/siddhesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-30 09:46:18.000000 siddhesh-0.2.0/siddhesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:46:18.000000 siddhesh-0.2.0/siddhesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 09:46:18.000000 siddhesh-0.2.0/siddhesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 09:46:18.000000 siddhesh-0.2.0/siddhesh.egg-info/top_level.txt
```

### Comparing `siddhesh-0.1.9/LICENSE` & `siddhesh-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.9/PKG-INFO` & `siddhesh-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.9
+Version: 0.2.0
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `siddhesh-0.1.9/README.md` & `siddhesh-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `siddhesh-0.1.9/setup.py` & `siddhesh-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.9"
+VERSION = "0.2.0"
 DESCRIPTION = "Check out Siddhesh Kulthe's profile, or send him a direct message!"
 LONG_DESCRIPTION = "A package that downloads Siddhesh Kulthe's Resume on your computer. All you need to do is to import siddhesh and use .Start() method to start the app!"
 
 # Setting up
 setup(
     name="siddhesh",
     version=VERSION,
```

### Comparing `siddhesh-0.1.9/siddhesh/__init__.py` & `siddhesh-0.2.0/siddhesh/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,34 +5,41 @@
 URL = "https://linkedin.com/in/siddheshkulthe"
 recipient_email = "siddheshkulthe43@gmail.com"
 
 social_list = []
 
 
 def send_message():
-    message = str(input("Enter your message: "))
+    name = str(input("So, what can I call you: "))
     time.sleep(1)
-    print("Just so that Siddhesh can get back to you,")
+    print(f"It's nice to meet you {name}!")
     time.sleep(1)
-    email = str(input("Please enter your email:"))
+    message = str(input("Tell me your messsage here: "))
+    time.sleep(1)
+    print(f"Just so that Siddhesh can get back to you {name},")
+    time.sleep(1)
+    email = str(input("Please share me your email: "))
     vercel_url = "http://34.204.127.0:5001"
     data = {"message": message, "email": email}
 
     # Make the HTTP POST request to your Vercel app's endpoint
     response = requests.post(vercel_url, json=data)
 
     if response.status_code == 200:
-        print("Message sent successfully!")
+        print("Thanks for reaching out.")
+        print("I've successfully informed Siddhesh that you wanted to reach out!")
     else:
         print("Error sending message.")
 
 
 def start():
     print("Hey yo! Nice to meet you :)")
     time.sleep(1)
+    print("I'm a Freddy. Developed by Siddhesh Kulthe.")
+    time.sleep(1)
     print("What would you like to do?\n")
     time.sleep(1)
     choice = int(
         input(
             "1. Send Siddhesh A Message \n2. Check out Siddhesh's LinkedIn \nEnter (1/2): "
         )
     )
@@ -40,9 +47,9 @@
         send_message()
     elif choice != 1:
         print("\nCool! I'll lead you to his resume!")
         time.sleep(2)
         print("Btw, he's a super cool guy. Would really love to be friends with you :)")
         time.sleep(2)
         print("...")
-        time.sleep(3)
+        time.sleep(1)
         webbrowser.open(URL)
```

### Comparing `siddhesh-0.1.9/siddhesh.egg-info/PKG-INFO` & `siddhesh-0.2.0/siddhesh.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siddhesh
-Version: 0.1.9
+Version: 0.2.0
 Summary: Check out Siddhesh Kulthe's profile, or send him a direct message!
 Author: Siddhesh Kulthe
 Author-email: siddheshkulthe43@gmail.com
 Keywords: python,sid,siddhesh kulthe,profile,message,social,iamsid47
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

