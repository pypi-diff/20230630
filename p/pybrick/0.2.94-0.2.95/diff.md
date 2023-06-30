# Comparing `tmp/pybrick-0.2.94-py3-none-any.whl.zip` & `tmp/pybrick-0.2.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6380 bytes, number of entries: 7
+Zip file size: 6400 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
 -rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-29 01:19 pybrick/ptest.csv
--rw-rw-rw-  2.0 fat    14527 b- defN 23-Jun-30 17:41 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      521 b- defN 23-Jun-30 17:42 pybrick-0.2.94.dist-info/RECORD
-7 files, 15558 bytes uncompressed, 5454 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat    14578 b- defN 23-Jun-30 18:15 pybrick/pybrick.py
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      521 b- defN 23-Jun-30 18:15 pybrick-0.2.95.dist-info/RECORD
+7 files, 15609 bytes uncompressed, 5474 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pybrick/ptest.csv
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.94.dist-info/METADATA
+Filename: pybrick-0.2.95.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.94.dist-info/WHEEL
+Filename: pybrick-0.2.95.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.94.dist-info/top_level.txt
+Filename: pybrick-0.2.95.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.94.dist-info/RECORD
+Filename: pybrick-0.2.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/pybrick.py

```diff
@@ -1,7 +1,8 @@
+__version__="0.2.95"
 __doc__="""
 pybrick uses sqlalchemy to provide a convenient connection to Yellowbrick.
 """
 import pdb
 import os
 import sys
 import subprocess
@@ -13,14 +14,15 @@
 import inspect
 from io import StringIO
 
 class YbConnector:
     """ A pytezza-esque connector to Yellowbrick. """
     def __init__(self,host,db,user,pw="",psql_compatible_version='13.7',ybhosts=None):
         """ """
+        self.orig_host=host
         self.host=self._resolveHost(host,ybhosts)
         self.db=db
         self.user=user
         self.pw=pw if pw else os.environ.get('YBPASSWORD')
         
         self.psql_compatible_version=psql_compatible_version
         self.dry_run_mode=False
```

