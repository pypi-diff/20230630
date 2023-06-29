# Comparing `tmp/amazon_kclpy-2.1.1.tar.gz` & `tmp/amazon_kclpy-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_kclpy-2.1.1.tar", last modified: Wed Jan 18 19:22:44 2023, max compression
+gzip compressed data, was "amazon_kclpy-2.1.2.tar", last modified: Thu Jun 29 22:14:58 2023, max compression
```

## Comparing `amazon_kclpy-2.1.1.tar` & `amazon_kclpy-2.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)    10142 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/LICENSE.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)       72 2023-01-18 00:37:46.000000 amazon_kclpy-2.1.1/MANIFEST.in
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      114 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/NOTICE.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      349 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/PKG-INFO
--rw-r--r--   0 yuzen    (13046794) amazon     (100)    16736 2023-01-18 00:42:38.000000 amazon_kclpy-2.1.1/README.md
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      827 2022-12-07 19:46:26.000000 amazon_kclpy-2.1.1/amazon_kclpy/__init__.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      781 2022-12-07 19:46:36.000000 amazon_kclpy-2.1.1/amazon_kclpy/checkpoint_error.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     1839 2022-12-07 19:46:42.000000 amazon_kclpy-2.1.1/amazon_kclpy/dispatch.py
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy/jars/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)        0 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/jars/__init__.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)    12498 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/kcl.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)    13819 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/messages.py
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy/v2/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      820 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/v2/__init__.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     5308 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/v2/processor.py
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy/v3/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      820 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/v3/__init__.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     5583 2021-12-29 18:08:16.000000 amazon_kclpy-2.1.1/amazon_kclpy/v3/processor.py
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      349 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/PKG-INFO
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      776 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/SOURCES.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)        1 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/dependency_links.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)        1 2022-12-06 18:28:46.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/not-zip-safe
--rw-r--r--   0 yuzen    (13046794) amazon     (100)       14 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/requires.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)       53 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/amazon_kclpy.egg-info/top_level.txt
--rw-r--r--   0 yuzen    (13046794) amazon     (100)    13690 2023-01-13 02:44:25.000000 amazon_kclpy-2.1.1/pom.xml
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/samples/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     2741 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/samples/__init__.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     7176 2022-12-06 19:15:29.000000 amazon_kclpy-2.1.1/samples/amazon_kclpy_helper.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     4281 2023-01-04 22:42:07.000000 amazon_kclpy-2.1.1/samples/sample.properties
--rwxr-xr-x   0 yuzen    (13046794) amazon     (100)     6915 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/samples/sample_kclpy_app.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     5706 2023-01-13 02:52:47.000000 amazon_kclpy-2.1.1/samples/sample_kinesis_wordputter.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)      104 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/setup.cfg
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     8728 2023-01-18 00:40:46.000000 amazon_kclpy-2.1.1/setup.py
-drwxr-xr-x   0 yuzen    (13046794) amazon     (100)        0 2023-01-18 19:22:44.000000 amazon_kclpy-2.1.1/test/
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     3791 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/test/test_amazon_kclpy.py
--rw-r--r--   0 yuzen    (13046794) amazon     (100)     3925 2021-12-10 20:32:26.000000 amazon_kclpy-2.1.1/test/test_amazon_kclpy_input_output_integration.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)    10142 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/LICENSE.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)       72 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/MANIFEST.in
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      114 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/NOTICE.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      351 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/PKG-INFO
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)    17303 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/README.md
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      827 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/__init__.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      781 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/checkpoint_error.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     1839 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/dispatch.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/jars/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/jars/__init__.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)    12498 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/kcl.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)    13819 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/messages.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/v2/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      820 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v2/__init__.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5308 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v2/processor.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy/v3/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      820 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v3/__init__.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5583 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/amazon_kclpy/v3/processor.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.391020 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      351 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/PKG-INFO
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      776 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)        1 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)        1 2023-06-29 21:55:36.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/not-zip-safe
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)       14 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/requires.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)       53 2023-06-29 22:14:58.000000 amazon_kclpy-2.1.2/amazon_kclpy.egg-info/top_level.txt
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)    14075 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/pom.xml
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/samples/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     2741 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/__init__.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     7176 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/amazon_kclpy_helper.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     4573 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample.properties
+-rwxr-xr-x   0 rmpelaez (23627871) amazon     (100)     6915 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample_kclpy_app.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     5706 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/samples/sample_kinesis_wordputter.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)      104 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/setup.cfg
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     8728 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/setup.py
+drwxr-xr-x   0 rmpelaez (23627871) amazon     (100)        0 2023-06-29 22:14:58.395020 amazon_kclpy-2.1.2/test/
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     3791 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/test/test_amazon_kclpy.py
+-rw-r--r--   0 rmpelaez (23627871) amazon     (100)     3925 2023-06-29 21:43:26.000000 amazon_kclpy-2.1.2/test/test_amazon_kclpy_input_output_integration.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `amazon_kclpy-2.1.1/LICENSE.txt` & `amazon_kclpy-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/README.md` & `amazon_kclpy-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,20 @@
 * The [Amazon KCL for Java][kinesis-github]
 * The [Amazon KCL for Ruby][amazon-kinesis-ruby-github]
 * The [Amazon Kinesis Documentation][amazon-kinesis-docs]
 * The [Amazon Kinesis Forum][kinesis-forum]
 
 ## Release Notes
 
+### Release 2.1.2 (June 29, 2023)
+* Added the ability to pass in streamArn to multilang Daemon [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
+* Upgraded KCL and KCL-Multilang Dependencies from 2.4.4 to 2.5.1 [PR #221](https://github.com/awslabs/amazon-kinesis-client-python/pull/221)
+* Upgraded Google Guava dependency from 31.0.1-jre to 32.0.0-jre [PR #223](https://github.com/awslabs/amazon-kinesis-client-python/pull/223)
+* Added aws-java-sdk-sts dependency [PR #212](https://github.com/awslabs/amazon-kinesis-client-python/pull/212)
+
 ### Release 2.1.1 (January 17, 2023)
 * Include the pom file in MANIFEST
 
 ### Release 2.1.0 (January 12, 2023)
 * Upgraded to use version 2.4.4 of the [Amazon Kinesis Client library][kinesis-github]
 
 ### Release 2.0.6 (November 23, 2021)
```

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/__init__.py` & `amazon_kclpy-2.1.2/amazon_kclpy/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/checkpoint_error.py` & `amazon_kclpy-2.1.2/amazon_kclpy/checkpoint_error.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/dispatch.py` & `amazon_kclpy-2.1.2/amazon_kclpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/kcl.py` & `amazon_kclpy-2.1.2/amazon_kclpy/kcl.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/messages.py` & `amazon_kclpy-2.1.2/amazon_kclpy/messages.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/v2/__init__.py` & `amazon_kclpy-2.1.2/amazon_kclpy/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/v2/processor.py` & `amazon_kclpy-2.1.2/amazon_kclpy/v2/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/v3/__init__.py` & `amazon_kclpy-2.1.2/amazon_kclpy/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy/v3/processor.py` & `amazon_kclpy-2.1.2/amazon_kclpy/v3/processor.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/amazon_kclpy.egg-info/SOURCES.txt` & `amazon_kclpy-2.1.2/amazon_kclpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/pom.xml` & `amazon_kclpy-2.1.2/pom.xml`

 * *Files 1% similar despite different names*

#### Comparing `amazon_kclpy-2.1.1/pom.xml` & `amazon_kclpy-2.1.2/pom.xml`

```diff
@@ -9,20 +9,20 @@
     <fasterxml-jackson.version>2.13.4</fasterxml-jackson.version>
     <logback.version>1.3.0</logback.version>
   </properties>
   <dependencies>
     <dependency>
       <groupId>software.amazon.kinesis</groupId>
       <artifactId>amazon-kinesis-client-multilang</artifactId>
