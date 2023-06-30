# Comparing `tmp/PEALS-1.2.1.tar.gz` & `tmp/PEALS-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/net/nfs-irwrsrchnas01/labs/JJChen_Grp/zhoukr/home/software/peals/dist/tmphvf73t49/PEALS-1.2.1.tar", last modified: Fri Mar 24 03:08:46 2023, max compression
+gzip compressed data, was "/net/nfs-irwrsrchnas01/labs/JJChen_Grp/zhoukr/home/software/peals/dist/tmp5dztknox/PEALS-1.2.4.tar", last modified: Fri Jun 30 04:48:44 2023, max compression
```

## Comparing `PEALS-1.2.1.tar` & `PEALS-1.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.611159 PEALS-1.2.1/
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.438807 PEALS-1.2.1/PEALS/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       58 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/__init__.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.503233 PEALS-1.2.1/PEALS/collection/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       74 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/__init__.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     8287 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/bamtool.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    38218 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/bedutils.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    23860 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/functools.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    12628 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/gfftools.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    13220 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/collection/optioncheck.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.536441 PEALS-1.2.1/PEALS/io/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       69 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/__init__.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     2073 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/constant.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     3411 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/paramlog.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     6010 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/report.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    16636 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/signals.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     2091 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/io/streamtools.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.553630 PEALS-1.2.1/PEALS/peak/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       37 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/peak/__init__.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    13530 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/peak/peakcall.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    34004 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/peak/peakutils.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.577861 PEALS-1.2.1/PEALS/stats/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       50 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/stats/__init__.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    14079 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/stats/correction.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    17368 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/stats/peaktest.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     4922 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/stats/statstools.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.595010 PEALS-1.2.1/PEALS/subcmd/
--rwxrwx---   0 kzhou    (22264) domain users (10000)       44 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/subcmd/__init__.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)     9486 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/subcmd/callpeak_cmd.py
--rwxrwx---   0 kzhou    (22264) domain users (10000)    14761 2023-03-24 02:57:50.000000 PEALS-1.2.1/PEALS/subcmd/diffpeak_cmd.py
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.468089 PEALS-1.2.1/PEALS.egg-info/
--rwxrwx---   0 kzhou    (22264) domain users (10000)     4727 2023-03-24 03:09:06.000000 PEALS-1.2.1/PEALS.egg-info/PKG-INFO
--rwxrwx---   0 kzhou    (22264) domain users (10000)      746 2023-03-24 03:09:06.000000 PEALS-1.2.1/PEALS.egg-info/SOURCES.txt
--rwxrwx---   0 kzhou    (22264) domain users (10000)        1 2023-03-24 03:09:06.000000 PEALS-1.2.1/PEALS.egg-info/dependency_links.txt
--rwxrwx---   0 kzhou    (22264) domain users (10000)      260 2023-03-24 03:09:06.000000 PEALS-1.2.1/PEALS.egg-info/requires.txt
--rwxrwx---   0 kzhou    (22264) domain users (10000)        6 2023-03-24 03:09:06.000000 PEALS-1.2.1/PEALS.egg-info/top_level.txt
--rwxrwx---   0 kzhou    (22264) domain users (10000)     4727 2023-03-24 03:09:06.608438 PEALS-1.2.1/PKG-INFO
--rwxrwx---   0 kzhou    (22264) domain users (10000)     3512 2023-03-24 02:57:50.000000 PEALS-1.2.1/README.md
-drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-03-24 03:09:06.601475 PEALS-1.2.1/bin/
--rwxrwx---   0 kzhou    (22264) domain users (10000)    20954 2023-03-24 02:57:50.000000 PEALS-1.2.1/bin/peals
--rwxrwx---   0 kzhou    (22264) domain users (10000)       38 2023-03-24 03:09:06.612418 PEALS-1.2.1/setup.cfg
--rwxrwx---   0 kzhou    (22264) domain users (10000)     2739 2023-03-24 02:57:50.000000 PEALS-1.2.1/setup.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.524844 PEALS-1.2.4/
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.365961 PEALS-1.2.4/PEALS/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       58 2023-06-30 04:14:26.000000 PEALS-1.2.4/PEALS/__init__.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.424328 PEALS-1.2.4/PEALS/collection/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       74 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/collection/__init__.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     8287 2023-06-30 04:14:24.000000 PEALS-1.2.4/PEALS/collection/bamtool.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    38218 2023-06-30 04:14:24.000000 PEALS-1.2.4/PEALS/collection/bedutils.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    25675 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/collection/functools.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    12628 2023-06-30 04:14:24.000000 PEALS-1.2.4/PEALS/collection/gfftools.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    15526 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/collection/optioncheck.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.455672 PEALS-1.2.4/PEALS/io/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       69 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/__init__.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     2074 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/constant.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     3454 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/paramlog.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     6489 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/report.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    16720 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/signals.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     2091 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/io/streamtools.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.471543 PEALS-1.2.4/PEALS/peak/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       37 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/peak/__init__.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    13530 2023-06-30 04:14:26.000000 PEALS-1.2.4/PEALS/peak/peakcall.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    34003 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/peak/peakutils.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.494281 PEALS-1.2.4/PEALS/stats/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       50 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/stats/__init__.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    14068 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/stats/correction.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    17568 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/stats/peaktest.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     4922 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/stats/statstools.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.510365 PEALS-1.2.4/PEALS/subcmd/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       44 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/subcmd/__init__.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     9278 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/subcmd/callpeak_cmd.py
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    14992 2023-06-30 04:14:25.000000 PEALS-1.2.4/PEALS/subcmd/diffpeak_cmd.py
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.392470 PEALS-1.2.4/PEALS.egg-info/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     4999 2023-06-30 04:49:55.000000 PEALS-1.2.4/PEALS.egg-info/PKG-INFO
+-rwxrwx---   0 kzhou    (22264) domain users (10000)      746 2023-06-30 04:49:57.000000 PEALS-1.2.4/PEALS.egg-info/SOURCES.txt
+-rwxrwx---   0 kzhou    (22264) domain users (10000)        1 2023-06-30 04:49:55.000000 PEALS-1.2.4/PEALS.egg-info/dependency_links.txt
+-rwxrwx---   0 kzhou    (22264) domain users (10000)      276 2023-06-30 04:49:55.000000 PEALS-1.2.4/PEALS.egg-info/requires.txt
+-rwxrwx---   0 kzhou    (22264) domain users (10000)        6 2023-06-30 04:49:55.000000 PEALS-1.2.4/PEALS.egg-info/top_level.txt
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     4999 2023-06-30 04:49:59.522621 PEALS-1.2.4/PKG-INFO
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     3776 2023-06-30 04:14:26.000000 PEALS-1.2.4/README.md
+drwxrwx---   0 kzhou    (22264) domain users (10000)        0 2023-06-30 04:49:59.515875 PEALS-1.2.4/bin/
+-rwxrwx---   0 kzhou    (22264) domain users (10000)    21414 2023-06-30 04:14:24.000000 PEALS-1.2.4/bin/peals
+-rwxrwx---   0 kzhou    (22264) domain users (10000)       38 2023-06-30 04:49:59.526289 PEALS-1.2.4/setup.cfg
+-rwxrwx---   0 kzhou    (22264) domain users (10000)     2780 2023-06-30 04:14:26.000000 PEALS-1.2.4/setup.py
```

### Comparing `PEALS-1.2.1/PEALS/collection/bamtool.py` & `PEALS-1.2.4/PEALS/collection/bamtool.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/collection/bedutils.py` & `PEALS-1.2.4/PEALS/collection/bedutils.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/collection/functools.py` & `PEALS-1.2.4/PEALS/collection/functools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 ##########################################
 #           utility                      #
-#          2021.8.5                      #
+#          2023.3.24                     #
 ##########################################
 __author__ = "Keren Zhou"
-__version__ = "v1.0"
+__version__ = "v1.2"
 
 import os
 import errno
 import sys
 import subprocess
 import statistics
 import networkx as nx
@@ -98,14 +98,37 @@
     if errorFlag is True:
         runResList = bytes.decode(subprocess.check_output(command, shell=True, stderr=None)).split('\n')
     else:
         runResList = bytes.decode(subprocess.check_output(command, shell=True, stderr=subprocess.PIPE)).split('\n')
     runResRowList = list(map(lambda x:x.split('\t'), list(filter(lambda x: bool(x), runResList))))
     return runResRowList
 
+def decodeSample(options):
+    ##column_name:value or column_name:control=value1,treated=value2
+    inforDict = {}
+    ## must have keys, ['column', 'control'] or ['column', 'control', 'treated']
+    column, infor = options.sample.split(':')
+    ## record column name
+    inforDict['column'] = column
+    ## record value
+    inforList = infor.split(',')
+    if options.subprogram == 'callpeak':
+        inforDict['value'] = inforList
+    elif options.subprogram == 'diffpeak':
+        valueList = []
+        ## decode value for each condition
+        for eachInfo in inforList:
+            condition, value = eachInfo.split('=')
+            inforDict[condition] = value
+            valueList.append(value)
+        valueList = list(set(valueList))
+        ## record all values
+        inforDict['value'] = valueList
+    return inforDict
+
 def getReadLength(bamFile):
     command = 'samtools view {} | head -n 100 | awk \'{{print $10}}\''.format(bamFile)
     readRowList = subprocessToList(command)
     readLenList = []
     for readRow in readRowList:
         read = readRow[0]
         readLenList.append(len(read))
