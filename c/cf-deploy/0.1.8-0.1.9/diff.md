# Comparing `tmp/cf_deploy-0.1.8.tar.gz` & `tmp/cf_deploy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_deploy-0.1.8.tar", max compression
+gzip compressed data, was "cf_deploy-0.1.9.tar", max compression
```

## Comparing `cf_deploy-0.1.8.tar` & `cf_deploy-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1293 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/cf_deploy/__init__.py
--rw-r--r--   0        0        0    12259 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/cf_deploy/main.py
--rw-r--r--   0        0        0     1671 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/cf_deploy/models.py
--rw-r--r--   0        0        0        0 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/cf_deploy/utils/__init__.py
--rw-r--r--   0        0        0      925 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/cf_deploy/utils/logging.py
--rw-r--r--   0        0        0      539 2023-03-20 13:36:14.878237 cf_deploy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 cf_deploy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1293 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/cf_deploy/__init__.py
+-rw-r--r--   0        0        0    12436 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/cf_deploy/main.py
+-rw-r--r--   0        0        0     1671 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/cf_deploy/models.py
+-rw-r--r--   0        0        0        0 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/cf_deploy/utils/__init__.py
+-rw-r--r--   0        0        0      925 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/cf_deploy/utils/logging.py
+-rw-r--r--   0        0        0      539 2023-03-20 13:54:01.839103 cf_deploy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 cf_deploy-0.1.9/PKG-INFO
```

### Comparing `cf_deploy-0.1.8/README.md` & `cf_deploy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cf_deploy-0.1.8/cf_deploy/main.py` & `cf_deploy-0.1.9/cf_deploy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
         StackName=stack_name,
         ChangeSetName=change_set_id,
     )
 
     if not arguments.skip_wait:
         track_stack_events(stack_name, config.region, verbose=not progress_bar)
 
+    log.info("Finished Deployment", name=stack_name)
     if progress_bar:
         progress_bar.update(1)
 
 
 def loading_config(path: Path, base_config: BaseConfig, arguments) -> Iterable[Config]:
     for p in (path if isinstance(path, list) else [path]):
         for file_location in glob.glob(p):
@@ -260,14 +261,15 @@
     parser.add_argument("--confirmation-required", help="Ask for confirmation before deploying", action="store_true")
     parser.add_argument("--debug", help="Enable debug logging", action="store_true")
     parser.add_argument("--dry-run", help="Only print changes", action="store_true")
     parser.add_argument("--region", help="AWS region to use", default=os.environ.get("AWS_DEFAULT_REGION", "eu-west-1"))
     parser.add_argument("--skip-wait", help="Disable waiting for stack to be deployed", action="store_true")
     parser.add_argument("--parallel", help="Deploy stacks in parallel", action="store_true")
     parser.add_argument("--delete-deprecated", help="Delete stacks that are not in the config", action="store_true")
+    parser.add_argument("--concurrency", help="Number of stacks to deploy in parallel", default=16, type=int)
 
     args = parser.parse_args()
 
     if args.debug:
         logging.getLogger().setLevel(logging.DEBUG)
 
     # Parse base configs if given
@@ -278,15 +280,15 @@
             base_config = BaseConfig(**always_merger.merge(base_config, yaml.load(base_config_file, Loader=Loader)))
 
     configs: List[Config] = list(loading_config(args.config, base_config, args))
 
     # Load configs
     if args.parallel:
         log.info("Deploying stacks in parallel")
-        with ThreadPoolExecutor(max_workers=10) as executor, tqdm(total=len(configs), desc="Stacks", unit="stack") as progress_bar:
+        with ThreadPoolExecutor(max_workers=args.concurrency) as executor, tqdm(total=len(configs), desc="Stacks", unit="stack") as progress_bar:
             deploy_stack_with_progress = partial(deploy_stack, progress_bar=progress_bar)
 
             for config in configs:
                 stack_name = f"{base_config.prefix or ''}{config.name}"
                 executor.submit(deploy_stack_with_progress, stack_name, config, base_config, args)
     else:
         for config in configs:
```

### Comparing `cf_deploy-0.1.8/cf_deploy/models.py` & `cf_deploy-0.1.9/cf_deploy/models.py`

 * *Files identical despite different names*

### Comparing `cf_deploy-0.1.8/cf_deploy/utils/logging.py` & `cf_deploy-0.1.9/cf_deploy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cf_deploy-0.1.8/pyproject.toml` & `cf_deploy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf-deploy"
-version = "0.1.8"
+version = "0.1.9"
 description = "A package to automate CloudFormation deployments"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `cf_deploy-0.1.8/PKG-INFO` & `cf_deploy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-deploy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to automate CloudFormation deployments
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