-      <version>2.4.4</version>
+      <version>2.5.1</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.kinesis</groupId>
       <artifactId>amazon-kinesis-client</artifactId>
-      <version>2.4.4</version>
+      <version>2.5.1</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.awssdk</groupId>
       <artifactId>kinesis</artifactId>
       <version>${awssdk.version}</version>
     </dependency>
     <dependency>
@@ -132,14 +132,19 @@
     </dependency>
     <dependency>
       <groupId>software.amazon.awssdk</groupId>
       <artifactId>apache-client</artifactId>
       <version>${awssdk.version}</version>
     </dependency>
     <dependency>
+      <groupId>software.amazon.awssdk</groupId>
+      <artifactId>arns</artifactId>
+      <version>${awssdk.version}</version>
+    </dependency>
+    <dependency>
       <groupId>io.netty</groupId>
       <artifactId>netty-codec-http</artifactId>
       <version>${netty.version}</version>
     </dependency>
     <dependency>
       <groupId>io.netty</groupId>
       <artifactId>netty-codec-http2</artifactId>
@@ -199,15 +204,15 @@
       <groupId>org.reactivestreams</groupId>
       <artifactId>reactive-streams</artifactId>
       <version>1.0.3</version>
     </dependency>
     <dependency>
       <groupId>com.google.guava</groupId>
       <artifactId>guava</artifactId>
