# Comparing `tmp/blacksmith_ai-0.2.0.tar.gz` & `tmp/blacksmith_ai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksmith_ai-0.2.0.tar", max compression
+gzip compressed data, was "blacksmith_ai-0.2.1.tar", max compression
```

## Comparing `blacksmith_ai-0.2.0.tar` & `blacksmith_ai-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 blacksmith_ai-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 blacksmith_ai-0.2.0/blacksmith/__init__.py
--rw-r--r--   0        0        0     2452 2023-06-29 21:50:17.114047 blacksmith_ai-0.2.0/blacksmith/agents.py
--rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 blacksmith_ai-0.2.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
--rw-r--r--   0        0        0      718 2023-06-29 10:04:18.913031 blacksmith_ai-0.2.0/blacksmith/defaults/prompts.py
--rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 blacksmith_ai-0.2.0/blacksmith/llm.py
--rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 blacksmith_ai-0.2.0/blacksmith/scripts/__init__.py
--rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4117 2023-06-30 08:23:28.853542 blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     4352 2023-06-30 08:21:48.445763 blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc
--rw-r--r--   0        0        0     5865 2023-06-29 21:11:14.960357 blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
--rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc
--rw-r--r--   0        0        0     2182 2023-06-30 08:23:13.650148 blacksmith_ai-0.2.0/blacksmith/scripts/cli.py
--rw-r--r--   0        0        0     3784 2023-06-30 08:21:39.811441 blacksmith_ai-0.2.0/blacksmith/scripts/images.py
--rw-r--r--   0        0        0     5297 2023-06-29 21:11:12.102979 blacksmith_ai-0.2.0/blacksmith/scripts/k8s.py
--rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 blacksmith_ai-0.2.0/blacksmith/tools.py
--rw-r--r--   0        0        0      517 2023-06-30 20:38:36.177443 blacksmith_ai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 blacksmith_ai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-06-26 21:55:07.746361 blacksmith_ai-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 22:46:21.760508 blacksmith_ai-0.2.1/blacksmith/__init__.py
+-rw-r--r--   0        0        0     2452 2023-06-29 21:50:17.114047 blacksmith_ai-0.2.1/blacksmith/agents.py
+-rw-r--r--   0        0        0      553 2023-06-28 03:04:51.693365 blacksmith_ai-0.2.1/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc
+-rw-r--r--   0        0        0      718 2023-06-29 10:04:18.913031 blacksmith_ai-0.2.1/blacksmith/defaults/prompts.py
+-rw-r--r--   0        0        0      368 2023-06-29 10:21:48.331464 blacksmith_ai-0.2.1/blacksmith/llm.py
+-rw-r--r--   0        0        0        0 2023-06-26 22:06:00.728175 blacksmith_ai-0.2.1/blacksmith/scripts/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-26 22:06:03.377477 blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4117 2023-06-30 08:23:28.853542 blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4352 2023-06-30 08:21:48.445763 blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/images.cpython-311.pyc
+-rw-r--r--   0        0        0     5865 2023-06-29 21:11:14.960357 blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc
+-rw-r--r--   0        0        0     2976 2023-06-26 22:05:41.831425 blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0        0        0     2235 2023-06-30 20:48:27.127415 blacksmith_ai-0.2.1/blacksmith/scripts/cli.py
+-rw-r--r--   0        0        0     3784 2023-06-30 08:21:39.811441 blacksmith_ai-0.2.1/blacksmith/scripts/images.py
+-rw-r--r--   0        0        0     5345 2023-06-30 20:49:29.575298 blacksmith_ai-0.2.1/blacksmith/scripts/k8s.py
+-rw-r--r--   0        0        0     2406 2023-06-28 23:45:12.797321 blacksmith_ai-0.2.1/blacksmith/tools.py
+-rw-r--r--   0        0        0      517 2023-06-30 20:50:46.027831 blacksmith_ai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 blacksmith_ai-0.2.1/PKG-INFO
```

### Comparing `blacksmith_ai-0.2.0/blacksmith/agents.py` & `blacksmith_ai-0.2.1/blacksmith/agents.py`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc` & `blacksmith_ai-0.2.1/blacksmith/defaults/__pycache__/prompts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/defaults/prompts.py` & `blacksmith_ai-0.2.1/blacksmith/defaults/prompts.py`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/cli.cpython-311.pyc` & `blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/images.cpython-311.pyc` & `blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/images.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc` & `blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/k8s.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/__pycache__/main.cpython-311.pyc` & `blacksmith_ai-0.2.1/blacksmith/scripts/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/cli.py` & `blacksmith_ai-0.2.1/blacksmith/scripts/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     print("🛠️  Building tool images...")
     tool_specs = build_tool_images()
     print("✨ Completed!")
 
     # Remove intermediate build files
     shutil.rmtree("./tmp")
 
