# Comparing `tmp/pycrawlers-0.1.2.tar.gz` & `tmp/pycrawlers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrawlers-0.1.2.tar", last modified: Fri Jun 30 07:25:11 2023, max compression
+gzip compressed data, was "pycrawlers-0.1.3.tar", last modified: Fri Jun 30 09:49:00 2023, max compression
```

## Comparing `pycrawlers-0.1.2.tar` & `pycrawlers-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.388288 pycrawlers-0.1.2/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.2/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)     2885 2023-06-30 07:25:11.388158 pycrawlers-0.1.2/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)     2428 2023-06-30 07:24:12.000000 pycrawlers-0.1.2/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.385222 pycrawlers-0.1.2/other/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.2/other/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.2/other/dw_hg.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.385415 pycrawlers-0.1.2/pycrawlers/
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.386355 pycrawlers-0.1.2/pycrawlers/Hugging_Face/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.2/pycrawlers/Hugging_Face/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.2/pycrawlers/Hugging_Face/download.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.387168 pycrawlers-0.1.2/pycrawlers/Web_Site/
--rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page.py
--rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page_id.py
--rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-0.1.2/pycrawlers/Web_Site/url_filters.py
--rw-r--r--   0 bo         (501) staff       (20)     1035 2023-06-30 07:15:34.000000 pycrawlers-0.1.2/pycrawlers/__init__.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.387821 pycrawlers-0.1.2/pycrawlers/common/
--rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.2/pycrawlers/common/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.2/pycrawlers/common/default_data.py
--rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.2/pycrawlers/common/tools.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 07:25:11.386003 pycrawlers-0.1.2/pycrawlers.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)     2885 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      556 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-30 07:25:11.000000 pycrawlers-0.1.2/pycrawlers.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-30 07:25:11.388329 pycrawlers-0.1.2/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-30 07:22:01.000000 pycrawlers-0.1.2/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.254108 pycrawlers-0.1.3/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2022-08-16 07:24:33.000000 pycrawlers-0.1.3/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)     2934 2023-06-30 09:49:00.254001 pycrawlers-0.1.3/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)     2477 2023-06-30 09:48:31.000000 pycrawlers-0.1.3/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.251176 pycrawlers-0.1.3/other/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:58:18.000000 pycrawlers-0.1.3/other/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)      745 2022-08-17 09:04:51.000000 pycrawlers-0.1.3/other/dw_hg.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.251380 pycrawlers-0.1.3/pycrawlers/
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-30 09:44:44.000000 pycrawlers-0.1.3/pycrawlers/__init__.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.252362 pycrawlers-0.1.3/pycrawlers/common/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 07:44:00.000000 pycrawlers-0.1.3/pycrawlers/common/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2644 2023-06-21 08:33:43.000000 pycrawlers-0.1.3/pycrawlers/common/default_data.py
+-rw-r--r--   0 bo         (501) staff       (20)     4962 2023-06-21 09:14:16.000000 pycrawlers-0.1.3/pycrawlers/common/tools.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.252783 pycrawlers-0.1.3/pycrawlers/huggingfaces/
+-rw-r--r--   0 bo         (501) staff       (20)       73 2022-08-17 08:04:35.000000 pycrawlers-0.1.3/pycrawlers/huggingfaces/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     4657 2023-02-16 06:57:07.000000 pycrawlers-0.1.3/pycrawlers/huggingfaces/download.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.253691 pycrawlers-0.1.3/pycrawlers/websites/
+-rw-r--r--   0 bo         (501) staff       (20)       75 2023-06-25 03:29:06.000000 pycrawlers-0.1.3/pycrawlers/websites/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     2239 2023-06-25 05:57:32.000000 pycrawlers-0.1.3/pycrawlers/websites/get_web_page.py
+-rw-r--r--   0 bo         (501) staff       (20)     3607 2023-06-30 07:03:43.000000 pycrawlers-0.1.3/pycrawlers/websites/get_web_page_id.py
+-rw-r--r--   0 bo         (501) staff       (20)      882 2023-06-30 09:44:44.000000 pycrawlers-0.1.3/pycrawlers/websites/get_websites.py
+-rw-r--r--   0 bo         (501) staff       (20)      568 2023-06-30 07:15:34.000000 pycrawlers-0.1.3/pycrawlers/websites/url_filters.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-30 09:49:00.251868 pycrawlers-0.1.3/pycrawlers.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)     2934 2023-06-30 09:48:59.000000 pycrawlers-0.1.3/pycrawlers.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      592 2023-06-30 09:49:00.000000 pycrawlers-0.1.3/pycrawlers.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-30 09:48:59.000000 pycrawlers-0.1.3/pycrawlers.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       71 2023-06-30 09:49:00.000000 pycrawlers-0.1.3/pycrawlers.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)       17 2023-06-30 09:49:00.000000 pycrawlers-0.1.3/pycrawlers.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-30 09:49:00.254142 pycrawlers-0.1.3/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      907 2023-06-30 09:48:31.000000 pycrawlers-0.1.3/setup.py
```

### Comparing `pycrawlers-0.1.2/LICENSE` & `pycrawlers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/PKG-INFO` & `pycrawlers-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -58,56 +58,55 @@
 
 #### 2.  通用抓取网页
 可以抓取那些反爬不厉害的网站
 
 - 简单使用
 
 
