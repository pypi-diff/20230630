# Comparing `tmp/redfishtool-1.1.6.tar.gz` & `tmp/redfishtool-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfishtool-1.1.6.tar", last modified: Mon Jun 20 14:29:27 2022, max compression
+gzip compressed data, was "redfishtool-1.1.7.tar", last modified: Fri Jun 30 19:19:27 2023, max compression
```

## Comparing `redfishtool-1.1.6.tar` & `redfishtool-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 14:29:27.664420 redfishtool-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-06-20 14:29:18.000000 redfishtool-1.1.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-06-20 14:29:18.000000 redfishtool-1.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)    37382 2022-06-20 14:29:27.664420 redfishtool-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    36658 2022-06-20 14:29:18.000000 redfishtool-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 14:29:27.660420 redfishtool-1.1.6/redfishtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    37382 2022-06-20 14:29:27.000000 redfishtool-1.1.6/redfishtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-06-20 14:29:27.000000 redfishtool-1.1.6/redfishtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-20 14:29:27.000000 redfishtool-1.1.6/redfishtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-20 14:29:27.000000 redfishtool-1.1.6/redfishtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-20 14:29:27.000000 redfishtool-1.1.6/redfishtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 14:29:27.660420 redfishtool-1.1.6/redfishtoollib/
--rw-r--r--   0 runner    (1001) docker     (121)    33641 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/AccountService.py
--rw-r--r--   0 runner    (1001) docker     (121)    40431 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/Chassis.py
--rw-r--r--   0 runner    (1001) docker     (121)    36346 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/Managers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/ServiceRoot.py
--rw-r--r--   0 runner    (1001) docker     (121)    18465 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/SessionService.py
--rw-r--r--   0 runner    (1001) docker     (121)    49741 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/Systems.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16476 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/raw.py
--rw-r--r--   0 runner    (1001) docker     (121)    27154 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/redfishtoolMain.py
--rw-r--r--   0 runner    (1001) docker     (121)    65475 2022-06-20 14:29:18.000000 redfishtool-1.1.6/redfishtoollib/redfishtoolTransport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 14:29:27.664420 redfishtool-1.1.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-06-20 14:29:18.000000 redfishtool-1.1.6/scripts/redfishtool
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-06-20 14:29:18.000000 redfishtool-1.1.6/scripts/redfishtool.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-20 14:29:27.664420 redfishtool-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-06-20 14:29:18.000000 redfishtool-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:19:27.895078 redfishtool-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-30 19:19:16.000000 redfishtool-1.1.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-30 19:19:16.000000 redfishtool-1.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-06-30 19:19:27.895078 redfishtool-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36658 2023-06-30 19:19:16.000000 redfishtool-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:19:27.891078 redfishtool-1.1.7/redfishtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-06-30 19:19:27.000000 redfishtool-1.1.7/redfishtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 19:19:27.000000 redfishtool-1.1.7/redfishtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:27.000000 redfishtool-1.1.7/redfishtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 19:19:27.000000 redfishtool-1.1.7/redfishtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 19:19:27.000000 redfishtool-1.1.7/redfishtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:19:27.891078 redfishtool-1.1.7/redfishtoollib/
+-rw-r--r--   0 runner    (1001) docker     (123)    33639 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/AccountService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/Chassis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36344 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/Managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/ServiceRoot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/SessionService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50173 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/Systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27152 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/redfishtoolMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65473 2023-06-30 19:19:16.000000 redfishtool-1.1.7/redfishtoollib/redfishtoolTransport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:19:27.891078 redfishtool-1.1.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-30 19:19:16.000000 redfishtool-1.1.7/scripts/redfishtool
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 19:19:16.000000 redfishtool-1.1.7/scripts/redfishtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 19:19:27.895078 redfishtool-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-30 19:19:16.000000 redfishtool-1.1.7/setup.py
```

### Comparing `redfishtool-1.1.6/LICENSE.md` & `redfishtool-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfishtool-1.1.6/PKG-INFO` & `redfishtool-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: redfishtool
-Version: 1.1.6
+Version: 1.1.7
 Summary: Redfishtool package and command-line client
 Home-page: https://github.com/DMTF/Redfishtool