@@ -218,18 +241,39 @@
         if os.path.islink(fileFullPath) is True:
             continue
         ## test.bam.bai
         baseName = fileFullPath.name
         binaryFileDict[baseName] = fileFullPath
     return binaryFileDict
 
+def subsetMatrix(options, matrixDf):
+    if options.sample is not None:
+        inforDict = decodeSample(options)
+        subsetCol = inforDict['column']
+        subsetValList = inforDict['value']
+        ## subset the matrix
+        matrixDf = matrixDf.loc[matrixDf[subsetCol].isin(subsetValList)]
+        ## check and change the condition for diffpeak
+        if options.subprogram == 'callpeak':
+            value = subsetValList[0]
+            matrixDf.loc[matrixDf[subsetCol] == value, 'condition'] = 'control'
+        elif options.subprogram == 'diffpeak':
+            ##rename the condition in sample matrix
+            conditionList = ['control', 'treated']
+            for condition in conditionList:
+                value = inforDict[condition]
+                matrixDf.loc[matrixDf[subsetCol] == value, 'condition'] = condition
+    return matrixDf
+
 def decodeMatrix(options):
     ## get sample matrix
     bamLinkDict = buildBamLinkDict(options)
     matrixDf = pd.read_csv(options.matrix, header=0, sep="\t", index_col=0, skiprows=0)
+    ## subset matrix if neeeded
+    matrixDf = subsetMatrix(options, matrixDf)
     ## load with binary files if necessary
     if options.binary is True:
         binaryFileDict = buildBinaryLinkDict(options)
         try:
             matrixDf['binary'] = list(map(lambda x: binaryFileDict[x], matrixDf['binary'].to_list()))
         except KeyError as e:
             options.error('No matched binary file found in --binary-dir!')
@@ -527,14 +571,15 @@
                 smoothValList = np.add(smoothForw, smoothBackw) / 2
             else:
                 smoothValList = bn.move_mean(smoothValList, window=span, min_count = 1)
     return smoothValList
 
 def smoothCsaps(options, npArr):
     spanmethod = options.spanmethod
+    spanloop = options.spanloop
     csapsp = options.csapsp
     maxSpan = options.spandict['max']
     minSpan = options.spandict['min']
     spanStep = options.spandict['step']
     ## make span not exceed array length
     optSpan = min(maxSpan, max(minSpan, int(npArr.size / spanStep)))
     indexArr = np.arange(npArr.size)
@@ -542,15 +587,15 @@
     weights = preprocessing.normalize([npArr], norm="l2")[0]
     weights[weights < csapsp] = weights[weights < csapsp] + csapsp
     weights[weights > 1] = 1
     smooth = 1 / math.log(indexArr.size) * csapsp
     try:
         csapsSmoothArr = csaps(indexArr, npArr, indexArr, weights=weights, smooth=smooth)
         ## smooth again with move average
-        npSmoothArr = smoothMove(csapsSmoothArr, 'move', span=optSpan, loop=1, backward=True)
+        npSmoothArr = smoothMove(csapsSmoothArr, 'move', span=optSpan, loop=spanloop, backward=True)
     except RuntimeError as e:
         npSmoothArr = smoothMove(npArr, 'move', span=optSpan, loop=3, backward=True)
     return npSmoothArr
 
 def findConGroup(npArr, stepSize=1):
     ##a = np.array([0, 47, 48, 49, 50, 97, 98, 99])
     ## return [array([0]), array([47, 48, 49, 50]), array([97, 98, 99])]
```

### Comparing `PEALS-1.2.1/PEALS/collection/gfftools.py` & `PEALS-1.2.4/PEALS/collection/gfftools.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/collection/optioncheck.py` & `PEALS-1.2.4/PEALS/collection/optioncheck.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,87 +24,102 @@
 
 from PEALS.collection import functools
 from PEALS.io.constant import *
 from PEALS.io import paramlog
 
 cpuCount = psutil.cpu_count()
 
+def exitError(message):
+    logging.error(message)
+    sys.exit(1)
+
 def parseError(option):
     message = "Error when parssing '--{}' option.".format(option)
     return message
 
 def parseAvail(values):
     optionValue = "{}".format(', '.join(map(str, values)))
     message = "Available values will be one of ({})".format(optionValue)
     return message
 
 def checkArgsEqual(option1, option2, optionName1, optionName2):
     if len(option1) != len(option2):
         logging.error("Error when parssing '--{}' and '--{}' option.".format(optionName1, optionName2))
-        logging.error("The number of input arguments of '--{}' and '--{}' option should be the same!".format(optionName1, optionName2))
-        sys.exit(1)
+        exitError("The number of input arguments of '--{}' and '--{}' option should be the same!".format(optionName1, optionName2))
 
 def checkThirdParty(options):
     logging.info("Checking whether required third party software are properly installed...")
     installFlag = True
     failureList = []
     for software in sorted(options.thirdparty.keys()):
         env = options.thirdparty[software]
         install = functools.checkSoftware(software, env)
         if install is False:
             failureList.append(software)
     if len(failureList) > 1:
         softwares = ', '.join(failureList)
-        logging.error("The following third party sofware is not installed or not found in your path environment: ({}).".format(softwares))
-        sys.exit(1)
+        exitError("The following third party sofware is not installed or not found in your path environment: ({}).".format(softwares))
     else:
         logging.info("Congratulations! All required third party software are properly installed!")
 
 def checkThead(options):
     if options.thread > 64:
         ## Value for argumant -T is out of range: 1 to 64, limited by featureCounts
         options.thread = 64
     elif options.thread <= 0:
         options.thread = 1
     return options
 
+def checkSample(options):
+    inforDict = functools.decodeSample(options)
+    count = len(inforDict['value'])
+    if options.subprogram == 'callpeak':
+        ##key: column,value
+        if count != 1:
+            exitError(parseError('sample'))
+    elif options.subprogram == 'diffpeak':
+        ##key: column,value,control,treated
+        keyList = sorted(inforDict.keys())
+        if 'control' not in keyList or 'treated' not in keyList:
+            exitError(parseError('sample'))
+        if count != 2:
+            exitError(parseError('sample'))
+    return inforDict
+
 def checkSplitSize(options):
     ## Value for split a transcript
     if options.txsizemax < 5000:
         options.txsizemax = 5000
-    elif options.txsizemax > 100000:
-        options.txsizemax = 100000
+    elif options.txsizemax > 50000:
+        options.txsizemax = 50000
     return options
 
 def checkVerbose(options):
     if options.verbose > 3:
         logging.error(parseError('verbose'))
-        logging.error(parseAvail([0, 1, 2, 3]))
-        sys.exit(1)
+        exitError(parseAvail([0, 1, 2, 3]))
 
 def chekFolder(folder, default, optionName):
     if folder is None:
         if default == 'cwd':
             folder = os.path.realpath(os.getcwd())
         else:
             folder = default
     else:
         try:
             os.makedirs(folder, exist_ok=True)
         except:
             logging.error(parseError(optionName))
-            logging.error("Output directory ({}) could not be created. Terminating program.".format(folder))
-            sys.exit(1)
+            exitError("Output directory ({}) could not be created. Terminating program.".format(folder))
 
 def checkArgsIsFile(*argsFiles, optionName):
     for argsFile in argsFiles:
         if os.path.isfile(argsFile) is False:
             logging.error(parseError(optionName))
-            logging.error("At least one invalid file detected in '--{}' option!".format(optionName))
-            sys.exit(1)
+            exitError("At least one invalid file detected in '--{}' option!".format(optionName))
 
 def readInputFromFile(fileList, optionName, extension):
     parsedFileList = []
     isFlag = True
     if len(fileList) == 1:
         ## check whether input is a valid file
         checkArgsIsFile(*fileList, optionName)
@@ -124,16 +139,15 @@
             return parsedFileList
         else:
             logging.error(parseError(optionName))
             logging.error("At least one file in the input is not with '{}' extension.".format(extension))
             sys.exit(1)
     else:
         logging.error(parseError(optionName))
-        logging.error("The input should be files with '{}' extension.".format(extension))
-        sys.exit(1)
+        exitError("The input should be files with '{}' extension.".format(extension))
 
 def checkInputFileOption(fileList, optionName, extension, readFlag=False):
     isFlag = True
     for File in fileList:
         ## check the extension
         fextend = os.path.splitext(os.path.basename(File))[-1]
         if fextend != extension:
@@ -144,16 +158,15 @@
         parsedFileList = readInputFromFile(fileList, optionName, extension)
         return parsedFileList
     else:
         return fileList
 
 def parssingMatrixError(message):
     logging.error(parseError('matrix'))
