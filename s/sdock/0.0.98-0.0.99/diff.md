# Comparing `tmp/sdock-0.0.98.tar.gz` & `tmp/sdock-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.0.98.tar", last modified: Mon Jan 30 05:32:21 2023, max compression
+gzip compressed data, was "sdock-0.0.99.tar", last modified: Mon Jan 30 20:32:17 2023, max compression
```

## Comparing `sdock-0.0.98.tar` & `sdock-0.0.99.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 05:32:21.714479 sdock-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-30 05:32:15.000000 sdock-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 05:32:21.714479 sdock-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-30 05:32:15.000000 sdock-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 05:32:21.710479 sdock-0.0.98/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-01-30 05:32:15.000000 sdock-0.0.98/sdock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 05:32:21.714479 sdock-0.0.98/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 05:32:21.000000 sdock-0.0.98/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-30 05:32:21.000000 sdock-0.0.98/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 05:32:21.000000 sdock-0.0.98/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 05:32:21.000000 sdock-0.0.98/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 05:32:21.000000 sdock-0.0.98/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 05:32:21.714479 sdock-0.0.98/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3161 2023-01-30 05:32:15.000000 sdock-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-30 20:32:13.000000 sdock-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 20:32:17.570637 sdock-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-30 20:32:13.000000 sdock-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-01-30 20:32:13.000000 sdock-0.0.99/sdock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 20:32:17.570637 sdock-0.0.99/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3161 2023-01-30 20:32:13.000000 sdock-0.0.99/setup.py
```

### Comparing `sdock-0.0.98/LICENSE` & `sdock-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.0.98/sdock/__init__.py` & `sdock-0.0.99/sdock/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,40 @@
 def wget(url, verify=True):
 	to = url.split('/')[-1].replace('%20','_')
 	if not os.path.exists(to):
 		resp = requests.get(url, allow_redirects=True,verify=verify)
 		open(to,'wb').write(resp.content)
 	return to
 
-def extract_ova_from_zip(local_zipfile):
+def extract_file_from_zip(zipfile, extractedfile):
 	import zipfile
 
-	ovafile = os.path.basename(local_zipfile).replace('.zip','.ova')
-	if not os.path.exists(ovafile):
+	if not os.path.exists(extractedfile):
 		cur_folder = os.path.abspath(os.curdir)
 		with zipfile.ZipFile(local_zipfile,"r") as zip_ref:
 			zip_ref.extractall(cur_folder)
 		os.remove(local_zipfile)
 
-	return ovafile if os.path.exists(ovafile) else None
+	return extractedfile if os.path.exists(extractedfile) else None
+
+
+def extract_ova_from_zip(local_zipfile):
+	if False:
+		import zipfile
+
+		ovafile = os.path.basename(local_zipfile).replace('.zip','.ova')
+		if not os.path.exists(ovafile):
+			cur_folder = os.path.abspath(os.curdir)
+			with zipfile.ZipFile(local_zipfile,"r") as zip_ref:
+				zip_ref.extractall(cur_folder)
+			os.remove(local_zipfile)
+
+		return ovafile if os.path.exists(ovafile) else None
+	else:
+		return extract_file_from_zip(local_zipfile, os.path.basename(local_zipfile).replace('.zip','.ova'))
 
 def open_port():
 	"""
 	https://gist.github.com/jdavis/4040223
 	"""
 
 	import socket
@@ -209,15 +224,15 @@
 		if self.ovafile:
 			self.import_ova(self.ovafile)
 
 		self.disable()
 		if self.sharedfolder:
 			self.__shared_folder(self.sharedfolder)
 		
-		for file in self.uploadfiles:
+		for file in list(self.uploadfiles):
 			self.uploadfile(file)
 
 		if False:			
 			self.start()
 			for cmd in self.cmds_to_exe_with_network:
 				self.vbexe(cmd)
 
@@ -333,15 +348,16 @@
 ))
 		return "on_start.ps1"
 
 	def add_file(self, foil, directory="C:\\\\Users\\\\vagrant\\\\Desktop"):
 		return """ win10.vm.provision "file", source: "{0}", destination: "{1}\\\\{0}" """.format(foil, directory)
 
 
-	def prep(self):		
+	def prep(self):
+		self.uploadfiles = list(self.uploadfiles)	
 		self.uploadfiles += [self.write_startup_file()]
 		uploading_file_strings = []
 		for foil in self.uploadfiles:
 			uploading_file_strings += [self.add_file(foil)]
 
 		uploading_file_strings += [
 			self.add_file(self.create_runner(),"""C:\\\\Users\\\\vagrant\\\\AppData\\\\Roaming\\\\Microsoft\\\\Windows\\\\Start Menu\\\\Programs\\\\Startup""")
@@ -439,10 +455,10 @@
 	
 	def destroy(self):
 		self.vagrant_name
 		exe(""" vagrant destroy -f """)
 		for foil in ["Vagrant", "on_start*", "on_login*"]:
 			exe("rm {0}".format(foil))
 		exe("yes|rm -r .vagrant/")
-		for foil in self.uploadfiles:
+		for foil in list(self.uploadfiles):
 			if foil not in self.save_files:
 				exe("rm {0}".format(foil))
```

### Comparing `sdock-0.0.98/setup.py` & `sdock-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.7.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.98"
+VERSION = "0.0.99"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

