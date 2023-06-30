# Comparing `tmp/subdomain_chopper-0.1.1.tar.gz` & `tmp/subdomain_chopper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdomain_chopper-0.1.1.tar", max compression
+gzip compressed data, was "subdomain_chopper-1.0.0.tar", max compression
```

## Comparing `subdomain_chopper-0.1.1.tar` & `subdomain_chopper-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      291 2023-06-30 17:55:27.505278 subdomain_chopper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2576 2023-06-30 17:50:47.343292 subdomain_chopper-0.1.1/subdomain_chopper.py
--rw-r--r--   0        0        0      447 2023-06-30 17:55:28.875347 subdomain_chopper-0.1.1/setup.py
--rw-r--r--   0        0        0      251 2023-06-30 17:55:28.875561 subdomain_chopper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-06-30 17:58:11.925105 subdomain_chopper-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-30 17:57:44.309095 subdomain_chopper-1.0.0/subdomain_chopper.py
+-rw-r--r--   0        0        0      447 2023-06-30 17:58:14.939198 subdomain_chopper-1.0.0/setup.py
+-rw-r--r--   0        0        0      251 2023-06-30 17:58:14.939360 subdomain_chopper-1.0.0/PKG-INFO
```

### Comparing `subdomain_chopper-0.1.1/subdomain_chopper.py` & `subdomain_chopper-1.0.0/subdomain_chopper.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 if __name__ == '__main__':
 
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("--domainfile")
+    parser.add_argument("--domainfile", required=True, help="Path to a newline-separated list of domains.")
     args = parser.parse_args()
 
     domain_file_path = args.domainfile
     domain_file_path_permuted = domain_file_path + '.chopped'
 
     domains_normal = read_domain_file(domain_file_path)
```

