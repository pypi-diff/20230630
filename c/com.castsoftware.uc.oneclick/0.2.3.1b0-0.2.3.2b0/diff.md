# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.3.1b0.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.3.1b0.tar", last modified: Thu Jun 29 15:08:32 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.3.2b0.tar", last modified: Thu Jun 29 23:50:51 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0.tar` & `com.castsoftware.uc.oneclick-0.2.3.2b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.410026 com.castsoftware.uc.oneclick-0.2.3.1b0/
--rw-rw-rw-   0        0        0      519 2023-06-29 15:08:32.396474 com.castsoftware.uc.oneclick-0.2.3.1b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.103520 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      519 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 15:08:31.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.201927 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/
--rw-rw-rw-   0        0        0        2 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.254447 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2745 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     4028 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    24987 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:08:32.384153 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4740 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     6814 2023-06-28 22:46:02.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9130 2023-06-28 22:43:16.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     2893 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-06-29 11:52:29.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2566 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    10978 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     3947 2023-06-28 21:49:06.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/setup.py
--rw-rw-rw-   0        0        0      779 2023-06-29 15:07:41.000000 com.castsoftware.uc.oneclick-0.2.3.1b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 15:08:32.410026 com.castsoftware.uc.oneclick-0.2.3.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 23:50:51.158737 com.castsoftware.uc.oneclick-0.2.3.2b0/
+-rw-rw-rw-   0        0        0      519 2023-06-29 23:50:51.150525 com.castsoftware.uc.oneclick-0.2.3.2b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.619769 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.745750 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.978145 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2745 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     4068 2023-06-29 19:27:55.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    24987 2023-06-29 16:00:26.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-06-29 23:50:51.139469 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4740 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7274 2023-06-29 23:42:53.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9130 2023-06-28 22:43:16.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     2893 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-06-29 11:52:29.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2740 2023-06-29 17:12:02.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    10978 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     3947 2023-06-28 21:49:06.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/setup.py
+-rw-rw-rw-   0        0        0      779 2023-06-29 23:50:33.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 23:50:51.158737 com.castsoftware.uc.oneclick-0.2.3.2b0/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.3.1b0
+Version: 0.2.3.2b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.3.1b0
+Version: 0.2.3.2b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/highlight_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         pass
 
     def run(cls, config:Config):
         if not config.is_hl_active:
             cls._log.warning('Highlight configuration is incomplete, analysis will not run')
             return 0
         
-        rest = HLRestCall(config.hl_url,config.hl_user,config.hl_password,config.hl_instance)
+        rest = HLRestCall(hl_base_url=config.hl_url,hl_user=config.hl_user,hl_pswd=config.hl_password,hl_instance=config.hl_instance)
 
         try:
             process = {}
             for appl in config.application:
                 hl_status = config.application[appl]['hl']
                 if hl_status == '' or hl_status.startswith('Error'):
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cloc.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from time import sleep
 
 from os import getcwd
 from os.path import exists,abspath,getsize
 from re import findall
 from pandas import DataFrame,ExcelWriter
 
+from ctypes import windll, c_int, c_wchar_p
 
 #TODO: Convert total line to formulas (d1-SHP)
 #TODO: Format all numbers as integers not text (d1-SHP)
 #TODO: Group tabs in pairs (before, after) then by application (d2)
 
 class ClocPreCleanup(SourceValidation):
     writer = None
@@ -40,14 +41,15 @@
 
     @property
     def cloc_results(cls):
         return cls._df
 
     def _run_cloc(cls,work_folder:str,cloc_output:str,cloc_output_ignored:str):
         args = [cls.cloc_path,work_folder,"--report-file",cloc_output,"--ignored",cloc_output_ignored,"--quiet"]
+        cls._log.info(' '.join(args))
         proc = run_process(args,False)
 
         sleep(10)
         if proc.poll() is not None and exists(cloc_output):
             return 'DONE'
         else:
             return proc
@@ -60,28 +62,42 @@
         cls.cloc_path=abspath(f'{config.base}\\scripts\\{cls.config.cloc_version}')
         list_of_tech_file=abspath(f'{config.base}\\scripts\\ListOfTechnologies.csv')
         with open(list_of_tech_file) as f:
             tech_list = f.read().splitlines()
             
         process = {}
         cloc_run=False