-    logging.error(message)
-    sys.exit(1)
+    exitError(message)
 
 def checkMatrixFile(options):
     ## check the header
     headerList = []
     idColValList = []
     with open(options.matrix, 'r') as f:
         headerList = f.readline().strip().split('\t')
@@ -163,29 +176,54 @@
     ## check whether the first column is id
     if headerList[0] != 'id':
         parssingMatrixError("The name of first column should be 'id'.")
     ## check whether id in 'id' column is unique
     if len(idColValList) != len(set(idColValList)):
         parssingMatrixError("The value of 'id' column should be unique.")
     ## check header
-    requiredColNameList = ["id", "library", "condition", "replicate", "label", "bam", "binary"]
+    #requiredColNameList = ["id", "library", "condition", "replicate", "label", "bam", "binary"]
+    requiredColNameList = ["id", "library", "condition", "replicate", "label", "bam"]
     for colName in requiredColNameList:
         if colName not in headerList:
-            parssingMatrixError("The column {} is required!".format(colName))
+            parssingMatrixError("The column ({}) is required!".format(colName))
     ##parsing sample matrix
     matrixDf = pd.read_csv(options.matrix, header=0, sep="\t", index_col=0, skiprows=0)
+    ## if needs to sample subset
+    if options.sample is not None:
+        inforDict = checkSample(options)
+        subsetCol = inforDict['column']
+        subsetValList = inforDict['value']
+        ## whether the column in matrix
+        if subsetCol not in matrixDf.columns:
+            parssingMatrixError("The column ({}) is not in sample matrix!".format(subsetCol))
+        ## subset the matrix
+        matrixDf = matrixDf.loc[matrixDf[subsetCol].isin(subsetValList)]
+        ## whether the subet matrix is empty
+        if matrixDf.empty is True:
+            values = ','.join(subsetValList)
+            parssingMatrixError("Values ({}) is not found in the column ({})in sample matrix!".format(values, subsetCol))
+        ## check and change the condition for diffpeak
+        if options.subprogram == 'callpeak':
+            value = subsetValList[0]
+            matrixDf.loc[matrixDf[subsetCol] == value, 'condition'] = 'control'
+        elif options.subprogram == 'diffpeak':
+            ##rename the condition in sample matrix
+            conditionList = ['control', 'treated']
+            for condition in conditionList:
+                value = inforDict[condition]
+                matrixDf.loc[matrixDf[subsetCol] == value, 'condition'] = condition
     ### check condition
     conditionList = sorted(matrixDf['condition'].unique())
     conditionCount = len(conditionList)
     if conditionCount == 1:
         if conditionList[0] != 'control' and conditionList[0] != 'treated':
-            parssingMatrixError("The value  in column 'condition' should be either 'control' or 'treated' when you have only 1 condition!")
+            parssingMatrixError("The value  in column 'condition' should be either 'control' or 'treated' when running 'callpeak' subcommand!")
     elif conditionCount == 2:
         if conditionList != ['control', 'treated']:
-            parssingMatrixError("The values in column 'condition' should be 'control' and 'treated' when you have 2 conditions!")
+            parssingMatrixError("The values in column 'condition' should be 'control' and 'treated' when running 'diffpeak' subcommand!")
     else:
         parssingMatrixError("Currently only support at most 2 conditions in a test ('control' and 'treat').")
     ## check library
     libraryList = sorted(matrixDf['library'].unique())
     if len(libraryList) == 2:
         for condition in conditionList:
             libraryList = sorted(matrixDf[ matrixDf['condition'] == condition ]['library'].unique())
@@ -234,29 +272,37 @@
     # setting logging object
     logging.basicConfig(level=(4-options.verbose)*10,
                         format='%(levelname)-5s @ %(asctime)s: %(message)s ',
                         datefmt='%a, %d %b %Y %H:%M:%S',
                         stream=sys.stderr,
                         filemode="w"
                         )
+    ## subprogram
+    options.subprogram = 'callpeak'
     # function alias
     options.error = logging.error
     options.warn  = logging.warning
     options.debug = logging.debug
     options.info  = logging.info
+    ## binary
+    options.reuse = False
+    options.binary = False
+    options.binaryapp = BINARY_APPENDIX
+    options.binarydir = None
     ## check sample matrix
     checkMatrixFile(options)
     # determin outputdir
     chekFolder(options.outputdir, 'cwd', 'output')
     # determin temdir
     chekFolder(options.tempdir, options.outputdir, 'temp')
+    # determin binarydir
+    chekFolder(options.binarydir, options.outputdir, 'binary')
     ## constant
     options.idsepdict = ID_SEP_DICT
     options.tempre = TEMP_PREFIX
-    options.binaryapp = BINARY_APPENDIX
     options.labelref = REF_PEAK_LABEL
     options.txoptsize = int(options.txsizemax * 0.2)
     options.spandict = SPAN_DICT
     options.version = VERSION
     ## construct peak regex
     peakidsep = options.idsepdict['peakid'].replace('|', '\\|')
     options.peakregex = r'{0}\d+{0}T$'.format(peakidsep)
@@ -284,29 +330,37 @@
     # setting logging object
     logging.basicConfig(level=(4-options.verbose)*10,
                         format='%(levelname)-5s @ %(asctime)s: %(message)s ',
                         datefmt='%a, %d %b %Y %H:%M:%S',
                         stream=sys.stderr,
                         filemode="w"
                         )
+    ## subprogram
+    options.subprogram = 'diffpeak'
     # function alias
     options.error = logging.error
     options.warn  = logging.warning
     options.debug = logging.debug
     options.info  = logging.info
+    ## binary
+    options.reuse = False
+    options.binary = False
+    options.binaryapp = BINARY_APPENDIX
+    options.binarydir = None
     ## check sample matrix
     checkMatrixFile(options)
     # determin outputdir
     chekFolder(options.outputdir, 'cwd', 'output')
     # determin temdir
     chekFolder(options.tempdir, options.outputdir, 'temp')
+    # determin binarydir
+    chekFolder(options.binarydir, options.outputdir, 'binary')
     ## constant
     options.idsepdict = ID_SEP_DICT
     options.tempre = TEMP_PREFIX
-    options.binaryapp = BINARY_APPENDIX
     options.labelref = REF_PEAK_LABEL
     options.txoptsize = int(options.txsizemax * 0.3)
     options.spandict = SPAN_DICT
     options.version = VERSION
     ## construct peak regex
     peakidsep = options.idsepdict['peakid'].replace('|', '\\|')
     options.peakregex = r'{0}\d+{0}T$'.format(peakidsep)
```

### Comparing `PEALS-1.2.1/PEALS/io/constant.py` & `PEALS-1.2.4/PEALS/io/constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # CONSTANT VALUE
-VERSION = '1.2.1'
+VERSION = '1.2.4'
 BUFFER_SIZE = 10000000
 THREAD = 10
 THREAD_START_METHOD="fork"
 MATH_RELTOL = 0.05
 MOVE_METHOD = "move"
 SMOOTH_LOOP = 1
 SMOOTH_SPAN = 25
 PEAK_SIZE = 35
 EXT_SIZE = 0
 LOOK_AHEAD = 25
 CSAPS_SMOOTH = 0.005
 IP_RATIO = 1.25
 CENTER = 0.25
 COMPLEXITY_RATE = 0.05