-      <version>31.0.1-jre</version>
+      <version>32.0.0-jre</version>
     </dependency>
     <dependency>
       <groupId>com.google.code.findbugs</groupId>
       <artifactId>jsr305</artifactId>
       <version>3.0.2</version>
     </dependency>
     <dependency>
@@ -292,14 +297,19 @@
     </dependency>
     <dependency>
       <groupId>com.amazonaws</groupId>
       <artifactId>aws-java-sdk-core</artifactId>
       <version>${aws-java-sdk.version}</version>
     </dependency>
     <dependency>
+      <groupId>com.amazonaws</groupId>
+      <artifactId>aws-java-sdk-sts</artifactId>
+      <version>${aws-java-sdk.version}</version>
+    </dependency>
+    <dependency>
       <groupId>software.amazon.ion</groupId>
       <artifactId>ion-java</artifactId>
       <version>1.5.1</version>
     </dependency>
     <dependency>
       <groupId>software.amazon.glue</groupId>
       <artifactId>schema-registry-serde</artifactId>
```

### Comparing `amazon_kclpy-2.1.1/samples/__init__.py` & `amazon_kclpy-2.1.2/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/samples/amazon_kclpy_helper.py` & `amazon_kclpy-2.1.2/samples/amazon_kclpy_helper.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/samples/sample.properties` & `amazon_kclpy-2.1.2/samples/sample.properties`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # The script that abides by the multi-language protocol. This script will
 # be executed by the MultiLangDaemon, which will communicate with this script
 # over STDIN and STDOUT according to the multi-language protocol.
 executableName = sample_kclpy_app.py
 
+# The Stream arn: arn:aws:kinesis:<region>:<account id>:stream/<stream name>
+# Important: streamArn takes precedence over streamName if both are set
+streamArn = arn:aws:kinesis:us-east-5:000000000000:stream/kclpysample
+
 # The name of an Amazon Kinesis stream to process.
+# Important: streamArn takes precedence over streamName if both are set
 streamName = kclpysample
 
 # Used by the KCL as the name of this application. Will be used as the name
 # of an Amazon DynamoDB table which will store the lease and checkpoint
 # information for workers with this application name
 applicationName = PythonKCLSample
```

### Comparing `amazon_kclpy-2.1.1/samples/sample_kclpy_app.py` & `amazon_kclpy-2.1.2/samples/sample_kclpy_app.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/samples/sample_kinesis_wordputter.py` & `amazon_kclpy-2.1.2/samples/sample_kinesis_wordputter.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/setup.py` & `amazon_kclpy-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #
 # Will retrieve the configured jars from maven and then advise the user
 # to rerun the install command.
 #
 
 PACKAGE_NAME = 'amazon_kclpy'
 JAR_DIRECTORY = os.path.join(PACKAGE_NAME, 'jars')
-PACKAGE_VERSION = '2.1.1'
+PACKAGE_VERSION = '2.1.2'
 PYTHON_REQUIREMENTS = [
     'boto',
     # argparse is part of python2.7 but must be declared for python2.6
     'argparse',
 ]
 REMOTE_MAVEN_PACKAGES_FILE = 'pom.xml'
```

### Comparing `amazon_kclpy-2.1.1/test/test_amazon_kclpy.py` & `amazon_kclpy-2.1.2/test/test_amazon_kclpy.py`

 * *Files identical despite different names*

### Comparing `amazon_kclpy-2.1.1/test/test_amazon_kclpy_input_output_integration.py` & `amazon_kclpy-2.1.2/test/test_amazon_kclpy_input_output_integration.py`

 * *Files identical despite different names*

