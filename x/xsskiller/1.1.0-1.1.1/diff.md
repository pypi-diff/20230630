# Comparing `tmp/xsskiller-1.1.0.tar.gz` & `tmp/xsskiller-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsskiller-1.1.0.tar", last modified: Wed Jun 28 04:22:21 2023, max compression
+gzip compressed data, was "xsskiller-1.1.1.tar", last modified: Fri Jun 30 01:19:40 2023, max compression
```

## Comparing `xsskiller-1.1.0.tar` & `xsskiller-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-28 04:22:21.212841 xsskiller-1.1.0/
--rwxrwxrwx   0 abel      (1000) abel      (1000)      633 2023-06-28 04:22:21.212587 xsskiller-1.1.0/PKG-INFO
--rwxrwxrwx   0 abel      (1000) abel      (1000)      108 2023-06-27 03:13:39.000000 xsskiller-1.1.0/README.md
--rwxrwxrwx   0 abel      (1000) abel      (1000)       38 2023-06-28 04:22:21.212947 xsskiller-1.1.0/setup.cfg
--rwxrwxrwx   0 abel      (1000) abel      (1000)      997 2023-06-28 04:21:44.000000 xsskiller-1.1.0/setup.py
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-28 04:22:21.080772 xsskiller-1.1.0/xsskiller/
--rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-28 04:22:18.000000 xsskiller-1.1.0/xsskiller/__init__.py
--rwxrwxrwx   0 abel      (1000) abel      (1000)     5698 2023-06-28 04:13:34.000000 xsskiller-1.1.0/xsskiller/xsskiller.py
-drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-28 04:22:21.212044 xsskiller-1.1.0/xsskiller.egg-info/
--rwxrwxrwx   0 abel      (1000) abel      (1000)      633 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/PKG-INFO
--rwxrwxrwx   0 abel      (1000) abel      (1000)      263 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/SOURCES.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)        1 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/dependency_links.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/entry_points.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       18 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/requires.txt
--rwxrwxrwx   0 abel      (1000) abel      (1000)       10 2023-06-28 04:22:21.000000 xsskiller-1.1.0/xsskiller.egg-info/top_level.txt
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-30 01:19:40.064446 xsskiller-1.1.1/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     1653 2023-06-30 01:19:40.064289 xsskiller-1.1.1/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      800 2023-06-28 04:56:43.000000 xsskiller-1.1.1/README.md
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       38 2023-06-30 01:19:40.064497 xsskiller-1.1.1/setup.cfg
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      997 2023-06-30 01:15:32.000000 xsskiller-1.1.1/setup.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-30 01:19:40.060922 xsskiller-1.1.1/xsskiller/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-30 01:15:38.000000 xsskiller-1.1.1/xsskiller/__init__.py
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     5730 2023-06-30 01:09:59.000000 xsskiller-1.1.1/xsskiller/xsskiller.py
+drwxrwxrwx   0 abel      (1000) abel      (1000)        0 2023-06-30 01:19:40.063960 xsskiller-1.1.1/xsskiller.egg-info/
+-rwxrwxrwx   0 abel      (1000) abel      (1000)     1653 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/PKG-INFO
+-rwxrwxrwx   0 abel      (1000) abel      (1000)      263 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/SOURCES.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)        1 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/dependency_links.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       56 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/entry_points.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       18 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/requires.txt
+-rwxrwxrwx   0 abel      (1000) abel      (1000)       10 2023-06-30 01:19:39.000000 xsskiller-1.1.1/xsskiller.egg-info/top_level.txt
```

### Comparing `xsskiller-1.1.0/setup.py` & `xsskiller-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="xsskiller",
-    version="1.1.0",
+    version="1.1.1",
     description="Automated tool scans URLS parameters to check if reflected XSS is vulnerable",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/abeljm/XSSKiller",
     author="Avelino Navarro",
     author_email="abeljm2017@gmail.com",
     classifiers=[
```

### Comparing `xsskiller-1.1.0/xsskiller/xsskiller.py` & `xsskiller-1.1.1/xsskiller/xsskiller.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def printError(msg): 
     print(f"{Fore.RED}[-] {msg}{Fore.RESET}")
 
 def printSuccess(msg):
     print(f"{Fore.GREEN}[+] {msg}{Fore.RESET}")
 
-def Send_req(url,payloads,file,verbose, proxy):
+def sendRequest(url,payloads,file,verbose, proxy):
     for payload in payloads:
         payload_enc = urllib.parse.quote(payload)
         new_url = re.sub(r"=[^?\|&]*", "=" + payload_enc, url)
 
         payload_esc = html.escape(payload)
 
         try:
@@ -64,30 +64,28 @@
             else:
                 if verbose:
                     printError(new_url)
 
         except requests.exceptions.HTTPError as e:
             pass
 
-def Threads_req(list_url,list_payloads,workers,file,verbose,proxy):
+def threadRequests(list_url,list_payloads,workers,file,verbose,proxy):
     threads = []
     with ThreadPoolExecutor(max_workers=workers)  as executor:
         for url in list_url:
             url = url.strip()
-            t = executor.submit(Send_req,url,list_payloads,file,verbose,proxy)
+            t = executor.submit(sendRequest,url,list_payloads,file,verbose,proxy)
             threads.append(t)
         wait(threads)
 
-def saveFile(name_file,data):
+def saveFile(name_file, data):
     path = os.getcwd()
-    path_file = "%s/%s" %(path,name_file)
+    path_file = os.path.join(path, name_file)
     with open(path_file, mode='a+', encoding='utf-8') as file:
-        file.write('%s\n' %(data))
-        file.close()
-
+        file.write('%s\n' % data)
 
 def main():    
     parser = argparse.ArgumentParser()
     parser.add_argument('-q', help='Ocultar banner', action='store_true')
     parser.add_argument('-t', '--threads',help='Agregar hilos', type=int, default=3, metavar='')
     parser.add_argument('-u', '--url', help='URL para escanear', metavar='')
     parser.add_argument('-l', '--list', help='Archivo con lista de urls', metavar='')
@@ -123,18 +121,18 @@
     elif args.pipe:
         url = [line.strip() for line in sys.stdin]
 
     elif args.list:
         url = [line.strip() for line in open(args.list,"r")]
 
     else:
-        print("Nesecariamente tiene que poner -u o -l")
+        print("Nesecariamente tiene que poner los argumentos -u --url, -l --list, -s --pipe")
         sys.exit(2)
 
-    Threads_req(url,payloads,args.threads,args.output,args.verbose,args.proxy)
+    threadRequests(url,payloads,args.threads,args.output,args.verbose,args.proxy)
 
     if args.d:
         total_time = time.time() - init_time
         print(f'\nTotal time: {round(total_time, 2)} sec')   
 
 if __name__ == "__main__":
     main()
```