-    from pycrawlers import website
+    from pycrawlers import crawl_website
 
     mongo_host = ''
     mongo_port = '27017'
     db_name = 'huxiu'
     id_collection_name = 'huxiu_id'
     collection_name = 'huxiu'
     base_url = 'https://www.huxiu.com'
     
     
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
+    crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
 
 - 进阶使用
   - 可以使用url filter 过滤不想抓取的网页，比如视频、图片
-  
-
 
 
-    from pycrawlers import website
-    from pycrawlers.Web_Site.url_filters import filter_video_photo
-
-    mongo_host = ''
-    mongo_port = '27017'
-    db_name = 'huxiu'
-    id_collection_name = 'huxiu_id'
-    collection_name = 'huxiu'
-    base_url = 'https://www.huxiu.com'
-
-    # url_filter 也可以自己定义
-    # photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
-    #               'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
-    # 
-    # video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
-    #               'dat', 'mkv', 'flv', 'vob', 'mpeg']
-    # 
-    # 
-    # def filter_video_photo(url: str):
-    #     all_types = photo_type + video_type
-    #     for i in all_types:
-    #         if url.endswith('.' + i):
-    #             return False
-    #     return True
-    
-    
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
+      from pycrawlers import crawl_website
+      from pycrawlers.websites.url_filters import filter_video_photo
+  
+      mongo_host = ''
+      mongo_port = '27017'
+      db_name = 'huxiu'
+      id_collection_name = 'huxiu_id'
+      collection_name = 'huxiu'
+      base_url = 'https://www.huxiu.com'
+      
+      """
+      url_filter 也可以自己定义
+      photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
+                  'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
+      
+      video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
+                  'dat', 'mkv', 'flv', 'vob', 'mpeg']
+      
+      
+      def filter_video_photo(url: str):
+        all_types = photo_type + video_type
+        for i in all_types:
+            if url.endswith('.' + i):
+                return False
+        return True
+      """
+      
+      crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
```

### Comparing `pycrawlers-0.1.2/README.md` & `pycrawlers-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,54 +42,53 @@
 
 #### 2.  通用抓取网页
 可以抓取那些反爬不厉害的网站
 
 - 简单使用
 
 
-    from pycrawlers import website
+    from pycrawlers import crawl_website
 
     mongo_host = ''
     mongo_port = '27017'
     db_name = 'huxiu'
     id_collection_name = 'huxiu_id'
     collection_name = 'huxiu'
     base_url = 'https://www.huxiu.com'
     
     
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
+    crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
 
 - 进阶使用
   - 可以使用url filter 过滤不想抓取的网页，比如视频、图片
