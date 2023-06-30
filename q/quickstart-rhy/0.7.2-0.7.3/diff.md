# Comparing `tmp/quickstart_rhy-0.7.2.tar.gz` & `tmp/quickstart_rhy-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart_rhy-0.7.2.tar", max compression
+gzip compressed data, was "quickstart_rhy-0.7.3.tar", max compression
```

## Comparing `quickstart_rhy-0.7.2.tar` & `quickstart_rhy-0.7.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.2/LICENSE
--rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.2/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.2/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.2/QuickStart_Rhy/API/ChatGPT.py
--rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepL.py
--rw-r--r--   0        0        0     1221 2023-05-18 04:35:41.557810 quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepLX.py
--rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.2/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.2/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.2/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.2/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.2/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.2/QuickStart_Rhy/API/alapi.py
--rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/__init__.py
--rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0        0        0     9151 2023-04-24 09:10:36.431917 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/__init__.py
--rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.2/QuickStart_Rhy/NumbaTools/__init__.py
--rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/DiskMac.py
--rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.2/QuickStart_Rhy/ThreadTools/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.2/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.2/QuickStart_Rhy/__cache__.py
--rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.2/QuickStart_Rhy/__config__.py
--rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.2/QuickStart_Rhy/__init__.py
--rw-r--r--   0        0        0    38978 2023-05-15 09:52:32.288702 quickstart_rhy-0.7.2/QuickStart_Rhy/apiTools.py
--rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.2/QuickStart_Rhy/funcList.py
--rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.2/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.2/QuickStart_Rhy/lang.json
--rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.2/QuickStart_Rhy/main.py
--rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.2/QuickStart_Rhy/netTools.py
--rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.2/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.2/QuickStart_Rhy/system.py
--rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.2/README.md
--rw-r--r--   0        0        0      548 2023-05-18 15:02:23.884592 quickstart_rhy-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.2/setup.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.3/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.3/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.3/QuickStart_Rhy/API/ChatGPT.py
+-rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepL.py
+-rw-r--r--   0        0        0     1221 2023-05-18 04:35:41.557810 quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepLX.py
+-rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.3/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.3/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.3/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.3/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.3/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.3/QuickStart_Rhy/API/alapi.py
+-rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/__init__.py
+-rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0        0        0     8878 2023-06-30 12:58:44.682083 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.3/QuickStart_Rhy/NumbaTools/__init__.py
+-rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/DiskMac.py
+-rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/__init__.py
+-rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.3/QuickStart_Rhy/ThreadTools/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.3/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.3/QuickStart_Rhy/__cache__.py
+-rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.3/QuickStart_Rhy/__config__.py
+-rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.3/QuickStart_Rhy/__init__.py
+-rw-r--r--   0        0        0    38978 2023-05-15 09:52:32.288702 quickstart_rhy-0.7.3/QuickStart_Rhy/apiTools.py
+-rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.3/QuickStart_Rhy/funcList.py
+-rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.3/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.3/QuickStart_Rhy/lang.json
+-rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.3/QuickStart_Rhy/main.py
+-rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.3/QuickStart_Rhy/netTools.py
+-rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.3/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.3/QuickStart_Rhy/system.py
+-rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.3/README.md
+-rw-r--r--   0        0        0      548 2023-06-30 12:59:06.312351 quickstart_rhy-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.3/setup.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.3/PKG-INFO
```

### Comparing `quickstart_rhy-0.7.2/LICENSE` & `quickstart_rhy-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/AliCloud.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/AliCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/BaiduCloud.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/ChatGPT.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/DeepLX.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepLX.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/Lolicon.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/Lolicon.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/QiniuOSS.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/SimpleAPI.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/TencentCloud.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/TencentCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/API/alapi.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/API/alapi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ColorTools.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImagePreview.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImagePreview.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/ImageTools.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImageTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/ImageTools/VideoTools.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/HttpServer.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/M3u8DL.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/MultiSingleDL.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/MultiSingleDL.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,41 +22,39 @@
 class MultiSingleDL:
     def __init__(
         self,
         urls: list,
         rt_dir: str,
         proxy: str = "",
         referer: str = "",
-        failed2exit: bool = False,
         save_to_mem: bool = False,
     ):
         self.proxy = proxy
         self.referer = referer
         self.proxies = (
             {"http": "http://" + proxy, "https": "https://" + proxy} if proxy else {}
         )
         self.headers = headers
         if referer:
             self.headers["Referer"] = referer
         self.rt_dir = rt_dir