+Download-URL: https://github.com/DMTF/Redfishtool/archive/1.1.5.tar.gz
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
-Download-URL: https://github.com/DMTF/Redfishtool/archive/1.1.5.tar.gz
 Keywords: Redfish
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -620,9 +619,7 @@
 ## Release Process
 
 1. Go to the "Actions" page
 2. Select the "Release and Publish" workflow
 3. Click "Run workflow"
 4. Fill out the form
 5. Click "Run workflow"
-
-
```

### Comparing `redfishtool-1.1.6/README.md` & `redfishtool-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `redfishtool-1.1.6/redfishtool.egg-info/PKG-INFO` & `redfishtool-1.1.7/redfishtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: redfishtool
-Version: 1.1.6
+Version: 1.1.7
 Summary: Redfishtool package and command-line client
 Home-page: https://github.com/DMTF/Redfishtool
+Download-URL: https://github.com/DMTF/Redfishtool/archive/1.1.5.tar.gz
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
-Download-URL: https://github.com/DMTF/Redfishtool/archive/1.1.5.tar.gz
 Keywords: Redfish
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -620,9 +619,7 @@
 ## Release Process
 
 1. Go to the "Actions" page
 2. Select the "Release and Publish" workflow
 3. Click "Run workflow"
 4. Fill out the form
 5. Click "Run workflow"
-
-
```

### Comparing `redfishtool-1.1.6/redfishtool.egg-info/SOURCES.txt` & `redfishtool-1.1.7/redfishtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfishtool-1.1.6/redfishtoollib/AccountService.py` & `redfishtool-1.1.7/redfishtoollib/AccountService.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: AccountService.py
 #
 # contains AccountService related subCommands and access functions
 #
 # Class RfAccountServiceMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
```

### Comparing `redfishtool-1.1.6/redfishtoollib/Chassis.py` & `redfishtool-1.1.7/redfishtoollib/Chassis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: Chassis.py
 #
 # contains Chassis subCommands and access functions
 #
 # Class RfSystemsMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
```

### Comparing `redfishtool-1.1.6/redfishtoollib/Managers.py` & `redfishtool-1.1.7/redfishtoollib/Managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: Managers.py
 #
 # contains Managers related subCommands and access functions
 #
 # Class RfManagersMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
```

### Comparing `redfishtool-1.1.6/redfishtoollib/ServiceRoot.py` & `redfishtool-1.1.7/redfishtoollib/ServiceRoot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: ServiceRoot.py
 #
 # contains serviceRoot related subCommands and access functions
 # Class RfServiceRoot
 #  - getServiceRoot   GET /redfish/v1
 #  - getOdataServiceDocument    GET /redfish/v1/odata
```

### Comparing `redfishtool-1.1.6/redfishtoollib/SessionService.py` & `redfishtool-1.1.7/redfishtoollib/SessionService.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: SessionService.py
 #
 # contains SessionService related subCommands and access functions
 #
 # Class RfSessionServiceMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
```

### Comparing `redfishtool-1.1.6/redfishtoollib/Systems.py` & `redfishtool-1.1.7/redfishtoollib/Systems.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: Systems.py
 #
 # contains Systems related subCommands and access functions
 #
 # Class RfSystemsMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
@@ -580,15 +580,21 @@
                 
             # verify that they have a BootSourceOverrideEnabled and BootSourceOverrideTarget prop
             if(  not "BootSourceOverrideTarget" in bootRes ):
                 rft.printErr("Error, the service does not have oneOf BootSourceOverride..Enabled or ..Target property")
                 return(8,None,False,None)
             
             #form the patch data
-            patchData={"Boot": {"BootSourceOverrideEnabled": enabledVal, "BootSourceOverrideTarget": targetVal } }
+
+            # Get the value of "BootSourceOverrideTarget" property and pass it in the patch request.
+            # Some HW vendors need this property to be passed explicitly.
+            if "BootSourceOverrideMode" in d["Boot"]:
+                patchData={"Boot": {"BootSourceOverrideEnabled": enabledVal, "BootSourceOverrideTarget": targetVal, "BootSourceOverrideMode": d["Boot"]["BootSourceOverrideMode"] } }
+            else:
+                patchData={"Boot": {"BootSourceOverrideEnabled": enabledVal, "BootSourceOverrideTarget": targetVal } }
 
             #call the generic patch command to send the patch.  This takes care of etag support
             rc,r,j,d=rft.patchResource(rft, r, patchData)
             
            
         if(rc==0):
             rft.printVerbose(1," Systems setBootOverride:",skip1=True, printV12=cmdTop)
