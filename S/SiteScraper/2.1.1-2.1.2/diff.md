# Comparing `tmp/SiteScraper-2.1.1.tar.gz` & `tmp/SiteScraper-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-2.1.1.tar", last modified: Fri Jun 30 16:14:09 2023, max compression
+gzip compressed data, was "SiteScraper-2.1.2.tar", last modified: Fri Jun 30 18:15:02 2023, max compression
```

## Comparing `SiteScraper-2.1.1.tar` & `SiteScraper-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.859696 SiteScraper-2.1.1/
--rw-rw-rw-   0        0        0     3989 2023-06-30 16:14:09.859696 SiteScraper-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.851069 SiteScraper-2.1.1/SiteScraper/
--rw-rw-rw-   0        0        0    10724 2023-06-30 16:13:26.000000 SiteScraper-2.1.1/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.1/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.858180 SiteScraper-2.1.1/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 10:06:55.000000 SiteScraper-2.1.1/SiteScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.1/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-30 16:14:09.860727 SiteScraper-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-06-30 16:13:38.000000 SiteScraper-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.568222 SiteScraper-2.1.2/SiteScraper/
+-rw-rw-rw-   0        0        0    10726 2023-06-30 18:11:27.000000 SiteScraper-2.1.2/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.2/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 18:15:02.000000 SiteScraper-2.1.2/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.2/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-06-30 18:15:02.576250 SiteScraper-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-06-30 18:14:28.000000 SiteScraper-2.1.2/setup.py
```

### Comparing `SiteScraper-2.1.1/PKG-INFO` & `SiteScraper-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.1
+Version: 2.1.2
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.1/README.md` & `SiteScraper-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SiteScraper-2.1.1/SiteScraper/SiteScraper.py` & `SiteScraper-2.1.2/SiteScraper/SiteScraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                         );''')
                     driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
                     if abort==True:
-                        if counter>=15:
+                        if counter>=100:
                             abortinput=input("Do you want to abort? press [y] for yes. ")
                             if abortinput=="y" or abortinput=="Y":
                                 break
                             else:
                                 counter=0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 title = list()
@@ -88,15 +88,15 @@
                         );''')
                     driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
                     if abort==True:
-                        if counter>=15:
+                        if counter>=100:
                             abortinput=input("Do you want to stop? press [y] for yes. ")
                             if abortinput=="y" or abortinput=="Y":
                                 break
                             else:
                                 counter=0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 title = list()
```

### Comparing `SiteScraper-2.1.1/SiteScraper.egg-info/PKG-INFO` & `SiteScraper-2.1.2/SiteScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.1
+Version: 2.1.2
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.1/licence.txt` & `SiteScraper-2.1.2/licence.txt`

 * *Files identical despite different names*

