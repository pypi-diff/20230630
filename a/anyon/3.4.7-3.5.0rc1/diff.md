# Comparing `tmp/anyon-3.4.7-cp311-none-win_amd64.whl.zip` & `tmp/anyon-3.5.0rc1-cp311-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 358613 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-22 00:42 anyon-3.4.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2318 b- defN 23-Jun-22 00:42 anyon-3.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-22 00:42 anyon-3.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-22 00:42 anyon-3.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 23-Jun-22 00:42 anyon-3.4.7.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Jun-22 00:42 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    81920 b- defN 23-Jun-22 00:42 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   101376 b- defN 23-Jun-22 00:42 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   154624 b- defN 23-Jun-22 00:42 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Jun-22 00:42 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    94208 b- defN 23-Jun-22 00:42 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   133120 b- defN 23-Jun-22 00:42 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    62976 b- defN 23-Jun-22 00:42 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   115200 b- defN 23-Jun-22 00:42 anyon/stage/device.pyd
-14 files, 788771 bytes uncompressed, 356851 bytes compressed:  54.8%
+Zip file size: 834272 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-30 03:00 anyon-3.5.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2271 b- defN 23-Jun-30 03:00 anyon-3.5.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-30 03:00 anyon-3.5.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 03:00 anyon-3.5.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      391 b- defN 23-Jun-30 03:00 anyon-3.5.0rc1.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   121968 b- defN 23-Jun-30 02:57 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   305934 b- defN 23-Jun-30 02:58 anyon/loader.so
+-rwxr-xr-x  2.0 unx   360830 b- defN 23-Jun-30 02:57 anyon/remote.so
+-rwxr-xr-x  2.0 unx   517950 b- defN 23-Jun-30 02:57 anyon/server.so
+-rwxr-xr-x  2.0 unx   122240 b- defN 23-Jun-30 02:59 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   324066 b- defN 23-Jun-30 02:59 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   472000 b- defN 23-Jun-30 02:58 anyon/stage/compiler.so
+-rwxr-xr-x  2.0 unx   236611 b- defN 23-Jun-30 02:59 anyon/stage/demodulator.so
+-rwxr-xr-x  2.0 unx   392462 b- defN 23-Jun-30 02:59 anyon/stage/device.so
+14 files, 2857896 bytes uncompressed, 832498 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-3.4.7.dist-info/LICENSE
+Filename: anyon-3.5.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.4.7.dist-info/METADATA
+Filename: anyon-3.5.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.4.7.dist-info/WHEEL
+Filename: anyon-3.5.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.4.7.dist-info/top_level.txt
+Filename: anyon-3.5.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.4.7.dist-info/RECORD
+Filename: anyon-3.5.0rc1.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/compiler.pyd
+Filename: anyon/stage/compiler.so
 Comment: 
 
-Filename: anyon/stage/demodulator.pyd
+Filename: anyon/stage/demodulator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
 Zip file comment:
```

## Comparing `anyon-3.4.7.dist-info/METADATA` & `anyon-3.5.0rc1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1
-Name: anyon
-Version: 3.4.7
-Summary: Dream It Possible!
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.20.0)
-Requires-Dist: axion (>=3.4.5)
-Requires-Dist: srpc (>=4.2.8)
-Requires-Dist: zee (>=0.0.3)
-Requires-Dist: requests (>=2.28.0)
-
+Metadata-Version: 2.1
+Name: anyon
+Version: 3.5.0rc1
+Summary: Dream It Possible!
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: axion (>=3.4.5)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.3)
+Requires-Dist: requests (>=2.28.0)
+
```

