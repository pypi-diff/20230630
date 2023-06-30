# Comparing `tmp/rosetta-ce-1.3.3.tar.gz` & `tmp/rosetta-ce-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.3.tar", last modified: Fri Jun 30 06:23:38 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.4.tar", last modified: Fri Jun 30 09:03:52 2023, max compression
```

## Comparing `rosetta-ce-1.3.3.tar` & `rosetta-ce-1.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 06:23:38.212078 rosetta-ce-1.3.3/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.3/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 06:23:38.211759 rosetta-ce-1.3.3/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.3/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 06:23:38.205527 rosetta-ce-1.3.3/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.3/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 06:23:38.207718 rosetta-ce-1.3.3/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.3/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.3/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.3/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.3/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.3/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    37216 2023-06-30 06:22:26.000000 rosetta-ce-1.3.3/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.3/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 06:23:38.209854 rosetta-ce-1.3.3/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 06:23:38.000000 rosetta-ce-1.3.3/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 06:23:38.000000 rosetta-ce-1.3.3/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 06:23:38.000000 rosetta-ce-1.3.3/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 06:23:38.000000 rosetta-ce-1.3.3/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 06:23:38.000000 rosetta-ce-1.3.3/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 06:23:38.212118 rosetta-ce-1.3.3/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 06:23:06.000000 rosetta-ce-1.3.3/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 06:23:38.211247 rosetta-ce-1.3.3/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.3/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.3/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.3/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.272039 rosetta-ce-1.3.4/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.4/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:03:52.271760 rosetta-ce-1.3.4/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.4/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.264836 rosetta-ce-1.3.4/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.4/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.266949 rosetta-ce-1.3.4/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.4/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.4/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.4/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    39105 2023-06-30 09:03:21.000000 rosetta-ce-1.3.4/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.4/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.269365 rosetta-ce-1.3.4/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-30 09:03:52.000000 rosetta-ce-1.3.4/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-30 09:03:52.272080 rosetta-ce-1.3.4/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-30 09:03:32.000000 rosetta-ce-1.3.4/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-30 09:03:52.271228 rosetta-ce-1.3.4/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.4/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.4/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.4/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.3/LICENSE` & `rosetta-ce-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/PKG-INFO` & `rosetta-ce-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.3
+Version: 1.3.4
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.3/README.md` & `rosetta-ce-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta/constants/sensors.py` & `rosetta-ce-1.3.4/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta/constants/sources.py` & `rosetta-ce-1.3.4/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta/constants/systems.py` & `rosetta-ce-1.3.4/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta/rconverter.py` & `rosetta-ce-1.3.4/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta/rfaker.py` & `rosetta-ce-1.3.4/rosetta/rfaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,14 @@
 
 
 class ObservableKnown(Enum):
     BAD = 'bad'
     GOOD = 'good'
 
 