+    # Create k8s manifests
+    os.makedirs("./k8s")
+
     print("📦  Creating manifest...")
     create_k8s_manifest(agent_specs, tool_specs)
     print("✨ Completed!")
     print("⚙️  Building Redis tool registry...")
     create_redis()
     print("✨ Completed!")
```

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/images.py` & `blacksmith_ai-0.2.1/blacksmith/scripts/images.py`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/blacksmith/scripts/k8s.py` & `blacksmith_ai-0.2.1/blacksmith/scripts/k8s.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                                 "port": 80,
                                 "targetPort": spec["ports"],
                                 "nodePort": 30000,
                             }
                         ],
                     },
                 }
-                with open(f"manifest.yaml", "a") as file:
+                with open(f"./k8s/manifest.yaml", "a") as file:
                     file.write(yaml.dump(node_port))
                     file.write("---\n")
 
             if spec["type"] == "TOOL":
                 # Generate a service for the deployment
                 service = {
                     "apiVersion": "v1",
@@ -78,15 +78,15 @@
                                 "protocol": "TCP",
                                 "port": 80,
                                 "targetPort": spec["ports"],
                             }
                         ],
                     },
                 }
-                with open(f"manifest.yaml", "a") as file:
+                with open(f"./k8s/manifest.yaml", "a") as file:
                     file.write(yaml.dump(service))
                     file.write("---\n")
         except Exception as e:
             print(f"Error: could not build {spec}: {e}")
 
 
 def create_redis():
@@ -108,37 +108,37 @@
                             "ports": [{"containerPort": 6379}],
                         }
                     ]
                 },
             },
         },
     }
-    with open(f"redis.yaml", "w") as file:
+    with open(f"./k8s/redis.yaml", "w") as file:
         file.write("# REDIS DEPLOYMENT # \n")
         file.write(yaml.dump(redis_deployment))
 
     # Add the service to the manifest
     redis_service = {
         "apiVersion": "v1",
         "kind": "Service",
         "metadata": {"name": "redis-service"},
         "spec": {
             "selector": {"app": "redis"},
             "ports": [{"name": "redis", "port": 6379}],
         },
     }
-    with open(f"redis.yaml", "a") as file:
+    with open(f"./k8s/redis.yaml", "a") as file:
         file.write("---\n")
         file.write(yaml.dump(redis_service))
 
 
 def apply_redis():
-    subprocess.run(["kubectl", "apply", "-f", "redis.yaml"], check=True)
+    subprocess.run(["kubectl", "apply", "-f", "./k8s/redis.yaml"], check=True)
 
 
 def apply_k8s_manifest():
-    subprocess.run(["kubectl", "apply", "-f", "manifest.yaml"], check=True)
+    subprocess.run(["kubectl", "apply", "-f", "./k8s/manifest.yaml"], check=True)
 
 
 def remove():
-    subprocess.run(["kubectl", "delete", "-f", "redis.yaml"], check=True)
-    subprocess.run(["kubectl", "delete", "-f", "manifest.yaml"], check=True)
+    subprocess.run(["kubectl", "delete", "-f", "./k8s/redis.yaml"], check=True)
+    subprocess.run(["kubectl", "delete", "-f", "./k8s/manifest.yaml"], check=True)
```

### Comparing `blacksmith_ai-0.2.0/blacksmith/tools.py` & `blacksmith_ai-0.2.1/blacksmith/tools.py`

 * *Files identical despite different names*

### Comparing `blacksmith_ai-0.2.0/pyproject.toml` & `blacksmith_ai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blacksmith-ai"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["alec <fkalec@gmail.com>"]
 readme = "README.md"
 packages = [{include = "blacksmith"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `blacksmith_ai-0.2.0/PKG-INFO` & `blacksmith_ai-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksmith-ai
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: alec
 Author-email: fkalec@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.1.3,<7.0.0)
```

