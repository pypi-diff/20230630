# Comparing `tmp/refyre-0.0.1.5.tar.gz` & `tmp/refyre-0.0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refyre-0.0.1.5.tar", max compression
+gzip compressed data, was "refyre-0.0.1.5.1.tar", max compression
```

## Comparing `refyre-0.0.1.5.tar` & `refyre-0.0.1.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    10130 2023-06-27 17:47:06.677770 refyre-0.0.1.5/README.md
--rw-r--r--   0        0        0      922 2023-06-27 17:47:06.677770 refyre-0.0.1.5/pyproject.toml
--rw-r--r--   0        0        0    23589 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/Refyre.py
--rw-r--r--   0        0        0      135 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cli.py
--rw-r--r--   0        0        0     3731 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Association.py
--rw-r--r--   0        0        0     3825 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Broadcast.py
--rw-r--r--   0        0        0     2281 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Cache.py
--rw-r--r--   0        0        0    20495 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/Cluster.py
--rw-r--r--   0        0        0      718 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/ClusterIterator.py
--rw-r--r--   0        0        0      237 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/cogs/VariableAction.py
--rw-r--r--   0        0        0     2767 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/cluster/cogs/VariableParser.py
--rw-r--r--   0        0        0       23 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/config/__init__.py
--rw-r--r--   0        0        0      355 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/config/log.py
--rw-r--r--   0        0        0      499 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/AliasManager.py
--rw-r--r--   0        0        0      375 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/CodeManager.py
--rw-r--r--   0        0        0     3882 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/RecipePreprocessor.py
--rw-r--r--   0        0        0      126 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/core/__init__.py
--rw-r--r--   0        0        0     1597 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/DataStack.py
--rw-r--r--   0        0        0      347 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/TorchStack.py
--rw-r--r--   0        0        0       34 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/datastack/__init__.py
--rw-r--r--   0        0        0      802 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/FileGraph.py
--rw-r--r--   0        0        0     2051 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/FileGraphNode.py
--rw-r--r--   0        0        0       73 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/graph/__init__.py
--rw-r--r--   0        0        0     2375 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/ExpressionGenerator.py
--rw-r--r--   0        0        0     6066 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/Lexer.py
--rw-r--r--   0        0        0     3287 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/Parser.py
--rw-r--r--   0        0        0     3492 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/PatternGenerator.py
--rw-r--r--   0        0        0      221 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/__init__.py
--rw-r--r--   0        0        0      799 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/cogs/LexerToken.py
--rw-r--r--   0        0        0      618 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/reader/cogs/lexer_utils.py
--rw-r--r--   0        0        0      153 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/__init__.py
--rw-r--r--   0        0        0      667 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/clone.py
--rw-r--r--   0        0        0      453 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/optional_imports.py
--rw-r--r--   0        0        0      903 2023-06-27 17:47:06.681770 refyre-0.0.1.5/refyre/utils/regex.py
--rw-r--r--   0        0        0    10989 1970-01-01 00:00:00.000000 refyre-0.0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10130 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/README.md
+-rw-r--r--   0        0        0      924 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    23582 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/Refyre.py
+-rw-r--r--   0        0        0      135 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cli.py
+-rw-r--r--   0        0        0     3731 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Association.py
+-rw-r--r--   0        0        0     3813 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Broadcast.py
+-rw-r--r--   0        0        0     2281 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Cache.py
+-rw-r--r--   0        0        0    20658 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/Cluster.py
+-rw-r--r--   0        0        0      718 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/ClusterIterator.py
+-rw-r--r--   0        0        0      237 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/cogs/VariableAction.py
+-rw-r--r--   0        0        0     2767 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/cluster/cogs/VariableParser.py
+-rw-r--r--   0        0        0       23 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/config/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/config/log.py
+-rw-r--r--   0        0        0      499 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/AliasManager.py
+-rw-r--r--   0        0        0      363 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/CodeManager.py
+-rw-r--r--   0        0        0     3543 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/RecipePreprocessor.py
+-rw-r--r--   0        0        0      126 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/core/__init__.py
+-rw-r--r--   0        0        0     1597 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/DataStack.py
+-rw-r--r--   0        0        0      347 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/TorchStack.py
+-rw-r--r--   0        0        0       34 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/datastack/__init__.py
+-rw-r--r--   0        0        0      802 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/FileGraph.py
+-rw-r--r--   0        0        0     2051 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/FileGraphNode.py
+-rw-r--r--   0        0        0       73 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/graph/__init__.py
+-rw-r--r--   0        0        0     2375 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/reader/ExpressionGenerator.py
+-rw-r--r--   0        0        0     6066 2023-06-30 01:37:12.644978 refyre-0.0.1.5.1/refyre/reader/Lexer.py
+-rw-r--r--   0        0        0     3287 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/Parser.py
+-rw-r--r--   0        0        0     3492 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/PatternGenerator.py
+-rw-r--r--   0        0        0      221 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/cogs/LexerToken.py
+-rw-r--r--   0        0        0      618 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/reader/cogs/lexer_utils.py
+-rw-r--r--   0        0        0      153 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/clone.py
+-rw-r--r--   0        0        0      453 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/optional_imports.py
+-rw-r--r--   0        0        0      903 2023-06-30 01:37:12.648978 refyre-0.0.1.5.1/refyre/utils/regex.py
+-rw-r--r--   0        0        0    10991 1970-01-01 00:00:00.000000 refyre-0.0.1.5.1/PKG-INFO
```

### Comparing `refyre-0.0.1.5/README.md` & `refyre-0.0.1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 These are all the basic quantifiers you can use, they cover ~80% of refyre's inner power. The other 20% are pretty obscure and aren't that useful normally.
 
 ### FileClusters (Variables)
 
 Variables are the backbone of refyre. The clusters provide an *avenue* for the variables to easily target the data without worrying about writing any code. However, they aren't the only way to access variable's powers. The docs below, again, specify the most useful abilities for these variables.
 
 `FileCluster(values = [], dirs = [], patterns = [], as_pathlib = False,)`