-class CEFDevices(Enum):
-    Firewall = "Firewall"
-    EmailGW = "EmailGW"
-
-
 class Observables:
     def __init__(self, src_ip: list = None, dst_ip: Optional[list] = None, src_host: Optional[list] = None,
                  dst_host: Optional[list] = None, src_domain: Optional[list] = None, dst_domain: Optional[list] = None,
                  sender_email: Optional[list] = None, recipient_email: Optional[list] = None,
                  email_subject: Optional[list] = None, email_body: Optional[list] = None,
                  url: Optional[list] = None, port: Optional[list] = None, protocol: Optional[list] = None,
                  inbound_bytes: Optional[list] = None, outbound_bytes: Optional[list] = None,
@@ -144,15 +139,15 @@
         - observable_type: The type of observable to generate (e.g., IP, URL, SHA256, CVE, Terms).
         - known: The known status of the observable (e.g., BAD, GOOD).
 
         Returns:
         - A list of generated observables.
 
         Raises:
-        - Exception: If the function fails to retrieve data from any configured source with a HTTP status code other
+        - Exception: If the function fails to retrieve data from any configured source with an HTTP status code other
             than 200.
         """
         faker = cls._create_faker()
         gen_observables = []
         if observable_type == ObservableType.IP and known == ObservableKnown.BAD:
             for source in BAD_IP_SOURCES:
                 try:
@@ -270,23 +265,25 @@
         """
         Returns:
             Faker instance.
         """
         return Observables()
 
     @classmethod
-    def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
+    def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
+            List[str]:
         """
         Generate fake syslog messages.
 
         Args:
             count: The number of syslog messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             the past hour from now will be used.
-            observables: Optional. An observables object. If not provided, random objservable will be generated and used.
+            observables: Optional. An observables object. If not provided, random objservable will be generated
+            and used.
         Returns:
             A list of syslog messages.
 
         Examples:
             >>> Events.syslog(5)
             ['Jan 01 05:32:48 myhostname sudo[1023]: username : COMMAND ; cat /etc/shadow',
              'Jan 01 05:17:59 myhostname sudo[2019]: username : COMMAND ; find / -name \'*.log\' -exec rm -f {} \\;',
@@ -313,29 +310,30 @@
             command = random.choice(observables.cmd) if observables and observables.cmd \
                 else random.choice(UNIX_CMD)
             syslog_messages.append(f"{timestamp.strftime('%Y-%m-%d %H:%M:%S')} {host} {process}[{pid}]: {user}"
                                    f" : {action} ; {command}")
         return syslog_messages
 
     @classmethod
-    def cef(cls, count: int, vendor: Optional[str] = None, product: Optional[CEFDevices] = CEFDevices.Firewall,
+    def cef(cls, count: int, vendor: Optional[str] = None, product: Optional[str] = None,
             version: Optional[str] = None, timestamp: Optional[datetime] = None,
             observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake CEF (Common Event Format) messages.
 
         Args:
             count: The number of CEF messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during.
             vendor: Optional. The vendor.
             product: Optional. The product value options include:
             - Firewall
             - EmailGW
             version: Optional. The version.
-            observables: Optional. An observables object. If not provided, random objservable will be generated and used.
+            observables: Optional. An observables object. If not provided, random objservable will be generated
+            and used.
         Returns:
             A list of fake CEF messages in string format.
 
         Raises:
             None.
 
         Example Usage:
@@ -353,15 +351,15 @@
         cef_messages = []
         faker = cls._create_faker()
         vendor = vendor or faker.company()
         version = version or faker.numerify("1.0.#")
         if timestamp is None:
             timestamp = datetime.now() - timedelta(hours=1)
             timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
-        if product.name == "Firewall":
+        if product == "Firewall":
             for i in range(count):
                 log_id = faker.uuid4()
                 timestamp += timedelta(seconds=1)
                 severity = random.choice(observables.severity) if observables and observables.severity \
                     else faker.random_int(min=1, max=5)
                 src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
                     else faker.ipv4()
@@ -370,54 +368,82 @@
                     else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
                 dst_port = random.choice(observables.port) if observables and observables.port \
                     else faker.random_int(min=1024, max=65535)
                 dst_url = random.choice(observables.url) if observables and observables.url \
                     else Observables.generator(observable_type=ObservableType.URL, known=ObservableKnown.BAD, count=1)
                 inbound_bytes = random.choice(observables.inbound_bytes) if observables and observables.inbound_bytes \
                     else faker.random_int(min=10, max=1073741824)
-                outbound_bytes = random.choice(observables.outbound_bytes) if observables and observables.outbound_bytes \
+                outbound_bytes = random.choice(observables.outbound_bytes) if observables and \
+                    observables.outbound_bytes \
                     else faker.random_int(min=10, max=1073741824)
                 protocol = random.choice(observables.protocol) if observables and observables.protocol \
                     else random.choice(PROTOCOLS)
                 rule_id = random.choice(observables.event_id) if observables and observables.event_id \
                     else faker.random_int(min=1, max=200)
                 action = random.choice(observables.action) if observables and observables.action \
                     else random.choice(ACTIONS)
-                event_description = f"Firewall {action} {protocol} traffic from {src_ip}:{src_port} to {dst_ip}:{dst_port}"
-                cef_messages.append(f"CEF:0|{vendor}|{product.name}|{version}|{log_id}|{timestamp}|{severity}|"
-                                    f"{event_description}|src={src_ip} spt={src_port} dst={dst_ip} url={dst_url}"
-                                    f"dpt={dst_port} in_bytes={inbound_bytes} out_bytes={outbound_bytes} proto={protocol}"
-                                    f" rule={rule_id} act={action}")
-        elif product.name == "EmailGW":
+                event_description = f"Firewall {action} {protocol} traffic from {src_ip}:{src_port} to " \
+                                    f"{dst_ip}:{dst_port}"
+                cef_messages.append(f"CEF:0|{vendor}|{product}|{version}|{log_id}|{timestamp}|{severity}|"
+                                    f"{event_description}|src_ip={src_ip} src_port={src_port} dst_ip={dst_ip} "
+                                    f"url={dst_url} dst_port={dst_port} in_bytes={inbound_bytes} "
+                                    f"out_bytes={outbound_bytes} proto={protocol} rule={rule_id} act={action}")
+        elif product == "EmailGW":
             for i in range(count):
                 mail_id = faker.uuid4()
                 timestamp += timedelta(seconds=1)
                 src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
                     else faker.ipv4()
                 src_domain = random.choice(observables.src_domain) if observables and observables.src_domain \
                     else faker.domain_name()
                 sender_email = random.choice(observables.sender_email) if observables and observables.sender_email \
                     else faker.email()
                 recipient_email = random.choice(observables.recipient_email) if observables and \
                     observables.recipient_email else faker.email()
-                email_subject = random.choice(observables.email_subject) if observables and observables.email_subject else \
-                    faker.sentence(nb_words=6)
+                email_subject = random.choice(observables.email_subject) if observables and observables.email_subject \
+                    else faker.sentence(nb_words=6)
                 email_body = random.choice(observables.email_body) if observables and observables.email_body else \
                     faker.sentence(nb_words=50)
                 attachment_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
                     else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD,
                                                count=1)
                 spam_score = faker.random_int(min=1, max=5)
                 action = random.choice(observables.action) if observables and observables.action \
                     else random.choice(ACTIONS)
-                cef_messages.append(f"CEF:0|{vendor}|{product.name}|{version}|{mail_id}|{timestamp}|"
-                                    f"src={src_ip} src_domain={src_domain} sender_email={sender_email} "
+                cef_messages.append(f"CEF:0|{vendor}|{product}|{version}|{mail_id}|{timestamp}|"
+                                    f"src_ip={src_ip} src_domain={src_domain} sender_email={sender_email} "
                                     f"recipient_email={recipient_email} email_subject={email_subject} "
                                     f"email_body={email_body} attachment_hash={attachment_hash} spam_score={spam_score}"
                                     f" action={action}")
+        else:
+            for i in range(count):
+                log_id = faker.uuid4()
+                timestamp += timedelta(seconds=1)
+                severity = random.choice(observables.severity) if observables and observables.severity \
+                    else faker.random_int(min=1, max=5)
+                src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
+                    else faker.ipv4()
+                src_port = faker.random_int(min=1024, max=65535)
+                dst_ip = random.choice(observables.dst_ip) if observables and observables.dst_ip \
+                    else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
+                dst_port = random.choice(observables.port) if observables and observables.port \
+                    else faker.random_int(min=1024, max=65535)
+                protocol = random.choice(observables.protocol) if observables and observables.protocol \
+                    else random.choice(PROTOCOLS)
+                rule_id = random.choice(observables.event_id) if observables and observables.event_id \
+                    else faker.random_int(min=1, max=200)
+                action = random.choice(observables.action) if observables and observables.action \
+                    else random.choice(ACTIONS)
+                generic_cef = f"CEF:0|{vendor}|{product}|{version}|{log_id}|{timestamp}|{severity}|src_ip={src_ip} " \
+                              f"src_port={src_port} dst_ip={dst_ip} dst_port={dst_port} proto={protocol} " \
+                              f"rule={rule_id} act={action}"
+                if observables:
+                    for observable, observable_value in vars(observables).items():
+                        generic_cef += f" {observable}={observable_value}"
+                cef_messages.append(generic_cef)
         return cef_messages
 
     @classmethod
     def leef(cls, count, timestamp: Optional[datetime] = None, vendor: Optional[str] = None,
              product: Optional[str] = None, version: Optional[str] = None,
              observables: Optional[Observables] = None) -> List[str]:
         """
@@ -483,15 +509,16 @@
             leef_log += f"request_size={request_size} " \
                         f"response_size={response_size} "
             leef_log += f"user_agent={user_agent}"
             leef_messages.append(leef_log)
         return leef_messages
 
     @classmethod
-    def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
+    def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> \
+            List[str]:
         """
         Generates fake Windows Event Log messages.
 
         Args:
             count (int): The number of fake messages to generate.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
```

### Comparing `rosetta-ce-1.3.3/rosetta/rsender.py` & `rosetta-ce-1.3.4/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.4/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.3
+Version: 1.3.4
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.3/setup.py` & `rosetta-ce-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.3",
+    version="1.3.4",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.3/tests/test_rconverter.py` & `rosetta-ce-1.3.4/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/tests/test_rfaker.py` & `rosetta-ce-1.3.4/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.3/tests/test_rsender.py` & `rosetta-ce-1.3.4/tests/test_rsender.py`

 * *Files identical despite different names*