```

### Comparing `redfishtool-1.1.6/redfishtoollib/raw.py` & `redfishtool-1.1.7/redfishtoollib/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool: rawMain.py
 #
 # contains raw subCommands and access functions
 #
 # Class RfRawMain
 #  - functions init, displayUsage, displayHelp, displayOperations,
```

### Comparing `redfishtool-1.1.6/redfishtoollib/redfishtoolMain.py` & `redfishtool-1.1.7/redfishtoollib/redfishtoolMain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool:  redfishtool.py  Main
 #
 # contains:
 #  - functions called for usage:
 #     -- displayUsage, displayOptions, listSubcommands, displayHelp
 #  - Main routine, with argc/argv option parsing, and valid argument/option checking
```

### Comparing `redfishtool-1.1.6/redfishtoollib/redfishtoolTransport.py` & `redfishtool-1.1.7/redfishtoollib/redfishtoolTransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Notice:
 # Copyright 2016 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool:  redfishtoolTransport.py
 #
 # Contents:
 # 1. Class RfSessionAuth --  holds auto-created session Auth info.  'requests' calls to get credentials
 # 2. Class RfTransport -- has the generic functions to send/receive http requests, generic print functions, etc  
 #  - transport object variables used to pass transport parameters from main to cmdTable and subcommand objects
@@ -56,16 +56,16 @@
         #print("Call SESSION AUTH")
         return(r)
 
 class RfTransport():
     def __init__(self):
         # constant parameters-- these dont change and are not updated
         self.program="redfishtool"              # program name (in case we want to change it)
-        self.version="1.1.6"                    # this redfishtool version
-        self.releaseDate="06/20/2022"           # release date for this version of redfishtool
+        self.version="1.1.7"                    # this redfishtool version
+        self.releaseDate="06/30/2023"           # release date for this version of redfishtool
         self.downloadFrom="https://github.com/DMTF/Redfishtool" # where to find redfishtool
         self.magic="12345"                      # used for debug to test for a known parameter in this object
         self.UNAUTHENTICATED_API=1              # unauthenticated API that doesn't send credentials in body data
         self.AUTHENTICATED_API=2                # authenticated API that doesn't send credentials in body data
         self.AUTHENTICATED_WITH_CREDENTIALS_API=3 # Authenticated API that sends credentials eg passwd update, add user
         self.UNAUTHENTICATED_WITH_CREDENTIALS_API=4 # session login (unauthenticated) but sends credentials
         self.authValidValues=["None", "Basic", "Session"]
```

### Comparing `redfishtool-1.1.6/scripts/redfishtool` & `redfishtool-1.1.7/scripts/redfishtool`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 # Copyright Notice:
 # Copyright 2016, 2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool:  scripts/redfishtool
 #
 # contents:
 #  -CLI wrapper:  calls main() routine in redfishtool  package
 #
 #  Note: structure supports a future lib interface to the routines
```

### Comparing `redfishtool-1.1.6/scripts/redfishtool.py` & `redfishtool-1.1.7/scripts/redfishtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 # Copyright Notice:
 # Copyright 2016, 2020 DMTF. All rights reserved.
-# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/master/LICENSE.md
+# License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfishtool/blob/main/LICENSE.md
 
 # redfishtool:  scripts/redfishtool.py
 #
 # contents:
 #  -CLI wrapper:  calls main() routine in redfishtool  package
 #
 #  Note: structure supports a future lib interface to the routines
```

### Comparing `redfishtool-1.1.6/setup.py` & `redfishtool-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='redfishtool',
-      version='1.1.6',
+      version='1.1.7',
       description='Redfishtool package and command-line client',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='DMTF, https://www.dmtf.org/standards/feedback',
       license='BSD 3-clause "New" or "Revised License"',
       classifiers=[
           'Development Status :: 5 - Production/Stable',
```