-    - `values`: string filepaths, or `Path` objects depending on wheterh `as_pathlib` is true or false.
+    - `values`: string filepaths, or `Path` objects depending on whether `as_pathlib` is true or false.
     - `patterns`: corresponds to the dirs, lists what patterns you want to target
 
 FileClusters are strongly rooted in *object oriented operations*, meaning each operation returns another FileCluster, so you can continue channeling FileCluster capabilities. To get out of FileClusters, you can use the following options:
     - `.vals()`: Returns a list of Path objects
     - `.item()`: Returns the first Path object
 
 Using this basic constructor, you can make some easy operations:
```

### Comparing `refyre-0.0.1.5/pyproject.toml` & `refyre-0.0.1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "refyre"
-version = "0.0.1.5"
+version = "0.0.1.5.1"
 description = "Filesystem dominance is all you need."
 authors = ["Ansh <teamnebulaco@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/flockfysh/refyre"
 license = "MIT"
 keywords = ["files", "manipulation", "data science", ]
 packages = [
```

### Comparing `refyre-0.0.1.5/refyre/Refyre.py` & `refyre-0.0.1.5.1/refyre/Refyre.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         '''
             Attaches an externally made variable to the refyre object
         '''
         assert type(key) == str, "Key should be a string referring to a variable name"
         assert type(value) == FileCluster, "Value should be a FileCluster variable"
         self.variables[key] = value
 
+    def __len__(self):
+        return len(self.variables)
+
     def __contains__(self, key):
         return key in self.variables
 
     #The Five Fundamental Operations of Refyre
     def __construct(self, input_path, is_output = False, expand_path = ""):
         '''
             Construct Operation:
@@ -136,15 +139,15 @@
                 logger.info('valid regex')
 
                 #Create nodes for each of the pattern matches
                 logger.info(f'{new_path}, {new_path.parent}')
                 for fl in new_path.parent.iterdir():
 
                     logger.info(f'file {fl}')
-                    if re.search(r'{}'.format(PatternGenerator(node.directory)), fl.as_posix()) and fl not in ret and fl.is_dir() and file_num >= lower and file_num <= upper: #No files will be allowed to be fclusters
+                    if re.search(r'{}'.format(PatternGenerator(node.directory)), str(fl)) and fl not in ret and fl.is_dir() and file_num >= lower and file_num <= upper: #No files will be allowed to be fclusters
 
                         pattern_matched_node = node.copy()
                         assert pattern_matched_node.pattern == node.pattern, f"Copy node has pattern {pattern_matched_node.pattern} while node has pattern {node.pattern}"
 
                         assert type(fl.name) == str
                         #Update the directory with the name 
                         pattern_matched_node.directory = fl.name 
@@ -233,17 +236,17 @@
                 if pattern_node.alias != '':
                     logger.debug(f'adding {pattern_node.alias}')
 
                     logger.debug(f'reversing {node.directory} {pattern_node.directory}')
                     n = ExpressionGenerator.reverse_generator_expression(node.directory, pattern_node.directory)
 
                     if ( ('*s' in node.flags or '*l' in node.flags) and n == mx_num + 1):
-                        self.alias_manager.add( ExpressionGenerator(pattern_node.alias)(1), Path(new_path.as_posix()), is_pathlib = True)
+                        self.alias_manager.add( ExpressionGenerator(pattern_node.alias)(1), Path(new_path), is_pathlib = True)
                     elif not ('*s' in node.flags or '*l' in node.flags):
-                        self.alias_manager.add( ExpressionGenerator(pattern_node.alias)(n), Path(new_path.as_posix()), is_pathlib = True)
+                        self.alias_manager.add( ExpressionGenerator(pattern_node.alias)(n), Path(new_path), is_pathlib = True)
                     
             
             return ret
 
         else:
             logger.debug('in else', )
             #Before we go to children, let's handle any imports we must
@@ -263,15 +266,15 @@
 
             if node.type == 'git' and node.link != '':
                 clone_node(node.link, new_path)
                 
             if node.alias != '':
                 logger.debug(f'adding {node.alias}')
                 logger.debug(ExpressionGenerator(node.alias)(1))
-                self.alias_manager.add(ExpressionGenerator(node.alias)(1), Path(new_path.as_posix()), is_pathlib = True)
+                self.alias_manager.add(ExpressionGenerator(node.alias)(1), Path(new_path), is_pathlib = True)
 
             nchild = []
             for child in node.children + [import_fgraph]:
                 nchild.extend(self.__expand(child, new_path, step = step))
             
             node.children = [c for c in nchild  if c is not None]
 
@@ -288,15 +291,15 @@
         '''
         new_path = Path(node.directory) if node.is_root_dir() else Path(path) / node.directory
 
         logger.debug(f'Testing to see if {new_path} exists')
         if not new_path.exists():
             return [False, None]
         
-        new_path = new_path.as_posix()
+        new_path = str(new_path)
 
         if not node.children:
             return [True, node]
 
         ret = []
         for child in node.children:
             ret.append(self.__verify(child, new_path))
@@ -323,15 +326,15 @@
 
         #Updating the path
         new_path = Path(node.directory) if node.is_root_dir() else Path(path) / node.directory
 
         if not new_path.exists():
             raise Exception(f"Weird issue caught during activation ... an invalid path appeared - {new_path}")
 
-        new_path = new_path.as_posix()
+        new_path = str(new_path)
 
         if node.name != "":
             logger.info(f'activating {new_path} {node.directory} {node.name}')
             self.__parse_var(node, new_path, mode)
 
         if node.flags != '':
             #Activate the code manager
@@ -355,15 +358,15 @@
         '''
         #Updating the path
         logger.debug(f'in output')
         new_path = Path(node.directory) if node.is_root_dir() else Path(path) / node.directory
 
         logger.debug(f'mode {node.mode}')
         self.__create_output(node, new_path, mode if node.mode == '' else node.mode)
-        new_path = new_path.as_posix()
+        new_path = str(new_path)
 
         for child in node.children:
             self.__output(child, new_path, "copy")
         
 
     def __clear(self, wipe_proto = True, wipe_vars = True):
         '''
@@ -476,28 +479,28 @@
                 
             logger.debug(f'Bad files: {bad_files}')
             
             #Snip ... snip ... *ouch* >_<
             for fl in bad_files:
                 logger.debug(f'Deleting {fl}')
                 if fl.is_dir():
-                    shutil.rmtree(fl.as_posix())
+                    shutil.rmtree(str(fl))
                 elif fl.is_file():
                     fl.unlink()
                 else:
                     logger.error('No clue how to handle this file', )
 
 
-        new_path = new_path.as_posix()
+        new_path = str(new_path)
 
         for child in node.children:
             self.__post_generate(child, new_path, mode, "*da" if node.flags == "*da" else flags)
         
 
-    def add_spec(self, spec_path):
+    def add_spec(self, spec_path, track = False):
         '''
         Adds a spec to parse
         '''
 
         #Construct an fgraph instance
         proto, graph_to_add = self.__construct(spec_path, is_output = False)
         logger.debug(graph_to_add, )
@@ -577,18 +580,18 @@
 
         pths = {}
 
         for var_name in self.variables:
             pths[var_name] = []
 
             for p in self.variables[var_name]:
-                pths[var_name].append(p.as_posix())
+                pths[var_name].append(str(p))
             
         save_pth = Path(save_dir) / "refyre_state.json"
-        with open(save_pth.as_posix(), 'w') as f:
+        with open(str(save_pth), 'w') as f:
             json.dump(pths, f, indent = 4)
      
     def load(load_filename):
 
         with open(load_filename, 'r') as f:
             pths = json.load(f)
```

### Comparing `refyre-0.0.1.5/refyre/cli.py` & `refyre-0.0.1.5.1/refyre/cli.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/cluster/Association.py` & `refyre-0.0.1.5.1/refyre/cluster/Association.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/cluster/Broadcast.py` & `refyre-0.0.1.5.1/refyre/cluster/Broadcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     @classmethod
     def clear(cls):
         cls.files_dict.clear()
 
     @classmethod
     def add(cls, id, cluster_vals):
         for v in cluster_vals:
-            insert(cls.files_dict, v.as_posix(), id) 
+            insert(cls.files_dict, str(v), id) 
 
         
     @classmethod
     def release(cls, cluster_id):
         logger.debug(f'released {cluster_id}')
         for k in cls.files_dict:
             logger.debug(f'{k}, {cluster_id}, {cls.files_dict[k]}')
@@ -93,15 +93,15 @@
                         if cluster_id != instance.id and Path(before) in cluster.values:
                             cluster.values[cluster.values.index(Path(before))] = Path(after)
                         
                 else:
                     for cluster_id in before_vals:
                         if cluster_id != instance.id:
                             cluster = clusters[cluster_id]()
-                            cluster.values = [v for v in cluster.values if v.as_posix() != before] 
+                            cluster.values = [v for v in cluster.values if str(v) != before] 
 
             self.files_dict = {k:self.files_dict[k] for k in self.files_dict if len(self.files_dict[k]) > 0 and Path(k).exists()}
             Broadcaster.files_dict = self.files_dict
 
             instance.values = [v for v in list(dict.fromkeys(instance.values)) if v.exists() ]
             logger.debug(f"RETURNED {instance.values} {self.files_dict} {Broadcaster.files_dict}")
```

### Comparing `refyre-0.0.1.5/refyre/cluster/Cache.py` & `refyre-0.0.1.5.1/refyre/cluster/Cache.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/cluster/Cluster.py` & `refyre-0.0.1.5.1/refyre/cluster/Cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,22 @@
             other - another FileCluster
 
             Returns the union between two FileClusters
         '''
 
         return FileCluster(input_paths = [], input_patterns = [], values = list(set(self.values).union(other.values)))
     
+    def __xor__(self, other):
+        '''
+            other - another FileCluster
+
+            Returns the exclusive or between the two FileClusters
+        '''
+        return FileCluster(input_paths = [], input_patterns = [], values = list(set(self.values) ^ set(other.values)))
+    
     def __sub__(self, other):
         '''
             other - another FileCluster
 
             Returns all the files that are exclusively in self
         '''
 
@@ -209,23 +217,22 @@
     def __iter__(self):
         return FileClusterIterator(self)
 
     def __copy__(self):
         return FileCluster(values = self.values, as_pathlib = True)
     
     def __deepcopy__(self):
-        return FileCluster(values = [Path(p.as_posix()) for p in self.values], as_pathlib = True)
+        return FileCluster(values = [Path(p) for p in self.values], as_pathlib = True)
 
     def __getitem__(self, key):
         if isinstance(key, slice):
             return FileCluster(input_patterns = [] , input_paths = [], values = self.values[key.start:key.stop:key.step], as_pathlib = True)
         elif isinstance(key, int):
             return FileCluster(input_patterns = [] , input_paths = [], values = [self.values[key]], as_pathlib = True)
 
-    
     @Broadcaster()
     def move(self, target_dir, conflict_function = handle_file_conflict):
         """
         The above code defines functions for moving, copying, and deleting files in a directory, with
         options for handling conflicts and broadcasting changes.
         
         :param target_dir: The directory to which files will be moved or copied
@@ -254,20 +261,20 @@
                 dest = conflict_function(p / v.name)
 
                 #if dest is None, we ignore it
                 if dest:
                     logger.debug(f'{str(v)}, {str(dest)}')
                     shutil.move(str(v), str(dest))
                     changes.append((str(v), str(dest)))
-                    nvals.append(Path(dest.as_posix()))
+                    nvals.append(Path(dest))
             else:
                 logger.debug('else')
                 logger.debug(str(v))
                 changes.append((str(v), str(v)))
-                nvals.append(Path(v.as_posix()))
+                nvals.append(Path(v))
             
         return changes, FileCluster(input_patterns = [], input_paths = [], values = nvals, as_pathlib = True)
     
     def copy(self, target_dir, conflict_function = handle_file_conflict):
         '''
         Input: 
             - target_dir: the directory to which all files will be sent.
@@ -284,34 +291,34 @@
         nvals = []
         for v in self.values:
             dest = conflict_function(p / v.name)
 
             #if dest is None, we ignore it
             if dest:
                 shutil.copy(str(v), str(dest))
-                nvals.append(Path(dest.as_posix()))
+                nvals.append(Path(dest))
             
         return FileCluster(input_patterns = [], input_paths = [], values = nvals, as_pathlib = True)
 
     @Broadcaster()
     def delete(self):
         """
         The function deletes all files in a FileCluster object and returns an empty object while keeping
         track of the changes made.
         :return: a tuple containing two elements: a list of changes made during the deletion process and
         an empty FileCluster object.
         """
         changes = []
         for fl in self.values:
             if fl.is_dir():
-                shutil.rmtree(fl.as_posix())
-                changes.append((fl.as_posix(), None))
+                shutil.rmtree(str(fl))
+                changes.append((str(fl), None))
             elif fl.is_file():
                 fl.unlink()
-                changes.append((fl.as_posix(), None))
+                changes.append((str(fl), None))
 
 
         return changes, FileCluster(input_patterns = [], input_paths = [], values = [])
 
     @Broadcaster()
     def rename(self, rename_function):
         """
@@ -327,16 +334,16 @@
         2. A new instance of the FileCluster class with the updated values after the renaming process.
         """
         
         nvals = []
         changes = []
         for i, v in enumerate(self.values):
             logger.debug(f'renaming, {v},{v.parent / rename_function(i)}')
-            nvals.append(Path(v.as_posix()).rename(v.parent / rename_function(i)))
-            changes.append((v.as_posix(), nvals[-1].as_posix()))
+            nvals.append(Path(v).rename(v.parent / rename_function(i)))
+            changes.append((str(v), str(nvals[-1])))
 
         return changes, FileCluster(input_patterns = [], input_paths = [], values = nvals, as_pathlib = True)
 
     def zip(self, save_dir = '.', save_name = "out.zip", conflict_function = handle_file_conflict):
         """
         This function zips all the files in a directory into a single zip file.
         
@@ -352,17 +359,17 @@
 
         save_p = Path(save_dir) / save_name
 
         copied = self.copy(save_dir)
 
 
         save_p = handle_file_conflict(save_p)
-        with zipfile.ZipFile(save_p.as_posix(), 'w') as zipMe:        
+        with zipfile.ZipFile(str(save_p), 'w') as zipMe:        
             for fl in copied.values:
-                zipMe.write(fl.as_posix(), compress_type=zipfile.ZIP_DEFLATED)
+                zipMe.write(str(fl), compress_type=zipfile.ZIP_DEFLATED)
         
         assert save_p.exists(), "For some reason, the newly created zip file does not exist"
 
         copied.delete()
 
         return FileCluster(input_patterns = [], input_paths = [], values = [save_p], as_pathlib = True)
 
@@ -394,15 +401,15 @@
 
 
             Return type: the Response object returned from the requests.get() call
             '''
 
             #Zip all the files up to send
             zipped = self.zip()
-            zipped_fp = zipped.vals()[0].as_posix()
+            zipped_fp = str(zipped.item())
 
             resp = None
             with open(zipped_fp, "rb") as f:
                 resp = requests.post(url = url, params = additional_data, files = { payload_name : f })
 
             #Delete the intermediate zip we constructed
             zipped.delete()
@@ -462,15 +469,15 @@
         If it
         :return: A FileCluster object with the filtered values.
         """
 
         nvals = []
         for v in self.values:
             if filter_func(v):
-                nvals.append(Path(v.as_posix())) #Append a copy of the object to prevent object ref shenanigans
+                nvals.append(Path(v)) #Append a copy of the object to prevent object ref shenanigans
         
         return FileCluster(input_patterns = [], input_paths = [], values = nvals, as_pathlib = True)
 
     def clone(self):
         """
         The function returns a deep clone of the current object.
         :return: A deep clone of the current object is being returned.
```

### Comparing `refyre-0.0.1.5/refyre/cluster/ClusterIterator.py` & `refyre-0.0.1.5.1/refyre/cluster/ClusterIterator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/cluster/cogs/VariableAction.py` & `refyre-0.0.1.5.1/refyre/cluster/cogs/VariableAction.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/cluster/cogs/VariableParser.py` & `refyre-0.0.1.5.1/refyre/cluster/cogs/VariableParser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/core/RecipePreprocessor.py` & `refyre-0.0.1.5.1/refyre/core/RecipePreprocessor.py`

 * *Files 11% similar despite different names*

```diff
@@ -85,18 +85,11 @@
                 if 'name' in recipe_dict['env']:
                     if not Path(recipe_dict['env']['name']).exists():
                         create_virtualenv_and_install_requirements(venv_path, recipe_dict['env']['requirements'])
                     elif 'refresh' in recipe_dict['env'] and recipe_dict['env']['refresh']:
                         shutil.rmtree(recipe_dict['env']['name'])
                         create_virtualenv_and_install_requirements(recipe_dict['env']['name'], recipe_dict['env']['requirements'])
 
-            #Activate the env 
-            activate_script = (
-                Path(venv_path) / "Scripts" / "activate" if sys.platform == "win32"
-                else Path(venv_path) / "bin" / "activate"
-            )
-            activate_cmd = f"source {activate_script}"
-            subprocess.run(activate_cmd, shell=True, check=True)
 
             return ref
```

### Comparing `refyre-0.0.1.5/refyre/datastack/DataStack.py` & `refyre-0.0.1.5.1/refyre/datastack/DataStack.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/graph/FileGraph.py` & `refyre-0.0.1.5.1/refyre/graph/FileGraph.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/graph/FileGraphNode.py` & `refyre-0.0.1.5.1/refyre/graph/FileGraphNode.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/ExpressionGenerator.py` & `refyre-0.0.1.5.1/refyre/reader/ExpressionGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/Lexer.py` & `refyre-0.0.1.5.1/refyre/reader/Lexer.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/Parser.py` & `refyre-0.0.1.5.1/refyre/reader/Parser.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/PatternGenerator.py` & `refyre-0.0.1.5.1/refyre/reader/PatternGenerator.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/cogs/LexerToken.py` & `refyre-0.0.1.5.1/refyre/reader/cogs/LexerToken.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/reader/cogs/lexer_utils.py` & `refyre-0.0.1.5.1/refyre/reader/cogs/lexer_utils.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/utils/clone.py` & `refyre-0.0.1.5.1/refyre/utils/clone.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/refyre/utils/regex.py` & `refyre-0.0.1.5.1/refyre/utils/regex.py`

 * *Files identical despite different names*

### Comparing `refyre-0.0.1.5/PKG-INFO` & `refyre-0.0.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refyre
-Version: 0.0.1.5
+Version: 0.0.1.5.1
 Summary: Filesystem dominance is all you need.
 Home-page: https://github.com/flockfysh/refyre
 License: MIT
 Keywords: files,manipulation,data science
 Author: Ansh
 Author-email: teamnebulaco@gmail.com
 Requires-Python: >=3.8
@@ -170,15 +170,15 @@
 These are all the basic quantifiers you can use, they cover ~80% of refyre's inner power. The other 20% are pretty obscure and aren't that useful normally.
 
 ### FileClusters (Variables)
 
 Variables are the backbone of refyre. The clusters provide an *avenue* for the variables to easily target the data without worrying about writing any code. However, they aren't the only way to access variable's powers. The docs below, again, specify the most useful abilities for these variables.
 
 `FileCluster(values = [], dirs = [], patterns = [], as_pathlib = False,)`
-    - `values`: string filepaths, or `Path` objects depending on wheterh `as_pathlib` is true or false.
+    - `values`: string filepaths, or `Path` objects depending on whether `as_pathlib` is true or false.
     - `patterns`: corresponds to the dirs, lists what patterns you want to target
 
 FileClusters are strongly rooted in *object oriented operations*, meaning each operation returns another FileCluster, so you can continue channeling FileCluster capabilities. To get out of FileClusters, you can use the following options:
     - `.vals()`: Returns a list of Path objects
     - `.item()`: Returns the first Path object
 
 Using this basic constructor, you can make some easy operations:
```