-  
-
 
 
-    from pycrawlers import website
-    from pycrawlers.Web_Site.url_filters import filter_video_photo
-
-    mongo_host = ''
-    mongo_port = '27017'
-    db_name = 'huxiu'
-    id_collection_name = 'huxiu_id'
-    collection_name = 'huxiu'
-    base_url = 'https://www.huxiu.com'
-
-    # url_filter 也可以自己定义
-    # photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
-    #               'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
-    # 
-    # video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
-    #               'dat', 'mkv', 'flv', 'vob', 'mpeg']
-    # 
-    # 
-    # def filter_video_photo(url: str):
-    #     all_types = photo_type + video_type
-    #     for i in all_types:
-    #         if url.endswith('.' + i):
-    #             return False
-    #     return True
-    
-    
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
+      from pycrawlers import crawl_website
+      from pycrawlers.websites.url_filters import filter_video_photo
+  
+      mongo_host = ''
+      mongo_port = '27017'
+      db_name = 'huxiu'
+      id_collection_name = 'huxiu_id'
+      collection_name = 'huxiu'
+      base_url = 'https://www.huxiu.com'
+      
+      """
+      url_filter 也可以自己定义
+      photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
+                  'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
+      
+      video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
+                  'dat', 'mkv', 'flv', 'vob', 'mpeg']
+      
+      
+      def filter_video_photo(url: str):
+        all_types = photo_type + video_type
+        for i in all_types:
+            if url.endswith('.' + i):
+                return False
+        return True
+      """
+      
+      crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
```

### Comparing `pycrawlers-0.1.2/other/dw_hg.py` & `pycrawlers-0.1.3/other/dw_hg.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/Hugging_Face/download.py` & `pycrawlers-0.1.3/pycrawlers/huggingfaces/download.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page.py` & `pycrawlers-0.1.3/pycrawlers/websites/get_web_page.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/Web_Site/get_web_page_id.py` & `pycrawlers-0.1.3/pycrawlers/websites/get_web_page_id.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/Web_Site/url_filters.py` & `pycrawlers-0.1.3/pycrawlers/websites/url_filters.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/common/default_data.py` & `pycrawlers-0.1.3/pycrawlers/common/default_data.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers/common/tools.py` & `pycrawlers-0.1.3/pycrawlers/common/tools.py`

 * *Files identical despite different names*

### Comparing `pycrawlers-0.1.2/pycrawlers.egg-info/PKG-INFO` & `pycrawlers-0.1.3/pycrawlers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrawlers
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Crawlers
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -58,56 +58,55 @@
 
 #### 2.  通用抓取网页
 可以抓取那些反爬不厉害的网站
 
 - 简单使用
 
 
-    from pycrawlers import website
+    from pycrawlers import crawl_website
 
     mongo_host = ''
     mongo_port = '27017'
     db_name = 'huxiu'
     id_collection_name = 'huxiu_id'
     collection_name = 'huxiu'
     base_url = 'https://www.huxiu.com'
     
     
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
+    crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url)
 
 - 进阶使用
   - 可以使用url filter 过滤不想抓取的网页，比如视频、图片
-  
-
 
 
-    from pycrawlers import website
-    from pycrawlers.Web_Site.url_filters import filter_video_photo
-
-    mongo_host = ''
-    mongo_port = '27017'
-    db_name = 'huxiu'
-    id_collection_name = 'huxiu_id'
-    collection_name = 'huxiu'
-    base_url = 'https://www.huxiu.com'
-
-    # url_filter 也可以自己定义
-    # photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
-    #               'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
-    # 
-    # video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
-    #               'dat', 'mkv', 'flv', 'vob', 'mpeg']
-    # 
-    # 
-    # def filter_video_photo(url: str):
-    #     all_types = photo_type + video_type
-    #     for i in all_types:
-    #         if url.endswith('.' + i):
-    #             return False
-    #     return True
-    
-    
-    website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
+      from pycrawlers import crawl_website
+      from pycrawlers.websites.url_filters import filter_video_photo
+  
+      mongo_host = ''
+      mongo_port = '27017'
+      db_name = 'huxiu'
+      id_collection_name = 'huxiu_id'
+      collection_name = 'huxiu'
+      base_url = 'https://www.huxiu.com'
+      
+      """
+      url_filter 也可以自己定义
+      photo_type = ['bmp', 'jpg','png', 'tif', 'gif', 'pcx', 'tga', 'exif', 'fpx', 'svg', 'psd',
+                  'cdr', 'pcd', 'dxf', 'ufo', 'eps', 'ai', 'raw', 'WMF', 'webp', 'avif', 'apng']
+      
+      video_type = ['wmv', 'asf', 'asx', 'rm', 'rmvb', 'mp4', '3gp', 'mov', 'm4v', 'avi',
+                  'dat', 'mkv', 'flv', 'vob', 'mpeg']
+      
+      
+      def filter_video_photo(url: str):
+        all_types = photo_type + video_type
+        for i in all_types:
+            if url.endswith('.' + i):
+                return False
+        return True
+      """
+      
+      crawl_website(mongo_host, mongo_port, db_name, id_collection_name, collection_name, base_url, url_filter=filter_video_photo)
```

### Comparing `pycrawlers-0.1.2/setup.py` & `pycrawlers-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrawlers',
-    version='0.1.2',
+    version='0.1.3',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A collection of Crawlers',
     long_description=long_description,
```