+
+        DefineDosDevice = windll.kernel32.DefineDosDeviceW
+        DefineDosDevice.argtypes = [ c_int, c_wchar_p, c_wchar_p ]
+
+        project_folder=abspath(f'{config.work}/AIP/{config.project_name}')
+        # Create a subst. Check the return for non-zero to mean success
+        if DefineDosDevice(0, "F:", project_folder ) == 0:
+            raise RuntimeError("Subst failed")
+
         for appl in config.application:
             cls._log.info(f'Running {config.project_name}/{appl}')
             create_folder(f'{config.report}/{config.project_name}/{appl}')
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
             cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt')
-            work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
+#            work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
+            work_folder = abspath(f'F:/{appl}')
 
             #if the report is already out there - no need to continue
             if exists(cloc_output):
                 process[appl]=None
                 continue 
             cloc_run=True
             process[appl] = cls._run_cloc(work_folder,cloc_output,cloc_output_ignored)
 
+        # Delete the subst.
+        if DefineDosDevice(2, "F:", project_folder ) == 0:
+            raise RuntimeError("Subst failed")
+
         #has all cloc processing completed
         all_done=False
         while (not all_done):
             all_done=True
             for p in process:
                 if process[p]=='DONE':
                     continue
@@ -104,32 +120,29 @@
                 sleep(60)
 
         for appl in config.application:
             #reading cloc_output.txt file
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
             cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt') 
             cls._log.info(f'Processing {cloc_output}')
-            summary_list=[]   
             with open(cloc_output, 'r') as f:
                 content = f.read()
-                f.seek(0)
-                summary_list= [line.rstrip('\n').lstrip() for line in f]
-                #print(summary_list)
 
             #extracting required data from content of cloc_output.txt using python regex
-#            pattern='(\S{1,}|\w{1,}[:])\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
-            pattern='([\w #]{30})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
-            statistics_list=findall(pattern,content)
-            statistics_list= statistics_list[:-1]
+            header=content.split('\n')[2]
+            header_list=findall('\w+',header.upper())
+
+            summary='\n'.join(content.split('\n')[4:-4])
+            pattern='(.{25})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
+            statistics_list=findall(pattern,summary)
             
             with open(cloc_output_ignored, 'r') as fp:
                 lines = len(fp.readlines())
             statistics_list.append(('Unknown Files','0','0','0',str(lines)))
-
-            df = DataFrame(statistics_list,columns=['LANGUAGE','FILES','BLANK','COMMENT','CODE'])
+            df = DataFrame(statistics_list,columns=header_list)
 
             #making technolgy case insensitive
             tech_list = list(map(lambda x: x.lower().strip(), tech_list))
             df['APPLICABLE']=df['LANGUAGE'].str.lower().str.strip().isin(tech_list)
 
             #converting column values into int from string
             numbers=['FILES','BLANK','COMMENT','CODE']
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/unzip.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,41 +24,45 @@
       found = True
       cls._log.info(f'Running {cls.__class__.__name__} for all applications')
       while found:
          found = False
          for app in apps:
             app_folder_aip = f'{config.work}\\AIP\\{config.project_name}\\{app}'
             for root, dirs, files in walk(app_folder_aip):
+               if '__MACOSX' in root or '.DS_Store' in files:
+                  continue
                for file in files:
                   if file.endswith(".zip") or \
                      file.endswith(".7z") or \
                      file.endswith(".tar") or \
                      file.endswith(".gztar") or \
                      file.endswith(".bztar"):
                      found = True
                      
-                     full_name = abspath(f'{root}\\{file}')
+                     full_name = abspath(f'{root.strip()}\\{file}')
                      dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
                      cls._log.info(f'Unzipping {full_name}')
 
                      Archive(full_name).extractall(dest,auto_create_dir=True)
                      
                      remove(full_name)
 
             app_folder_hl = f'{config.work}\\HL\\{config.project_name}\\{app}'
             for root, dirs, files in walk(app_folder_hl):
+               if '__MACOSX' in root:
+                  continue
                for file in files:
                   if file.endswith(".zip") or \
                      file.endswith(".7z") or \
                      file.endswith(".tar") or \
                      file.endswith(".gztar") or \
                      file.endswith(".bztar"):
                      found = True
                      
-                     full_name = abspath(f'{root}\\{file}')
+                     full_name = abspath(f'{root.strip()}\\{file}')
                      dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
                      cls._log.info(f'Unzipping {full_name}')
 
                      Archive(full_name).extractall(dest,auto_create_dir=True)
                      
                      remove(full_name)
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/oneclick/setup.py` & `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/setup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.1b0/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.3.2b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.3.1-beta' #prod version
+version='0.2.3.2-beta' #prod version
 dependencies = [
     'pandas','python-pptx==0.6.18','python-docx',
     'argparse_formatter','django','pyunpack',
     'patool','archive',
     'com.castsoftware.uc.python.common',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
```