-SPAN_DICT = {'max':200, 'min':5, 'step':80}
+SPAN_DICT = {'max':200, 'min':2, 'step':100}
 TX_SPLIT_MAX_SIZE=50000
 TX_SPLIT_OPT_SIZE=int(TX_SPLIT_MAX_SIZE * 0.3)
 THIRD_PARTY_SOFTWARE = {'bedtools':['bash', '2.30.0'], \
                         'featureCounts':['bash', '2.0.2'], \
                         'samtools':['bash', '1.14'], \
                         'DESeq2':['R', '1.32.0'], \
                         'ashr':['R', '2.2.54'], \
```

### Comparing `PEALS-1.2.1/PEALS/io/paramlog.py` & `PEALS-1.2.4/PEALS/io/paramlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def glue(param, value):
     report = '{}={}'.format(param, value)
     return report
 
 def log(options):
     inputParamDict = {'inputdir':'input', 'matrix':'matrix', 'binarydir':'binary-dir', \
                       'binary':'call-with-binary', 'recursive':'recursive', 'rnatype':'type', \
+                      'sample':'sample', \
                      }
     outputParamDict = {'outputdir':'output', 'tempdir':'temp', 'prefix':'prefix', \
                       'nobwtrack':'no-bwtrack', 'keeptemp':'keep-temp', 'verbose':'verbose', \
                      }
     libraryParamDict = {'library':'library', 'estlibsize':'estlib-size', 'extsize':'extsize', \
                       'pairend':'pairend', \
                      }
```

### Comparing `PEALS-1.2.1/PEALS/io/report.py` & `PEALS-1.2.4/PEALS/io/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,18 +51,21 @@
             peakRowList[i][3] = options.idsepdict['peakid'].join(peakidRow)
     return peakRowList
 
 def peakReport(options, txBedDict, testResDf, peakRowList):
     ## peakRowList = [bed12Row, bed12Row, ...]
     peakBed = os.path.join(options.outputdir, options.prefix + '.bed')
     peakTxt = os.path.join(options.outputdir, options.prefix + '.txt')
+    ## drop rows contain nan, output from DESeq2
+    testResDf.dropna(how='any', inplace=True)
     ## get significant peaks
-    testResDf = getSigTestResDf(options, testResDf)
+    testSigResDf = getSigTestResDf(options, testResDf)
     ## sort testing results by log10padj
     testResDf = testResDf.sort_values(by=['log10padj'])
+    testSigResDf = testSigResDf.sort_values(by=['log10padj'])
     ## output bed
     bedRow = ['chrom', 'chromStart', 'chromEnd', 'name', 'score', 'strand']
     bedRow += ['thickStart', 'thickEnd', 'itemRgb', 'blockCount', 'blockSizes', 'blockStarts']
     txtRow = bedRow + ['log2FC', 'log10Pval', 'log10Padj', 'peakLength']
     if options.poolmode == 'pool':
         txtRow += ['ipMean', 'inputMean']
     else:
@@ -77,18 +80,23 @@
     peakBedDict = {}
     for peakRow in peakRowList:
         ## get peakid, geneid:txid|condition|number|T(|F)
         peakid = peakRow[3]
         peakBedDict[peakid] = peakRow[0:12]
     ## preparing for output
     uniqDict = defaultdict(int)
+    if options.poolmode == 'pool':
+        loopIndex = testSigResDf.index
+    else:
+        loopIndex = testResDf.index
+    ## output results
     with open(peakBed, 'w') as bedOut, open(peakTxt, 'w') as txtOut:
         bedOut.write('\t'.join(bedRow) + '\n')
         txtOut.write('\t'.join(txtRow) + '\n')
-        for peakid in testResDf.index:
+        for peakid in loopIndex:
             bedRow = peakBedDict[peakid]
             ## get peak annotations
             geneid, labelTxid = peakid.split(options.idsepdict['peakid'])[0].split(options.idsepdict['genetx'])
             #geneid, geneName, geneType, labelTxid, txName, txType = txBedDict[labelTxid].name.split(':')
             txidInforList = txBedDict[labelTxid].name.split(options.idsepdict['txinfo'])
             ## reget the transcript id
             txidInforList[3] = txidInforList[3].split(options.idsepdict['labeltxid'])[0]
@@ -117,11 +125,15 @@
                     tinputMean = peakTestRes['tinputMean']
                     txtRow += list(map(lambda x: round(x, 3), [cipMean, cinputMean, tipMean, tinputMean]))
                 else:
                     txtRow += list(map(lambda x: round(x, 3), [cipMean, tipMean]))
             ## add txid information
             txtRow += txidInforList
             ## output bed format
-            bedOut.write('\t'.join(map(str, bedRow)) + '\n')
             txtOut.write('\t'.join(map(str, txtRow)) + '\n')
+            if options.poolmode == 'pool':
+                bedOut.write('\t'.join(map(str, bedRow)) + '\n')
+            else:
+                if peakid in testSigResDf.index:
+                    bedOut.write('\t'.join(map(str, bedRow)) + '\n')
             ## output txt format
             uniqDict[geneid] += 1
```

### Comparing `PEALS-1.2.1/PEALS/io/signals.py` & `PEALS-1.2.4/PEALS/io/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     else:
         options.info('Use raw reads count to estimate the gene expression.'.format(expMethod))
     lengthDf = readCountDf.iloc[:, 0]
     countDf = readCountDf.iloc[:, range(1, readCountDf.shape[1])]
     totalReadDf = countDf.sum(axis=0)
     if expMethod == 'count':
         norExpDf = countDf
-    elif expMethod == 'FRPKM':
+    elif expMethod == 'FPKM':
         norExpDf = countDf.div(lengthDf, axis=0).div(totalReadDf, axis=1).multiply(1e9)
     elif expMethod == 'TPM':
         countPerbpDf = countDf.div(lengthDf, axis=0)
         norExpDf = countPerbpDf.div(countPerbpDf.sum(axis=0), axis=1).multiply(1e6)
     return norExpDf
 
 def getReadCountsDf(options, annoFile, annoType, bamFileList, normalize=False, keeplen=False):
@@ -327,33 +327,35 @@
         identifier = '-g {}'.format(options.identifier.split(':')[3])
         extsizeParam = ''
     ## count with fraction
     if options.nofraction is False:
         fractionParam = "--fraction"
     else:
         fractionParam = ''
-    uniqueParam = "-C -M -O {}".format(fractionParam)
+    ## fraction parameter
     fracOverlapParam = '--fracOverlap {}'.format(options.fracoverlap)
     ## whether to sort
     if options.sortbam is True:
         sortParam = ""
     else:
         sortParam = "--donotsort"
     ## deal with PCR duplicates
     if options.ignoredup is True:
         dupParam = "--ignoreDup"
     else:
         dupParam = ""
     ## count pair or extend
     if options.pairend is True:
         ##command = 'featureCounts -a {} -F {} {} -o {} -s {} -T {} -p {} --countReadPairs {} {} {}'
+        uniqueParam = "-C -M -O {}".format(fractionParam)
         ## remove the countReadParis will greatly speed-up the program
         command = 'featureCounts -a {} -F {} {} -o {} -s {} -T {} -p {} {} {} {} {}'
         command = command.format(annoFile, annoFormat, identifier, countTmp.name, options.library, options.thread, fracOverlapParam, uniqueParam, sortParam, dupParam, bamFileParam)
     else:
+        uniqueParam = "-M -O {}".format(fractionParam)
         command = 'featureCounts -a {} -F {} {} -o {} -s {} -T {} {} {} {} {} {} {}'
         command = command.format(annoFile, annoFormat, identifier, countTmp.name, options.library, options.thread, fracOverlapParam, extsizeParam, uniqueParam, sortParam, dupParam, bamFileParam)
     ## debug
     options.debug('Running featureCounts with command ({})...'.format(command))
     __ = functools.subprocessRun(command)
     ## debug
     options.debug('Running featureCounts done.')
```

### Comparing `PEALS-1.2.1/PEALS/io/streamtools.py` & `PEALS-1.2.4/PEALS/io/streamtools.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/peak/peakcall.py` & `PEALS-1.2.4/PEALS/peak/peakcall.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/peak/peakutils.py` & `PEALS-1.2.4/PEALS/peak/peakutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
     return [mlMargin, mrMargin, mMarginSize]
 
 def centerPeak(options, dataArr, ratio, cutoff):
     ## Center the candidate peak region by shearing points of which are less than --center of highest coverage
     peaksize = options.peaksize
     if ratio > 0:
         if ratio < 1:
-             center = options.center * ( 1 + ratio )
+            center = options.center * ( 1 + ratio )
         else:
             center = options.center * ( 1 + 1 / ratio )
     else:
         center = options.center
     ## make sure center percentage no more than 0.6
     if center > 0.6:
         center = 0.6
```

### Comparing `PEALS-1.2.1/PEALS/stats/correction.py` & `PEALS-1.2.4/PEALS/stats/correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     ## reorder the column
     geneNorInputReadCountDf = geneNorInputReadCountDf.reindex(columns=inputBamidList)
     ## construct gene counts to each peak
     peakGeneDict = defaultdict(list)
     for peakid in peakReadCountDf.index:
         geneid = peakid.split(options.idsepdict['peakid'])[0].split(options.idsepdict['genetx'])[0]
         peakGeneDict[geneid].append(peakid)
-    ## get read count df of peak
+    ## get IP read count df of peak
     peakIpDf = peakReadCountDf.loc[:, ipBamidList]
     ## copy peakIpDf to a new df
     peakGeneInputDf = peakIpDf.copy()
     geneidList = sorted(peakGeneDict.keys())
     geneidReadCountList = [ geneNorInputReadCountDf.loc[i, :].to_list() for i in geneidList ]
     for i in range(len(geneidList)):
         peakidList = peakGeneDict[geneidList[i]]
@@ -87,48 +87,48 @@
     ## using all corrected peak regions to calculate the IP enrichment factor
     peakIpFilterDf = peakIpDf.loc[peakidList, :]
     peakOnlyIpDf = peakIpFilterDf[peakIpFilterDf.index.str.contains(options.peakregex, regex = True)]
     if options.estipeff == 'within':
         ## normalize by the library size first
         libSizeDf = subMatrixDf.loc[ipBamidList, :]['lib_size']
         libSizeFactor = libSizeDf.div(libSizeDf.min())
-        options.debug("Normalize IP reads count by sequencing depth with library size factors:\n" + libSizeFactor.to_markdown())
+        options.info("Normalize IP reads count by sequencing depth with library size factors:\n" + libSizeFactor.to_markdown())
         peakNorIpDf = peakIpDf.div(libSizeFactor)
         ## get gene reads count df
         peakOnlyNorInputDf = peakGeneInputDf.loc[peakidList, ]
         ## normalize IP read counts per condition
         conditionList = ['control', 'treated']
         bamidList2d = [cipBamidList, tipBamidList]
         for i in range(2):
             condition = conditionList[i]
             bamidList = bamidList2d[i]
             ## divide the IP reads count by gene counts
             ipEfficiencyDf = peakOnlyIpDf.loc[:, bamidList].div(peakOnlyNorInputDf.loc[:, bamidList])
             ## determining the the size factor with median-of-ratio
             ipSizeFactorSeries = calMedianRatio(ipEfficiencyDf)
             ## debug
-            options.debug("Normalize IP read counts ({}) by estimated IP efficiency factor:\n".format(condition) + ipSizeFactorSeries.to_markdown())
+            options.info("Normalize IP read counts ({}) by estimated IP efficiency factor:\n".format(condition) + ipSizeFactorSeries.to_markdown())
             ## normalize by calcualted IP efficiency factors
             peakNorIpDf.loc[:, bamidList] = normalizeCountDf(peakNorIpDf.loc[:, bamidList], ipSizeFactorSeries)
     elif options.estipeff == 'across':
         ## only use peaks that are higher than 25% in all samples
-        options.debug("only use peaks that are higher than 25\% in all samples.")
-        peakOnlyIpDf = peakOnlyIpDf[ peakOnlyIpDf > peakOnlyIpDf.quantile(0.25) ]
+        options.info("only use top 50\% enriched peaks in all samples.")
+        peakOnlyIpDf = peakOnlyIpDf[ peakOnlyIpDf > peakOnlyIpDf.quantile(0.5) ]
         ## filter out rows contain NaN in any columns
         peakOnlyIpDf = peakOnlyIpDf[peakOnlyIpDf.notnull().all(1)]
         peakidList = peakOnlyIpDf.index.to_list()
-        options.debug("{} of peak candidates used for calculating the IP efficiency factors.".format(len(peakidList)))
+        options.info("{} of peak candidates used for calculating the IP efficiency factors.".format(len(peakidList)))
         ## retrive corresponding gene counts
         peakOnlyNorInputDf = peakGeneInputDf.loc[peakidList, ]
         ## divide the IP reads count by gene counts
         ipEfficiencyDf = peakOnlyIpDf.div(peakOnlyNorInputDf)
         ## determining the the size factor with median-of-ratio
         ipSizeFactorSeries = calMedianRatio(ipEfficiencyDf)
         ## debug
-        options.debug("Normalize IP read counts by estimated IP efficiency factor:\n" + ipSizeFactorSeries.to_markdown())
+        options.info("Normalize IP read counts by estimated IP efficiency factor:\n" + ipSizeFactorSeries.to_markdown())
         ## normalize by calcualted IP efficiency factors
         peakNorIpDf = normalizeCountDf(peakIpDf, ipSizeFactorSeries)
     return [peakNorIpDf, peakNorInputDf]
 
 def normalizeByEnrichmentByGenesum(options, peakReadCountDf):
     ## get bamidList
     bamidList = peakReadCountDf.columns
```

### Comparing `PEALS-1.2.1/PEALS/stats/peaktest.py` & `PEALS-1.2.4/PEALS/stats/peaktest.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,22 @@
     ## get the p-value to H0: p < p0, using pnbinom in R, get high precision of p-value
     k = robjects.FloatVector(inputReads.to_numpy())
     size = robjects.FloatVector(ipReads.to_numpy())
     log10PvalArr = np.array(robjects.r['pnbinom'](k, size, p0, log='TRUE')) / np.log(10)
     ## perform fdr corrections
     alpha = 0.05
     ## transfer 'BH' to 'padjmethod'
-    if options.padjmethod == 'BH':
-        padjmethod = 'BH'
-    else:
-        padjmethod = 'BY'
-    fdrArr = statstools.fdr_correction(mpmath.mpf(10) ** log10PvalArr, alpha=alpha, method=padjmethod)[1]
+    #if options.padjmethod == 'BH':
+    #    padjmethod = 'BH'
+    #else:
+    #    padjmethod = 'none'
+    #fdrArr = statstools.fdr_correction(mpmath.mpf(10) ** log10PvalArr, alpha=alpha, method=padjmethod)[1]
+    # use R to calculate the adjusted P-value
+    pvalArr = mpmath.mpf(10) ** log10PvalArr
+    fdrArr = np.array(robjects.r['p.adjust'](robjects.FloatVector(pvalArr), method = options.padjmethod))
     log10FdrArr = np.array([mpmath.log10(fdr) for fdr in fdrArr])
     ## example results
     ## array([-7.69204611e-02, -4.06128956e-02, -7.69204611e-02, ...,  -7.69204611e-02, -1.55633270e-01, -3.35241642e-06])
     log2FcArr = np.log2(ipReads.divide(inputReads)).to_numpy()
     dataArr = np.vstack((log2FcArr, log10PvalArr, log10FdrArr)).T
     nbinomResDf =  pd.DataFrame(data = dataArr, columns = ['log2fc', 'log10pval', 'log10padj'], index =peakReadCountNorDf.index)
     ## add reads to dataframe
@@ -277,15 +280,15 @@
         'shrink': shrink,
         'sep': sep,
         'outputPrefix': outputPrefix,
         'reduced': reduced,
         'padjmethod': options.padjmethod,
         'testmethod': options.test,
         'fittype': options.fittype,
-        "temp": tempPrefixName,
+        "temp": tempPrefix,
         'outputdir': options.outputdir,
         'plot': plot,
         'skipsize': skipsize,
         'skipsubplot': skipSubplot,
     }
     command = command.format(**runGlmNbinomTestArgsDict)
     ## running DESeq2
