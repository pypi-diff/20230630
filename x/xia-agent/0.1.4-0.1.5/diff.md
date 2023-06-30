# Comparing `tmp/xia_agent-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_agent-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3689 bytes, number of entries: 7
--rw-r--r--  2.0 unx      145 b- defN 23-Jun-29 20:38 xia_agent/__init__.py
+Zip file size: 3608 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-30 11:16 xia_agent/__init__.py
 -rw-r--r--  2.0 unx     7183 b- defN 23-Jun-29 20:32 xia_agent/agent.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:41 xia_agent-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      686 b- defN 23-Jun-29 20:41 xia_agent-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:41 xia_agent-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 20:41 xia_agent-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 23-Jun-29 20:41 xia_agent-0.1.4.dist-info/RECORD
-7 files, 8824 bytes uncompressed, 2711 bytes compressed:  69.3%
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      462 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jun-30 11:17 xia_agent-0.1.5.dist-info/RECORD
+7 files, 8600 bytes uncompressed, 2630 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_agent/__init__.py
 Comment: 
 
 Filename: xia_agent/agent.py
 Comment: 
 
-Filename: xia_agent-0.1.4.dist-info/LICENSE.txt
+Filename: xia_agent-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_agent-0.1.4.dist-info/METADATA
+Filename: xia_agent-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_agent-0.1.4.dist-info/WHEEL
+Filename: xia_agent-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_agent-0.1.4.dist-info/top_level.txt
+Filename: xia_agent-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_agent-0.1.4.dist-info/RECORD
+Filename: xia_agent-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_agent/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_agent.agent import Agent, AgentFunction, MetaFunction
 
 __all__ = [
     "Agent", "AgentFunction", "MetaFunction"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

