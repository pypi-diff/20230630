# Comparing `tmp/pypalert-2.1.1.tar.gz` & `tmp/pypalert-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalert-2.1.1.tar", last modified: Fri Jun 30 02:01:35 2023, max compression
+gzip compressed data, was "pypalert-2.1.2.tar", last modified: Fri Jun 30 06:55:53 2023, max compression
```

## Comparing `pypalert-2.1.1.tar` & `pypalert-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 02:01:35.739723 pypalert-2.1.1/
--rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.1.1/LICENSE.rst
--rw-rw-rw-   0        0        0      244 2023-06-30 02:01:35.739723 pypalert-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-06-30 02:01:35.741726 pypalert-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-06-30 02:01:26.000000 pypalert-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:01:35.698264 pypalert-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 02:01:35.724165 pypalert-2.1.1/src/pypalert/
--rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.1.1/src/pypalert/__init__.py
--rw-rw-rw-   0        0        0    24257 2023-06-30 01:11:42.000000 pypalert-2.1.1/src/pypalert/mode1.py
--rw-rw-rw-   0        0        0    11828 2023-06-30 02:01:11.000000 pypalert-2.1.1/src/pypalert/pypalert.py
-drwxrwxrwx   0        0        0        0 2023-06-30 02:01:35.739723 pypalert-2.1.1/src/pypalert.egg-info/
--rw-rw-rw-   0        0        0      244 2023-06-30 02:01:35.000000 pypalert-2.1.1/src/pypalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-30 02:01:35.000000 pypalert-2.1.1/src/pypalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 02:01:35.000000 pypalert-2.1.1/src/pypalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 02:01:35.000000 pypalert-2.1.1/src/pypalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 06:55:53.118528 pypalert-2.1.2/
+-rw-rw-rw-   0        0        0      420 2023-03-31 07:27:40.000000 pypalert-2.1.2/LICENSE.rst
+-rw-rw-rw-   0        0        0      244 2023-06-30 06:55:53.118528 pypalert-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-06-30 06:55:53.126529 pypalert-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-30 06:54:10.000000 pypalert-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:55:53.087433 pypalert-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-30 06:55:53.100432 pypalert-2.1.2/src/pypalert/
+-rw-rw-rw-   0        0        0        0 2023-03-24 06:06:44.000000 pypalert-2.1.2/src/pypalert/__init__.py
+-rw-rw-rw-   0        0        0    24913 2023-06-30 06:54:13.000000 pypalert-2.1.2/src/pypalert/mode1.py
+-rw-rw-rw-   0        0        0    11828 2023-06-30 02:01:11.000000 pypalert-2.1.2/src/pypalert/pypalert.py
+drwxrwxrwx   0        0        0        0 2023-06-30 06:55:53.118528 pypalert-2.1.2/src/pypalert.egg-info/
+-rw-rw-rw-   0        0        0      244 2023-06-30 06:55:53.000000 pypalert-2.1.2/src/pypalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-30 06:55:53.000000 pypalert-2.1.2/src/pypalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 06:55:53.000000 pypalert-2.1.2/src/pypalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 06:55:53.000000 pypalert-2.1.2/src/pypalert.egg-info/top_level.txt
```

### Comparing `pypalert-2.1.1/src/pypalert/mode1.py` & `pypalert-2.1.2/src/pypalert/mode1.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
         self.Y = []
         self.Z = []
         self.Pd = []
         self.Dis = []
         self.Stime = []
         self.Etime = ''
         self.SPS = 0
-        self.connect_success=False
-        self.wait=False
+        self.connect_success = False
+        self.wait = False
+        self.header = 0
+        self.packet_type = 0
         self.PGV_1s = 0
         self.PGA_10s = 0
         self.Pd_warning_threshold = 0
         self.PGA_warning_threshold = 0
         self.Pd_flag = 0
         self.Pd_watch_threshold = 0
         self.PGA_warning_threshold = 0
@@ -79,29 +81,30 @@
         while True:
             link1 = client.recv(2500)
             
             data = link1.hex()
             #print(data)
             if(data == "010200000006010600c00001"):
                 continue
+            
             #print(len(data))
             header = data[:400]
             self.header = header
             #print(header)
-            packet_type = data[2:4] + data[0:2]
+            self.packet_type = int(data[2:4] + data[0:2] ,16)
             #print(packet_type)
-            event_flag = data[6:8] + data[4:6]
+            self.event_flag = int(data[6:8] + data[4:6] ,16)
             #print(event_flag)
             Syear =  int(data[10:12] + data[8:10] ,16)
             Smonth =  int(data[14:16] + data[12:14] ,16)
             Sday =  int(data[18:20] + data[16:18] ,16)
             Shour =  int(data[22:24] + data[20:22] ,16) 
-            Sminute = int(data[26:28] + data[24:26],16)
-            Ssecond = int(data[30:32],16)
-            Smsecond = int(data[28:30],16)
+            Sminute = int(data[26:28] + data[24:26] ,16)
+            Ssecond = int(data[30:32] ,16)
+            Smsecond = int(data[28:30] ,16)
             Stime = str(Syear) + "-" + str(Smonth) + "-" + str(Sday) + "-" + str(Shour) + "-" + str(Sminute) + "-" + str(Ssecond) + "-" + str(Smsecond)
             #print(Stime)
             self.Stime.append(Stime)
             Eyear =  int(data[34:36] + data[32:34] ,16)
             Emonth =  int(data[38:40] + data[36:38] ,16)
             Eday =  int(data[42:44] + data[40:42] ,16)
             Ehour =  int(data[46:48] + data[44:46] ,16) 
@@ -393,14 +396,34 @@
             return Disreturn, UTreturn
             
         except :
             if(self.connect_success == True):
                 print("Port Wrong, so Nothing in list")
             else:
                 print("Connect Fail, so Nothing in list")
+
+                
+    def get_Now_packet_type(self):
+        if(self.wait == False):
+            time.sleep(2)
+            self.wait = True
+        try:
+            return self.packet_type        
+        except :
+            print("Connect Fail, so Nothing in list")
+
+            
+    def get_Now_event_flag(self):
+        if(self.wait == False):
+            time.sleep(2)
+            self.wait = True
+        try:
+            return self.event_flag          
+        except :
+            print("Connect Fail, so Nothing in list")
                 
     def get_Now_PGV_1s(self):
         if(self.wait == False):
             time.sleep(2)
             self.wait = True
         try:
             return self.PGV_1s
```

### Comparing `pypalert-2.1.1/src/pypalert/pypalert.py` & `pypalert-2.1.2/src/pypalert/pypalert.py`

 * *Files identical despite different names*