```

### Comparing `PEALS-1.2.1/PEALS/stats/statstools.py` & `PEALS-1.2.4/PEALS/stats/statstools.py`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/PEALS/subcmd/callpeak_cmd.py` & `PEALS-1.2.4/PEALS/subcmd/callpeak_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     ## prepare genome information
     ## info
     info("Reading information from chromosome size file.")
     options.chrsizedict = signals.readGenomeSize(options)
     ## info
     info("Reading information from input sample matrix file ({}).".format(os.path.basename(options.matrix)))
     options = functools.buildFullMatrix(options)
+    debug("The final information of input sample matrix file is as follow:{}".format(options.matrixdf.to_markdown()))
     ## output buildFullMatrix to tempory file
     fullMatrixFile = tempPrefix + '.fullmatrix.tmp'
     options.matrixdf.to_csv(fullMatrixFile, sep='\t', header=True, index=True)
     ## info
     info("Creating soft symbolic links to input bam and bai files.")
     functools.bamToSymlink(options)
     ## get inputs
@@ -115,31 +116,33 @@
     peakRowList = []
     if options.binary is True:
         ## read binary files into peakRowList
         bamidList = sorted(set(map(lambda x: options.bamdict[x], ipBamList)))
         binaryFileList = sorted(options.matrixdf.loc[bamidList, ]['binary'].unique())
         binaryFileForLog = ','.join(map(lambda x: os.path.basename(x), binaryFileList))
         info( READ_BINARY_LOG.format(binaryFileForLog) )
-        peakRowList = streamtools.readPeakFromMbb(binaryFileList, bufferSize=options.buffer, folder=None)
+        peakRowList = streamtools.readPeakFromMbb(binaryFileList, bufferSize=options.buffer, folder=options.binarydir)
     ## info
     info("Starting to call peaks on IP and input libraries...")
     for i in range(len(pairBamList3d)):
         bamList = pairBamList3d[i]
         label = labelList[i]
         subIpBamList, subInputBamList = bamList
         ipBamName = ','.join(map(lambda x:os.path.basename(x), subIpBamList))
         inputBamName = ','.join(map(lambda x:os.path.basename(x), subInputBamList))
         ## info
         info( CALL_PEAK_LOG.format(ipBamName, inputBamName) )
         ### running code
         perPeakRowList = peakcall.callPeak(options, txBedDict, subTxExpDf, bamList, label)
-        ## write peakRowList to binary file *.mbb
+        ''' just used for development
+        ## write peakRowList to binary file *.pb
         if label != options.labelref:
             binaryFile = functools.getCellByBam(options, subIpBamList[0], 'binary')
             pickle.dump( perPeakRowList, open(binaryFile, "wb") )
+        '''
         ## append peakRowList
         peakRowList.extend(perPeakRowList)
         ## info
         info( CALL_PEAK_DONE_LOG.format(ipBamName, inputBamName) )
     ## testing the significance
     sampleCount = max([len(ipBamList), len(inputBamList)])
     ## removing any duplicate bams
@@ -149,19 +152,14 @@
         ## info
         info("Performing statistical testing on peak candidates...")
         ### running code
         peakReadCountDf = peakutils.getPeakReadCountsDf(options, peakRowList, testBamList, normalize=False)
         testResDf = peaktest.runNbinomTest(options, peakReadCountDf)
         info("Statistical testing on peak candidates done.")
     else:
-        ### testing code
-        ####binaryFile = os.path.join(options.outputdir, 'pool_ref' + options.binaryapp)
-        ####pickle.dump( peakRowList, open(binaryFile, "wb") )
-        ####peakRowList = streamtools.readPeakFromMbb([binaryFile], bufferSize=options.buffer, folder=None)
-        ####streamtools.peakToFile(peakRowList, 'pool_ref.bed', bed12=False, folder=options.outputdir)
         ## info
         info("Finding consensus peak candidates from replicates...")
         ## running peak pooling
         peakRowList = peakutils.poolPeak(options, peakRowList, sampleCount, options.prefix, peakMode='intersect', txBedDict=None)
         ## info
         info("Performing statistical testing on peak candidates...")
         ## get reads of peakid
```

