# Comparing `tmp/SiteScraper-1.2.2.tar.gz` & `tmp/SiteScraper-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-1.2.2.tar", last modified: Thu May 25 10:06:56 2023, max compression
+gzip compressed data, was "SiteScraper-2.1.0.tar", last modified: Fri Jun 30 16:00:56 2023, max compression
```

## Comparing `SiteScraper-1.2.2.tar` & `SiteScraper-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 10:06:56.229882 SiteScraper-1.2.2/
--rw-rw-rw-   0        0        0     3989 2023-05-25 10:06:56.230879 SiteScraper-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 10:06:56.190986 SiteScraper-1.2.2/SiteScraper/
--rw-rw-rw-   0        0        0     9896 2023-05-25 08:44:46.000000 SiteScraper-1.2.2/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-1.2.2/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 10:06:56.227889 SiteScraper-1.2.2/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-05-25 10:06:55.000000 SiteScraper-1.2.2/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-25 10:06:56.000000 SiteScraper-1.2.2/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 10:06:55.000000 SiteScraper-1.2.2/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 10:06:55.000000 SiteScraper-1.2.2/SiteScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-25 10:06:55.000000 SiteScraper-1.2.2/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-25 10:06:55.000000 SiteScraper-1.2.2/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-1.2.2/licence.txt
--rw-rw-rw-   0        0        0      158 2023-05-25 10:06:56.235883 SiteScraper-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-05-25 10:01:52.000000 SiteScraper-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.810847 SiteScraper-2.1.0/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 16:00:56.810847 SiteScraper-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.800861 SiteScraper-2.1.0/SiteScraper/
+-rw-rw-rw-   0        0        0    10823 2023-06-30 16:00:13.000000 SiteScraper-2.1.0/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.0/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.809338 SiteScraper-2.1.0/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 10:06:55.000000 SiteScraper-2.1.0/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.0/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-06-30 16:00:56.811865 SiteScraper-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-06-30 16:00:41.000000 SiteScraper-2.1.0/setup.py
```

### Comparing `SiteScraper-1.2.2/PKG-INFO` & `SiteScraper-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 1.2.2
+Version: 2.1.0
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-1.2.2/README.md` & `SiteScraper-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SiteScraper-1.2.2/SiteScraper/SiteScraper.py` & `SiteScraper-2.1.0/SiteScraper/SiteScraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,37 +19,47 @@
             options.add_argument('--no-sandbox')
             options.add_argument('--headless')
             options.add_argument('--disable-gpu')
             options.add_argument("--window-size=1920, 1200")
             options.add_argument('--disable-dev-shm-usage')
             driver = webdriver.Firefox(options=options)
             return driver
-    def yt_vedios_data(self, url,browser='Chrome'):
+    def yt_vedios_data(self, url,browser='Chrome',abort=bool):
         if browser=='Chrome' or browser=='chrome':
             driver = self.web_driver_chrome()
            
             self.url = url
             try:
                 driver.get(self.url)
                 
                 prev_h = 0
+                videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
+                counter=0
                 while True:
+                    counter=counter+1
                     height = driver.execute_script('''
                         return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );''')
                     driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
-
+                    if abort==True:
+                        if counter>=15:
+                            abortinput=input("Do you want to abort? press [y] for yes. ")
+                            if abortinput=="y" or abortinput=="Y":
+                                break
+                            else:
+                                counter=0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
+
                 title = list()
                 views = list()
                 when = list()
                 for vedio in videos:
                     title.append(vedio.find_element(By.ID, 'video-title').text)
                     views.append(vedio.find_element(
                         By.XPATH, './/*[@id="metadata-line"]/span[1]').text)
@@ -68,27 +78,35 @@
         else:
             driver =self.web_driver_firefox()
             self.url = url
             try:
                 driver.get(self.url)
                 
                 prev_h = 0
+                counter=0
                 while True:
+                    counter+=counter
                     height = driver.execute_script('''
                         return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
                         Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
                         Math.max(document.body.clientHeight, document.documentElement.clientHeight)
                         );''')
                     driver.execute_script(f"window.scrollTo({prev_h},{prev_h+2000})")
                     time.sleep(3)
                     prev_h += driver.execute_script('return window.innerHeight;')
                     if prev_h >= height:
                         break
-
+                    if abort==True:
+                        if counter>=15:
+                            abortinput=input("Do you want to stop? press [y] for yes. ")
+                            if abortinput=="y" or abortinput=="Y":
+                                break
+                            else:
+                                counter=0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 title = list()
                 views = list()
                 when = list()
                 for vedio in videos:
                     title.append(vedio.find_element(By.ID, 'video-title').text)
                     views.append(vedio.find_element(
```

### Comparing `SiteScraper-1.2.2/SiteScraper.egg-info/PKG-INFO` & `SiteScraper-2.1.0/SiteScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 1.2.2
+Version: 2.1.0
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-1.2.2/licence.txt` & `SiteScraper-2.1.0/licence.txt`

 * *Files identical despite different names*

