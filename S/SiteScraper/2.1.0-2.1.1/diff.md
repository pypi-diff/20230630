# Comparing `tmp/SiteScraper-2.1.0.tar.gz` & `tmp/SiteScraper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiteScraper-2.1.0.tar", last modified: Fri Jun 30 16:00:56 2023, max compression
+gzip compressed data, was "SiteScraper-2.1.1.tar", last modified: Fri Jun 30 16:14:09 2023, max compression
```

## Comparing `SiteScraper-2.1.0.tar` & `SiteScraper-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.810847 SiteScraper-2.1.0/
--rw-rw-rw-   0        0        0     3989 2023-06-30 16:00:56.810847 SiteScraper-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.800861 SiteScraper-2.1.0/SiteScraper/
--rw-rw-rw-   0        0        0    10823 2023-06-30 16:00:13.000000 SiteScraper-2.1.0/SiteScraper/SiteScraper.py
--rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.0/SiteScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 16:00:56.809338 SiteScraper-2.1.0/SiteScraper.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 10:06:55.000000 SiteScraper-2.1.0/SiteScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 16:00:56.000000 SiteScraper-2.1.0/SiteScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.0/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-30 16:00:56.811865 SiteScraper-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-06-30 16:00:41.000000 SiteScraper-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.859696 SiteScraper-2.1.1/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 16:14:09.859696 SiteScraper-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3760 2023-05-25 09:12:48.000000 SiteScraper-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.851069 SiteScraper-2.1.1/SiteScraper/
+-rw-rw-rw-   0        0        0    10724 2023-06-30 16:13:26.000000 SiteScraper-2.1.1/SiteScraper/SiteScraper.py
+-rw-rw-rw-   0        0        0       46 2023-05-25 10:05:57.000000 SiteScraper-2.1.1/SiteScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 16:14:09.858180 SiteScraper-2.1.1/SiteScraper.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 10:06:55.000000 SiteScraper-2.1.1/SiteScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-30 16:14:09.000000 SiteScraper-2.1.1/SiteScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      626 2023-05-25 07:53:45.000000 SiteScraper-2.1.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-06-30 16:14:09.860727 SiteScraper-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-06-30 16:13:38.000000 SiteScraper-2.1.1/setup.py
```

### Comparing `SiteScraper-2.1.0/PKG-INFO` & `SiteScraper-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.0/README.md` & `SiteScraper-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SiteScraper-2.1.0/SiteScraper/SiteScraper.py` & `SiteScraper-2.1.1/SiteScraper/SiteScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,17 @@
             options.add_argument("--window-size=1920, 1200")
             options.add_argument('--disable-dev-shm-usage')
             driver = webdriver.Firefox(options=options)
             return driver
     def yt_vedios_data(self, url,browser='Chrome',abort=bool):
         if browser=='Chrome' or browser=='chrome':
             driver = self.web_driver_chrome()
-           
             self.url = url
             try:
                 driver.get(self.url)
-                
                 prev_h = 0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
                 counter=0
                 while True:
                     counter=counter+1
                     height = driver.execute_script('''
                         return Math.max(
@@ -51,15 +49,14 @@
                         if counter>=15:
                             abortinput=input("Do you want to abort? press [y] for yes. ")
                             if abortinput=="y" or abortinput=="Y":
                                 break
                             else:
                                 counter=0
                 videos = driver.find_elements(By.XPATH, '//*[@id="contents"]')
-
                 title = list()
                 views = list()
                 when = list()
                 for vedio in videos:
                     title.append(vedio.find_element(By.ID, 'video-title').text)
                     views.append(vedio.find_element(
                         By.XPATH, './/*[@id="metadata-line"]/span[1]').text)
@@ -70,21 +67,19 @@
                 list_of_dic = {'title': title, 'views': views, 'when': when}
                 
                 driver.quit()
                 return list_of_dic
             except:
                 driver.quit()
                 logging.error("Invalid url")
-            
         else:
             driver =self.web_driver_firefox()
             self.url = url
             try:
                 driver.get(self.url)
-                
                 prev_h = 0
                 counter=0
                 while True:
                     counter+=counter
                     height = driver.execute_script('''
                         return Math.max(
                         Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
@@ -109,16 +104,14 @@
                 when = list()
                 for vedio in videos:
                     title.append(vedio.find_element(By.ID, 'video-title').text)
                     views.append(vedio.find_element(
                         By.XPATH, './/*[@id="metadata-line"]/span[1]').text)
                     when .append(vedio.find_element(
                         By.XPATH, './/*[@id="metadata-line"]/span[2]').text)
-                    
-
                 list_of_dic = {'title': title, 'views': views, 'when': when}
                 
                 driver.quit()
                 return list_of_dic
             except:
                 driver.quit()
                 logging.error("Invalid url")
@@ -154,15 +147,14 @@
                 for element in comment_likes:
                     likes.append(element.text)
                 time_posted=list()
                 comment_time=driver.find_elements(By.XPATH,'//*[@id="header-author"]/yt-formatted-string/a')
                 for element in comment_time:
                     time_posted.append(element.text)
                 dic={'comment_text':txt,'likes':likes,'comment_time':time_posted}
-                
                 driver.quit()
                 return dic
 
             except:
                 driver.quit()
                 logging.error('Invalid url')
         else: 
@@ -195,15 +187,15 @@
                 likes=list()
                 for element in comment_likes:
                     likes.append(element.text)
                 time_posted=list()
                 comment_time=driver.find_elements(By.XPATH,'//*[@id="header-author"]/yt-formatted-string/a')
                 for element in comment_time:
                     time_posted.append(element.text)
-                dic={'comment_text':txt,'likes':likes,'comment_time':time_posted}
+                dic={'comment_text':txt,'likes':likes,'comment_posting_time':time_posted}
                 
                 driver.quit()
                 return dic
 
             except:
                 driver.quit()
                 logging.error('Invalid url')
```

### Comparing `SiteScraper-2.1.0/SiteScraper.egg-info/PKG-INFO` & `SiteScraper-2.1.1/SiteScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiteScraper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Scraping high intensity content sites
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # SiteScraper
```

### Comparing `SiteScraper-2.1.0/licence.txt` & `SiteScraper-2.1.1/licence.txt`

 * *Files identical despite different names*