### Comparing `PEALS-1.2.1/PEALS/subcmd/diffpeak_cmd.py` & `PEALS-1.2.4/PEALS/subcmd/diffpeak_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     ## prepare genome information
     ## info
     info("Reading information from chromosome size file.")
     options.chrsizedict = signals.readGenomeSize(options)
     ## info
     info("Reading information from input sample matrix file ({}).".format(os.path.basename(options.matrix)))
     options = functools.buildFullMatrix(options)
+    debug("The final information of input sample matrix file is as follow:{}".format(options.matrixdf.to_markdown()))
     ## output buildFullMatrix to tempory file
     fullMatrixFile = tempPrefix + '.fullmatrix.tmp'
     options.matrixdf.to_csv(fullMatrixFile, sep='\t', header=True, index=True)
     ## info
     info("Creating soft symbolic links to input bam and bai files.")
     functools.bamToSymlink(options)
     ## assign arguments to variables
@@ -111,16 +112,18 @@
         info( "Trying to call peak candidates from control samples..." )
         controlPeakRowList = findPeakFromSample(options, txBedDict, cipBamList, cinputBamList, clabelList, geneExpDf, subTxExpDf, 'control')
         ## info
         info( "Trying to call peak candidates from treated samples..." )
         treatPeakRowList = findPeakFromSample(options, txBedDict, tipBamList, tinputBamList, tlabelList, geneExpDf, subTxExpDf, 'treated')
         info( "Merging peak candidates from control and treated conditions..." )
         peakRowList = controlPeakRowList + treatPeakRowList
+        ''' just used for development
         ### for reuse
         streamtools.dumpPeakToMbb(peakRowList, 'combine.peak.mbb', folder=options.outputdir)
+        '''
     else:
         ## info
         info("Reading \"combine.peak.mbb\" instead of calling peaks!")
         peakRowList = streamtools.readPeakFromMbb(['combine.peak.mbb'], bufferSize=options.buffer, folder=options.outputdir)
         tempCombinePeak = tempPrefix + '.combine.peak.bed'
         streamtools.peakToFile(peakRowList, tempCombinePeak, bed12=False, folder=None)
         info( "Merging peak candidates from control and treated conditions..." )
@@ -220,31 +223,33 @@
     peakRowList = []
     if options.binary is True:
         ## read binary files into peakRowList
         bamidList = sorted(set(map(lambda x: options.bamdict[x], ipBamList)))
         binaryFileList = sorted(options.matrixdf.loc[bamidList, ]['binary'].unique())
         binaryFileForLog = ','.join(map(lambda x: os.path.basename(x), binaryFileList))
         info( READ_BINARY_LOG.format(binaryFileForLog) )
-        peakRowList = streamtools.readPeakFromMbb(binaryFileList, bufferSize=options.buffer, folder=None)
+        peakRowList = streamtools.readPeakFromMbb(binaryFileList, bufferSize=options.buffer, folder=options.binarydir)
     ## info
     info("Starting to call peaks on IP and input libraries...")
     for i in range(len(pairBamList3d)):
         bamList = pairBamList3d[i]
         label = labelList[i]
         subIpBamList, subInputBamList = bamList
         ipBamName = ','.join(map(lambda x:os.path.basename(x), subIpBamList))
         inputBamName = ','.join(map(lambda x:os.path.basename(x), subInputBamList))
         ## info
         info( CALL_PEAK_LOG.format(ipBamName, inputBamName) )
         ### running code
         perPeakRowList = peakcall.callPeak(options, txBedDict, txExpDf, bamList, label)
+        ''' just used for development
         ## write peakRowList to binary file *.mbb
         if label != options.labelref:
             binaryFile = functools.getCellByBam(options, subIpBamList[0], 'binary')
             pickle.dump( perPeakRowList, open(binaryFile, "wb") )
+        '''
         ## append peakRowList
         peakRowList.extend(perPeakRowList)
         ## info
         info( CALL_PEAK_DONE_LOG.format(ipBamName, inputBamName) )
     ## testing the significance
     sampleCount = max([len(ipBamList), len(inputBamList)])
     ##testBamList = functools.removeDupBam(options, ipBamList + inputBamList)
