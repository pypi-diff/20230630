# Comparing `tmp/rosetta-ce-1.3.5.tar.gz` & `tmp/rosetta-ce-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.5.tar", last modified: Fri Jun 30 09:38:33 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.6.tar", last modified: Fri Jun 30 11:53:22 2023, max compression
```

## Comparing `rosetta-ce-1.3.5.tar` & `rosetta-ce-1.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.690719 rosetta-ce-1.3.5/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.5/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:38:33.690377 rosetta-ce-1.3.5/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.5/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.684242 rosetta-ce-1.3.5/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.5/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.686149 rosetta-ce-1.3.5/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.5/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.5/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.5/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    39169 2023-06-30 09:38:06.000000 rosetta-ce-1.3.5/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.5/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.688181 rosetta-ce-1.3.5/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 09:38:33.000000 rosetta-ce-1.3.5/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 09:38:33.690764 rosetta-ce-1.3.5/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 09:38:19.000000 rosetta-ce-1.3.5/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:38:33.689791 rosetta-ce-1.3.5/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.5/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.5/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.5/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 11:53:22.169448 rosetta-ce-1.3.6/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.6/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 11:53:22.168897 rosetta-ce-1.3.6/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.6/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 11:53:22.161701 rosetta-ce-1.3.6/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.6/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 11:53:22.165642 rosetta-ce-1.3.6/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.6/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.6/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.6/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.6/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.6/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    41965 2023-06-30 11:52:24.000000 rosetta-ce-1.3.6/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.6/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 11:53:22.167378 rosetta-ce-1.3.6/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 11:53:22.000000 rosetta-ce-1.3.6/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 11:53:22.000000 rosetta-ce-1.3.6/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 11:53:22.000000 rosetta-ce-1.3.6/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 11:53:22.000000 rosetta-ce-1.3.6/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 11:53:22.000000 rosetta-ce-1.3.6/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 11:53:22.169493 rosetta-ce-1.3.6/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 11:53:05.000000 rosetta-ce-1.3.6/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 11:53:22.168469 rosetta-ce-1.3.6/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.6/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.6/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.6/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.5/LICENSE` & `rosetta-ce-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/PKG-INFO` & `rosetta-ce-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.5
+Version: 1.3.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.5/README.md` & `rosetta-ce-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta/constants/sensors.py` & `rosetta-ce-1.3.6/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta/constants/sources.py` & `rosetta-ce-1.3.6/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta/constants/systems.py` & `rosetta-ce-1.3.6/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta/rconverter.py` & `rosetta-ce-1.3.6/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta/rfaker.py` & `rosetta-ce-1.3.6/rosetta/rfaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,47 +474,82 @@
              'LEEF:1.0|Leef|Payment Portal|1.0|192.168.0.1|mycomputer|08:00:27:da:2e:2e|08:00:27:da:2e:2f|src=10.0.0.2
               dst=mycomputer spt=57251 dpt=443 request=https://example.com/admin.php?sessionid=12345 method=POST
                proto=HTTP/1.1 status=404 request_size=1216 response_size=9729 user_agent=Mozilla/5.0
                (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3']
         """
         leef_messages = []
         faker = cls._create_faker()
+        vendor = vendor or faker.company()
         version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
-        for i in range(count):
-            timestamp += timedelta(seconds=1)
-            vendor = vendor or faker.company()
-            product = product or "Application Server"
-            src_port = faker.random_int(min=1024, max=65535)
-            request_size = faker.random_int(min=100, max=10000)
-            response_size = faker.random_int(min=100, max=10000)
-            user_agent = faker.user_agent()
-            host = random.choice(observables.src_host) if observables and observables.src_host \
-                else faker.hostname()
-            src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
-                else faker.ipv4()
-            url = random.choice(observables.technique).get('indicator') if observables and observables.technique \
-                else random.choice(TECHNIQUES).get('indicator')
-            file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
-                else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD, count=1)
-            method = random.choice(observables.technique).get('mechanism') if observables and observables.technique \
-                else random.choice(TECHNIQUES).get('mechanism')
-            error_code = random.choice(observables.error_code) if observables and observables.error_code \
-                else random.choice(ERROR_CODE)
-
-            leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|" \
-                       f"{faker.mac_address()}|{faker.mac_address()}|"
-            leef_log += f"src={src_ip} dst={host} spt={src_port} dpt=443 request={url} "
-            leef_log += f"method={method} proto=HTTP/1.1 status={str(error_code)} hash={file_hash}"
-            leef_log += f"request_size={request_size} " \
-                        f"response_size={response_size} "
-            leef_log += f"user_agent={user_agent}"
-            leef_messages.append(leef_log)
+        if product == "WAF":
+            for i in range(count):
+                timestamp += timedelta(seconds=1)
+                severity = random.choice(observables.severity) if observables and observables.severity \
+                    else faker.random_int(min=1, max=5)
+                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
+                    else faker.ipv4()
+                src_port = faker.random_int(min=1024, max=65535)
+                host = random.choice(observables.src_host) if observables and observables.src_host \
+                    else faker.hostname()
+                method = random.choice(observables.technique).get('mechanism') if observables and observables.technique \
+                    else random.choice(TECHNIQUES).get('mechanism')
+                url = random.choice(observables.technique).get('indicator') if observables and observables.technique \
+                    else random.choice(TECHNIQUES).get('indicator')
+                protocol = random.choice(observables.protocol) if observables and observables.protocol \
+                    else random.choice(PROTOCOLS)
+                user_agent = faker.user_agent()
+                referer = random.choice(observables.url) if observables and observables.url \
+                    else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
+                response_code = random.choice(observables.error_code) if observables and observables.error_code \
+                    else random.choice(ERROR_CODE)
+                response_size = faker.random_int(min=100, max=10000)
+                rule_id = random.choice(observables.event_id) if observables and observables.event_id \
+                    else faker.random_int(min=1, max=200)
+                action = random.choice(observables.action) if observables and observables.action \
+                    else random.choice(ACTIONS)
+                attack_type = random.choice(observables.technique).get('technique') if observables and \
+                    observables.technique else random.choice(TECHNIQUES).get('technique')
+                cookie_name = faker.word()
+                cookie_value = faker.uuid4()
+                cookies = f"{cookie_name}={cookie_value}"
+                leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|"
+                leef_log += f"src_ip={src_ip} src_port={src_port} request_url={url} method={method} referer={referer} "
+                leef_log += f"protocol={protocol} status={str(response_code)} action={action} attack_type={attack_type}"
+                leef_log += f" response_size={response_size} rule_id={rule_id} user_agent={user_agent} "
+                leef_log += f"severity={severity} cookie={cookies}"
+                leef_messages.append(leef_log)
+        else:
+            for i in range(count):
+                timestamp += timedelta(seconds=1)
+                severity = random.choice(observables.severity) if observables and observables.severity \
+                    else faker.random_int(min=1, max=5)
+                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
+                    else faker.ipv4()
+                src_port = faker.random_int(min=1024, max=65535)
+                host = random.choice(observables.src_host) if observables and observables.src_host \
+                    else faker.hostname()
+                url = random.choice(observables.technique).get('indicator') if observables and observables.technique \
+                    else random.choice(TECHNIQUES).get('indicator')
+                protocol = random.choice(observables.protocol) if observables and observables.protocol \
+                    else random.choice(PROTOCOLS)
+                response_code = random.choice(observables.error_code) if observables and observables.error_code \
+                    else random.choice(ERROR_CODE)
+                action = random.choice(observables.action) if observables and observables.action \
+                    else random.choice(ACTIONS)
+                leef_log = f"LEEF:1.0|{vendor}|{product}|{version}|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|"
+                leef_log += f"src_ip={src_ip} src_port={src_port} request_url={url} protocol={protocol} "
+                leef_log += f"status={str(response_code)} action={action} severity={severity}"
+                if observables:
+                    for observable, observable_value in vars(observables).items():
+                        if observable_value:
+                            leef_log += f" {observable}={random.choice(observable_value)}"
+                leef_messages.append(leef_log)
         return leef_messages
 
     @classmethod
     def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
             List[str]:
         """
         Generates fake Windows Event Log messages.
```

### Comparing `rosetta-ce-1.3.5/rosetta/rsender.py` & `rosetta-ce-1.3.6/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.6/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.5
+Version: 1.3.6
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.5/setup.py` & `rosetta-ce-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.5",
+    version="1.3.6",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.5/tests/test_rconverter.py` & `rosetta-ce-1.3.6/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/tests/test_rfaker.py` & `rosetta-ce-1.3.6/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.5/tests/test_rsender.py` & `rosetta-ce-1.3.6/tests/test_rsender.py`

 * *Files identical despite different names*