-        self.failed2exit = failed2exit
         self.save_to_mem = save_to_mem
         self.status_dict = {}
         self.infos = {}
-        self.urls = set(urls)
+        self.urls = urls
         self.task_num = len(self.urls)
         if self.save_to_mem:
             self.content_ls = [b""] * self.task_num
         self.cur_task_num = 0
         self.task_num_lock = Lock()
         self.max_retry = 3
         self.job_queue = queue.Queue()
         self.pool = None
         self.status = qs_default_status("获取文件信息中...")
-        self.progress, self.task_id = NormalProgressBar("多文件下载", self.task_num)
+        self.progress, self.task_id = None, None
 
     def _info(self, url):
         retry = 3
         while retry:
             real_url, name, r = get_fileinfo(url, self.proxy, self.referer)
             if all([real_url, name, r]):
                 break
@@ -68,17 +66,14 @@
             qs_default_console.print(
                 qs_error_string if self.failed2exit else qs_warning_string,
                 f"{url}: Get File information failed, please check network!"
                 if user_lang != "zh"
                 else "获取文件信息失败，请检查网络!",
                 (real_url, name, r)
             )
-            if self.failed2exit:
-                self.enabled = False
-                return
 
         self.infos[url] = {
             "url": real_url,
             "name": os.path.basename(url) if name and "." not in name else name,
             "size": -1
             if not info_flag
             else int(r.headers["content-length"])
@@ -100,18 +95,19 @@
                 proxies=self.proxies,
                 headers=self.headers,
             )
             if not self.save_to_mem:
                 with open(os.path.join(self.rt_dir, filename), "wb") as f:
                     for chunk in r.iter_content(32768):
                         f.write(chunk)
+                        self.progress.advance(self.task_id, 32768)
             else:
                 for chunk in r.iter_content(32768):
                     self.content_ls[job_id] += chunk
-            self.progress.advance(self.task_id, 1)
+                    self.progress.advance(self.task_id, 32768)
         except Exception as e:
             if retry < self.max_retry:
                 self.progress.print(
                     qs_warning_string,
                     f'"{url}": task anomaly, ' if user_lang != "zh" else f'"{url}": 任务异常, ',
                     "retrying..." if user_lang != "zh" else "正在重试...",
                 )
@@ -162,14 +158,16 @@
         failed_num = [self.infos[i]["size"] for i in self.infos].count(-1)
         if not without_output:
             qs_default_console.print(
                 qs_info_string,
                 f"获取文件信息完毕! 文件总大小: {size_format(total)} | 未获取到详细信息条数为: {failed_num}",
             )
         self.status.stop()