```

### Comparing `PEALS-1.2.1/PEALS.egg-info/SOURCES.txt` & `PEALS-1.2.4/PEALS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PEALS-1.2.1/README.md` & `PEALS-1.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,53 +13,54 @@
 ## Required third party software
 
 PEALS relies on the following third party software. Before installing PEALS, please to ensure the following software have been properly installed.
 
  * [bedTools (>=2.30.0)](https://bedtools.readthedocs.io/en/latest/content/installation.html)
  * [samtools (>=1.14)](http://www.htslib.org/download/)
  * [featureCounts (>=2.0.2)](https://subread.sourceforge.net/featureCounts.html)
+
+The following R pacakges should be also installed.
+ * [getopt (>=1.20.3)](https://bioconductor.org/packages/release/bioc/html/DESeq2.html)
  * [DESeq2 (>=1.32.0)](https://bioconductor.org/packages/release/bioc/html/DESeq2.html)
  * [ggplot2 (>=3.4.1)](https://ggplot2.tidyverse.org/index.html)
+ * [ashr (>=2.2.54)](https://github.com/stephens999/ashr)
+ * [apeglm (>=1.14.0)](https://bioconductor.org/packages/release/bioc/html/apeglm.html)
+ * [glmGamPoi (>=1.4.0)](https://bioconductor.org/packages/release/bioc/html/glmGamPoi.html)
 
 ## Install
 
 The common way to install PEALS is through
-[PYPI](https://pypi.org/project/peals/)) or
-[INSTALL](./docs/INSTALL.md) document for detail.
+[PYPI](https://pypi.org/project/peals/)).
+
+Please check [INSTALL](./docs/INSTALL.md) document for detail.
 
 ## Usage
 
-Example for regular peak calling on MeRIP-seq:
+Example for regular peak calling on MeRIP-seq.
+
+For sample matrix, please chek the [sample matrix](./example/peals.callpeak.sample.txt) here as reference.
 
 `peals callpeak -i <bam directory> -m <sample matrix> -P <prefix> -o <output directory>`
 
-Example for differentially methylated peak calling on MeRIP-seq:
+Example for differentially methylated peak calling on MeRIP-seq.
+
+For sample matrix, please chek the [sample matrix](./example/peals.diffpeak.sample.txt) here as reference.
 
 `peals diffpeak -i <bam directory> -m <sample matrix> -P <prefix> -o <output directory>`
 
 
 Subcommand | Description
 -----------|----------
 [`callpeak`](./docs/callpeak.md) | Main function to call peaks from alignment results.
 [`diffpeak`](./docs/diffpeak.md) | Main function to call differentially methylated peaks from alignment results.
 
-For advanced usage, for example, to run `peals` in a modular way,
-please read the [advanced usage](./docs/advanced_usage.md). There is a
-[Q&A](./docs/qa.md) document where we collected some common questions
-from users.
-
 ## Contribute
-
-Please read our [CODE OF CONDUCT](./CODE_OF_CONDUCT.md) and
-[How to contribute](./CONTRIBUTING.md) documents. If you have any
-questions, suggestion/ideas, or just want to have conversions with
-developers and other users in the community, we recommand you use the
-[PEALS Discussions](https://github.com/peals-project/PEALS/discussions)
-instead of posting to our
-[Issues](https://github.com/peals-project/PEALS/issues) page.
+If you have any questions, suggestion/ideas, or just want to have conversions with
+developers and other users in the community, we recommand you using [discussion](https://github.com/kerenzhou062/PEALS/discussion) section or posting to our
+[Issues](https://github.com/kerenzhou062/PEALS/issues) page.
 
 ## Ackowledgement
 
 PEALS project also relies on the following python packages.
 
  * [CSAPS](https://pypi.org/project/csaps/)
  * [findpeaks](https://pypi.org/project/findpeaks/)
```

### Comparing `PEALS-1.2.1/bin/peals` & `PEALS-1.2.4/bin/peals`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     """Prepare optparser object. New options will be added in this
     function first.
     """
     description = "%(prog)s -- Peak-based Enhancement Analysis PipeLine for MeRIP-Seq"
     epilog = "For command line options of each command, type: %(prog)s COMMAND -h"
     # top-level parser
     argparser = ap.ArgumentParser( description = description, epilog = epilog ) #, usage = usage )
-    argparser.add_argument("--version", dest = "version", action="version", version="%(prog)s v"+ VERSION)
+    argparser.add_argument("-v", "--version", dest = "version", action="version", version="%(prog)s v"+ VERSION)
     subparsers = argparser.add_subparsers( dest = 'subcommand' ) #help="sub-command help")
     subparsers.required = True
 
     # command for 'callpeak'
     add_callpeak_parser( subparsers )
     # command for 'diffpeak'
     add_diffpeak_parser( subparsers )
@@ -57,53 +57,51 @@
 
 def add_input_option ( parser ):
     parser.add_argument("-i", "--input", dest = "inputdir", type = str,
                         required = True,
                         help = "Input directory contains all *.bam and *.bai files.")
     parser.add_argument("-m", "--matrix", dest = "matrix", type = str,
                         required = True,
-                        help = "The tab-separated matrix contain all information of input samples. Header format: label,library,condition,sample,replicate,bam,binary,...")
-    parser.add_argument("-b", "--binary-dir", dest = "binarydir", type = str,
-                        help = "The directory contains all binary files (*.mbb).")
-    parser.add_argument("--call-with-binary", dest = "binary", action="store_true",
-                        default=False,
-                        help = "Call peaks with binary inputs.")
+                        help = "The tab-separated matrix contain all information of input samples. Header format: label,library,condition,sample,replicate,bam,...")
     parser.add_argument("--recursive", dest = "recursive", action="store_true",
                         default=False,
                         help = "Recursively walk through --input to find *.bam and *.bai files.")
     parser.add_argument("--type", dest = "rnatype", action="store", 
                         choices = ['mature', 'primary', 'mixture'],
                         default='mature',
-                        help = "The type of RNA transcripts in input MeRIP library (mature: only contain mature transcripts; primary: only contain primary transcripts; mixture: contain both mature and primay transcripts).")
+                        help = "The type of RNA transcripts in input MeRIP library (mature: only contain mature transcripts; \
+                                primary: only contain primary transcripts; mixture: contain both mature and primay transcripts).")
 
 def add_output_option ( parser ):
     parser.add_argument("-o", "--output", dest = "outputdir", type = str,
                         required = True,
-                        help = "If specified, all output files will be written to this directory.")
+                        help = "All output files will be written to this directory.")
     parser.add_argument("-T", "--temp", dest = "tempdir", type = str,
                         help = "If specified, all temporary files will be written to this directory. Default is the same with --output.")
     parser.add_argument("-P", "--prefix", dest = "prefix", type = str,
                         required = True,
                         help = "The prefix of all output files")
     parser.add_argument("--no-bwtrack", dest = "nobwtrack", action='store_true',
                         default = False,
                         help = "If specified, will not output bigwig signal tracks which can be loaded in IGV.")
     parser.add_argument("--keep-temp", dest = "keeptemp", action='store_true',
                         default = False,
                         help = "Keep the temporary files")
     parser.add_argument( "--verbose", dest = "verbose", type = int,
                         choices=[0, 1, 2, 3],
                         default = 2,
-                        help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, 2: show process information, 3: show debug messages." )
+                        help = "Set verbose level of runtime message. 0: only show critical message, 1: show additional warning message, \
+                                2: show process information, 3: show debug messages." )
 
 def add_library_option ( parser ):
     parser.add_argument("-l", "--library", dest = "library", action="store", type=int,
                         choices = [0, 1, 2],
                         default = 2,
-                        help = "Library protocols of input bam files. For details, 0 (unstranded), 1 (stranded or fr-secondstrand) and 2 (reversely stranded or fr-firstrand).")
+                        help = "Library protocols of input bam files. For details, 0 (unstranded), 1 (stranded or fr-secondstrand) \
+                                and 2 (reversely stranded or fr-firstrand).")
     parser.add_argument("--estlib-size", dest = "estlibsize", action="store", type=str,
                         choices = ["primary", "mapped", "primary_mapped"],
                         default = "primary_mapped",
                         help = "How to estimate the library size when calling peaks and scaled bigwig outputs.")
     parser.add_argument("-e", "--extsize", dest = "extsize", type = int,
                         default = EXT_SIZE,
                         help = "Extend reads in 5\'->3\' direction to # bp (not recommend to be set when handling the paired-end data).")
@@ -115,15 +113,15 @@
     parser.add_argument("--exp-method", dest = "expmethod", type = str,
                         choices = ['count', 'TPM', 'FPKM'],
                         default = 'count',
                         help = "The method to estimate gene expression (mainly used for filter non-expressed genes).")
     parser.add_argument("--estpeak-sizefactor", dest = "peaksizefactor", type = str,
                         choices = ['peak', 'gene'],
                         default = 'peak',
-                        help = "How to normalize reads count of peak candidates for peak calling.")
+                        help = "How to normalize reads count of peak candidates for normalization before applying DESEq2 model.")
     parser.add_argument("--bw-scale", dest = "bwscale", type = str,
                         choices = ['raw', 'rpm', 'paired', 'whole'],
                         default = 'rpm',
                         help = "How to handle the signal track output (in bigwig format).")
 
 def add_bam_option ( parser ):
     parser.add_argument("--scale-sample", dest = "scalesample", type = str,
@@ -134,21 +132,21 @@
                         default = False,
                         help = "Sort bams before passing to featureCounts")
     parser.add_argument("--no-fraction", dest = "nofraction", action='store_true',
                         default = False,
                         help = "Do not count the multiple-aligned reads with fraction.")
     parser.add_argument("--frac-overlap", dest = "fracoverlap", type = float,
                         default = 0,
-                        help = "Only overlap fraction of reads larger than this value will count to peak.")
+                        help = "Only overlap # fraction of reads larger than this value will count to peak.")
     parser.add_argument("--ignore-dup", dest = "ignoredup", action='store_true',
                         default = False,
-                        help = "If specified, will ignore PCR duplicate reads.")
+                        help = "If specified, will ignore PCR duplicate reads flagged by '1024'.")
     parser.add_argument("--exp-cutoff", dest = "expcutoff", type = float,
                         default = 1,
-                        help = "The cutoff for an expressed transcript. Only call peaks on expressed transcripts")
+                        help = "The cutoff for an expressed transcript. Only call peaks on expressed transcripts.")
 
 def add_constant_option ( parser ):
     parser.add_argument("-t", "--thread", dest = "thread", type = int,
                         default = THREAD,
                         help = "How many threads used for parallel computation. Please note that more threads will use more physical and virtual memories.")
     parser.add_argument("-start", "--thread-start", dest = "threadstart", type = str,
                         choices=['forkserver', 'fork', 'spawn'],
@@ -203,15 +201,15 @@
     parser.add_argument("--peak-size", dest = "peaksize", type = int,
                         help = "The minimun peak size. Default is the maximum value between 'half of the --extsize' and '{}'.".format(PEAK_SIZE))
     parser.add_argument("--ipratio", dest = "ipratio", type = float,
                         default = IP_RATIO,
                         help = "Define the candidate peaks within which regions have the ratio of ip/input >= --ipratio.")
     parser.add_argument("--center", dest = "center", type = float,
                         default = CENTER,
-                        help = "Center the candidate peak region by shearing points of which are less than '--center' of highest coverage. Should be the range [0, 0.5]")
+                        help = "Center the candidate peak region by shearing points of which are less than '--center' of highest coverage. Should be the range [0, 0.5].")
 
 def add_model_option ( parser ):
     parser.add_argument("--fit-type", dest = "fittype", type = str,
                         choices = ["parametric", "local", "mean", "glmGamPoi"],
                         default = "parametric",
                         help = "Type of fitting of dispersions to the mean intensity (passed to DESeq2).")
     parser.add_argument("--shrink", dest = "shrink", action="store", type=str,
@@ -219,63 +217,69 @@
                         default = 'apeglm',
                         help='The method used for shrinking the fold change (lfcShrink() in DESeq2)')
     parser.add_argument("--test", dest = "test", action="store", type=str,
                         choices = ['Wald', 'LRT'],
                         default = "Wald",
                         help="The test method for calculating p-value (DESeq2).")
     parser.add_argument("--formula", dest = "formula", action="store", type=str,
-                        help="The design formula passed to DESeq2(). Will overwrite the default formula")
+                        help="The design formula passed to DESeq2(). Will overwrite the default formula.")
 
 def add_filter_option ( parser ):
     parser.add_argument("-p", "--pval", dest = "pvalcutoff", type = float,
                         default = 0.05,
                         help = "If specified, only peaks have p-value <= --pval will be recognized significant peaks.")
     parser.add_argument("-q", "--padj", dest = "padjcutoff", type = float,
                         default = 0.05,
                         help = "If specified, only peaks have adjusted p-value (FDR) <= --padj will be recognized significant peaks.")
     parser.add_argument("--padj-method", dest = "padjmethod", type = str,
+                        choices=["holm", "hochberg", "hommel", "bonferroni", "BH", "BY", "fdr", "none"],
                         default = 'BH',
                         help = "The method used to calculate adjusted p-value")
 
 def add_callpeak_parser( subparsers ):
     """Add main function 'peak calling' argument parsers.
     """
     argparser_callpeak = subparsers.add_parser("callpeak",
                                                formatter_class = ap.ArgumentDefaultsHelpFormatter,
                                                epilog = EPILOG_CALL_PEAK,
                                                help="Main PEALS Function: Call peaks from alignment results.")
     ## group for input
-    group_input = argparser_callpeak.add_argument_group( "Input files arguments" )
+    group_input = argparser_callpeak.add_argument_group( "Input options" )
     add_input_option( group_input )
+    ## add subset sample option
+    group_input.add_argument("-s", "--sample", dest = "sample", type = str,
+                        help = "If specified, will select samples in an additional column of sample matrix ('--matrix') used for testing \
+                        by the following format: \"column_name:value\", in which the value should be unique for each condition, \
+                        e.g., \"group:HeLa_control\".")
     ## group for output
-    group_output = argparser_callpeak.add_argument_group( "Output files arguments" )
+    group_output = argparser_callpeak.add_argument_group( "Output options" )
     add_output_option( group_output )
     ## group for library
-    group_library = argparser_callpeak.add_argument_group( "Sequencing library arguments" )
+    group_library = argparser_callpeak.add_argument_group( "Library options" )
     add_library_option( group_library )
     ## group for bam options
-    group_bam = argparser_callpeak.add_argument_group( "Bam options arguments" )
+    group_bam = argparser_callpeak.add_argument_group( "Bam options" )
     add_bam_option( group_bam )
     ## group for normalization options
-    group_normalize = argparser_callpeak.add_argument_group( "Normalization options arguments" )
+    group_normalize = argparser_callpeak.add_argument_group( "Normalization options" )
     add_normalize_option ( group_normalize )
     ## group for constant options
-    group_constant = argparser_callpeak.add_argument_group( "Constants arguments" )
+    group_constant = argparser_callpeak.add_argument_group( "Constants options" )
     add_constant_option( group_constant)
     ## group for constant options
-    group_anno = argparser_callpeak.add_argument_group( "Genome and gene annotation arguments" )
+    group_anno = argparser_callpeak.add_argument_group( "Genome options" )
     add_anno_option( group_anno )
     ## group for peak options
-    group_peak = argparser_callpeak.add_argument_group( "Peak detection arguments" )
+    group_peak = argparser_callpeak.add_argument_group( "Peak options" )
     add_peak_option( group_peak )
     ## group for model options
-    group_model = argparser_callpeak.add_argument_group( "Model arguments" )
+    group_model = argparser_callpeak.add_argument_group( "Model options" )
     add_model_option( group_model )
     ## group for filter options
-    group_filter = argparser_callpeak.add_argument_group( "Filter arguments" )
+    group_filter = argparser_callpeak.add_argument_group( "Filter options" )
     group_filter.add_argument("-f", "--fold", dest = "foldcutoff", type = float,
                         default = 2,
                         help = "If specified, only peaks have fold change (IP/input) (>= fold) will be recognized significant peaks.")
     add_filter_option( group_filter )
     ##
     return
 
@@ -283,50 +287,53 @@
     """Add main function 'peak calling' argument parsers.
     """
     argparser_callpeak = subparsers.add_parser("diffpeak",
                                                formatter_class = ap.ArgumentDefaultsHelpFormatter,
                                                epilog = EPILOG_DIFF_PEAK,
                                                help="Main PEALS Function: Call differential peaks from alignment results.")
     ## group for input
-    group_input = argparser_callpeak.add_argument_group( "Input files arguments" )
+    group_input = argparser_callpeak.add_argument_group( "Input files options" )
     add_input_option( group_input )
-    group_input.add_argument("--reuse", dest = "reuse", action="store_true",
-                    default=False,
-                    help = "Will read the \"combine.peak.mbb\" from output directory instead of calling peaks. Will not generate the bw track.")
+    ## add subset sample option
+    group_input.add_argument("-s", "--sample", dest = "sample", type = str,
+                        help = "If specified, will select samples in an additional column of sample matrix ('--matrix') used for testing \
+                        by the following format: \"column_name:control=value1,treated=value2\", \
+                        in which the value should be unique for each condition, \
+                        e.g., \"group:control=HeLa_control,treated=HeLa_treated\".")
     ## group for output
-    group_output = argparser_callpeak.add_argument_group( "Output files arguments" )
+    group_output = argparser_callpeak.add_argument_group( "Output files options" )
     add_output_option( group_output )
     ## group for library
-    group_library = argparser_callpeak.add_argument_group( "Sequencing library arguments" )
+    group_library = argparser_callpeak.add_argument_group( "Sequencing library options" )
     add_library_option( group_library )
     ## group for bam options
-    group_bam = argparser_callpeak.add_argument_group( "Bam options arguments" )
+    group_bam = argparser_callpeak.add_argument_group( "Bam options" )
     add_bam_option( group_bam )
     ## group for normalization options
-    group_normalize = argparser_callpeak.add_argument_group( "Normalization options arguments" )
+    group_normalize = argparser_callpeak.add_argument_group( "Normalization options" )
     add_normalize_option ( group_normalize )
     group_normalize.add_argument("--estip-eff", dest = "estipeff", type = str,
                         choices = ['across', 'within'],
                         default = 'within',
                         help = "How estimate the IP efficiency factors of control and treated conditions. If 'within' is specified, it will estimate IP efficiency factors within each condition, repspectively. \
                         If 'across' is specified, will estimate IP efficiency factors across 2 conditions (may introduce over-estimation).")
     ## group for constant options
-    group_constant = argparser_callpeak.add_argument_group( "Constants arguments" )
+    group_constant = argparser_callpeak.add_argument_group( "Constants options" )
     add_constant_option( group_constant)
     ## group for constant options
-    group_anno = argparser_callpeak.add_argument_group( "Genome and gene annotation arguments" )
+    group_anno = argparser_callpeak.add_argument_group( "Genome and gene annotation options" )
     add_anno_option( group_anno )
     ## group for peak options
-    group_peak = argparser_callpeak.add_argument_group( "Peak detection arguments" )
+    group_peak = argparser_callpeak.add_argument_group( "Peak detection options" )
     add_peak_option( group_peak )
     ## group for model options
-    group_model = argparser_callpeak.add_argument_group( "Model arguments" )
+    group_model = argparser_callpeak.add_argument_group( "Model options" )
     add_model_option( group_model )
     ## group for filter options
-    group_filter = argparser_callpeak.add_argument_group( "Filter arguments" )
+    group_filter = argparser_callpeak.add_argument_group( "Filter options" )
     group_filter.add_argument("-f", "--fold", dest = "foldcutoff", type = float,
                         default = 2,
                         help = "If specified, only peaks have fold change (IP/input) in either conditions (>= fold) will be recognized significant peaks.")
     add_filter_option( group_filter )
     group_filter.add_argument("-F", "--diff-fold", dest = "difffoldcutoff", type = float,
                         default = 1,
                         help = "If specified, only peaks have fold change (IP/input) (>= fold or <= 1/fold) will be recognized significantly changed peaks.")
@@ -344,8 +351,8 @@
     try:
         main()
     except KeyboardInterrupt:
         sys.stderr.write("User interrupted me! ;-) Bye!\n")
         sys.exit(0)
     except MemoryError:
         sys.exit( "MemoryError occurred. Please try to run with less threads." )
-        sys.exit(1)
+        sys.exit(1)
```

### Comparing `PEALS-1.2.1/setup.py` & `PEALS-1.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 installRequires = [ "numpy>=1.21.2",
                      "pandas>=1.1.4",
                      "scipy>=1.7.1",
                      "pysam>=0.16.0.1",
                      "psutil>=5.9.4",
                      "pyBigWig>=0.3.18",
                      "tqdm>=4.64.1",
+                     "tabulate>=0.8.7",
                      "rpy2>=3.4.5",
                      "mpmath>=1.1.0",
                      "findpeaks>=2.4.6",
                      "csaps>=1.1.0",
                      "bottleneck>=1.3.2",
                      "scikit-learn>=0.24.2",
                      "networkx>=2.5.1",
@@ -57,24 +58,24 @@
         sys.exit(1)
 
     with open("README.md", "r") as fh:
         longDescription = fh.read()
 
     setup( name = "PEALS",
            version = VERSION,
-           description = "Peak-based Enhancement Analysis Pipeline for MeRIP-Seq",
+           description = "Peak-based Enhancement Analysis PipeLine for MeRIP-Seq",
            long_description = longDescription,
            long_description_content_type = "text/markdown",
            include_package_data=True,
            author = 'Keren Zhou',
            author_email = 'zhoukr062@gmail.com',
            url = 'http://github.com/kerenzhou062/PEALS/',
            package_dir = {'PEALS' : 'PEALS'},
            packages = ['PEALS', 'PEALS.io', 'PEALS.collection', 'PEALS.peak', 'PEALS.stats', 'PEALS.subcmd'],
-           package_data = {'PEALS.stats':['*.R']},
+           package_data = {'PEALS.stats':['*.R'],},
            scripts = ['bin/peals', ],
            classifiers = classifiers,
            install_requires = installRequires,
            setup_requires = installRequires,
            tests_require = testsRequires,
            python_requires = '>=3.8' )
```