+        
+        self.progress, self.task_id = NormalProgressBar("多文件下载", total)
 
         for _id, item in enumerate(self.urls):
             self.job_queue.put(
                 {"url": item,
                     "filename": self.infos[item]["name"], "job_id": _id}
                 if not name_map
                 else {"url": item, "filename": f'{name_map[item]}.{file_suffix(self.infos[item]["name"])}', "job_id": _id}
@@ -196,65 +194,60 @@
 
 
 def multi_single_dl(
     urls: list,
     rt_dir: str = "./",
     proxy: str = "",
     referer: str = "",
-    failed2exit: bool = False,
     name_map: dict = None,
     qps: int = 0,
     qps_info: int = 0,
     qps_download: int = 0,
     without_output: bool = False,
 ):
     """
     并行多个小文件下载
 
     :param urls: 小文件的URL
     :param rt_dir: 文件下载目录
     :param proxy: 代理
     :param referer: referer
-    :param failed2exit: 信息获取失败立即退出
     :param name_map: 文件命名映射{URL: filename}, 后缀名会自动获取并添加
     :param qps: 限制每秒请求次数, qps_info和qps_download默认为qps
     :param qps_info: 限制每秒获取信息次数
     :param qps_download: 限制每秒下载次数
     :param without_output: 不输出信息
     :return: 下载好的文件路径列表
     """
     return MultiSingleDL(
-        urls=urls, rt_dir=rt_dir, proxy=proxy, referer=referer, failed2exit=failed2exit
+        urls=urls, rt_dir=rt_dir, proxy=proxy, referer=referer
     ).run(name_map=name_map, qps=qps, qps_info=qps_info, qps_download=qps_download, without_output=without_output)
 
 
 def multi_single_dl_content_ls(
     urls: list,
     rt_dir: str = "./",
     proxy: str = "",
     referer: str = "",
-    failed2exit: bool = False,
     qps: int = 0,
     without_output: bool = False,
 ):
     """
     并行多个小文件下载
 
     :param urls: 小文件的URL
     :param rt_dir: 文件下载目录
     :param proxy: 代理
     :param referer: referer
-    :param failed2exit: 信息获取失败立即退出
     :param qps: 限制每秒请求次数
     :param without_output: 不输出信息
     :return: 存储在内存中的文件内容列表
     """
     dl = MultiSingleDL(
         urls=urls,
         rt_dir=rt_dir,
         proxy=proxy,
         referer=referer,
-        failed2exit=failed2exit,
         save_to_mem=True,
     )
     dl.run(qps=qps, without_output=without_output)
     return dl.get_content_ls()
```

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/NormalDL.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFi.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NetTools/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/NumbaTools/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/NumbaTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Compress.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/Diff.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/DiskMac.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/DiskMac.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/FileHash.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/SystemTools/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/ThreadTools/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Bar.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Bar.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Line.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Line.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/TuiTools/Table.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Table.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/Wrapper/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/__cache__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/__cache__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/__config__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/__config__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/__init__.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/apiTools.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/apiTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/funcList.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/funcList.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/imageDeal.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/imageDeal.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/lang.json` & `quickstart_rhy-0.7.3/QuickStart_Rhy/lang.json`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/main.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/main.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/netTools.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/netTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/qsLesson.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/qsLesson.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/QuickStart_Rhy/system.py` & `quickstart_rhy-0.7.3/QuickStart_Rhy/system.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/README.md` & `quickstart_rhy-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.2/pyproject.toml` & `quickstart_rhy-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "QuickStart-Rhy"
-version = "0.7.2"
+version = "0.7.3"
 description = "A Command Line Toolbox"
 authors = ["Rhythmicc <rhythmlian.cn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "QuickStart_Rhy"}, {include = "QuickStart_Rhy/lang.json"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = "^2.28.2"
+requests = "^2.31.0"
 urllib3 = "^1.26.15"
 rich = "^13.3.4"
 Qpro = "^0.12.1"
 inquirer-rhy = "^0.1.2"
 
 [tool.poetry.scripts]
 qs = "QuickStart_Rhy.main:main"
```

### Comparing `quickstart_rhy-0.7.2/setup.py` & `quickstart_rhy-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 {'': ['*']}
 
 modules = \
 ['lang']
 install_requires = \
 ['Qpro>=0.12.1,<0.13.0',
  'inquirer-rhy>=0.1.2,<0.2.0',
- 'requests>=2.28.2,<3.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'rich>=13.3.4,<14.0.0',
  'urllib3>=1.26.15,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['qs = QuickStart_Rhy.main:main']}
 
 setup_kwargs = {
     'name': 'quickstart-rhy',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'A Command Line Toolbox',
     'long_description': '# QuickStart_Rhy\n\n```shell\npip3 install quickstart-rhy                                         # stable version\npip3 install git+https://github.com/Rhythmicc/quickstart-rhy.git -U # beta version but more features\n```\n\n| Key  | Value                                              |\n| :--: | -------------------------------------------------- |\n| ENV  | **^Python 3.7**                                    |\n| FONT | **Cascadia Code / Meslo**                          |\n| DOCS | <https://rhythmlian.cn/2020/02/14/QuickStart-Rhy/> |\n\n## Tab Complete\n\n1. fig\n\n   ```shell\n   npx @fig/publish-spec -p complete/fig/qs-<your language>.ts --name qs\n   ```\n\n2. zsh\n\n   ```shell\n   mv _qs /path/in/$FPATH/\n   ```\n',
     'author': 'Rhythmicc',
     'author_email': 'rhythmlian.cn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quickstart_rhy-0.7.2/PKG-INFO` & `quickstart_rhy-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: quickstart-rhy
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Command Line Toolbox
 License: MIT
 Author: Rhythmicc
 Author-email: rhythmlian.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Qpro (>=0.12.1,<0.13.0)
 Requires-Dist: inquirer-rhy (>=0.1.2,<0.2.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Description-Content-Type: text/markdown
 
 # QuickStart_Rhy
 
 ```shell
```

