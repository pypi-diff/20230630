# Comparing `tmp/aicoder-0.1.7-py3-none-any.whl.zip` & `tmp/aicoder-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20848 bytes, number of entries: 12
+Zip file size: 20843 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12662 b- defN 23-Jun-29 12:24 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8124 b- defN 23-Jun-29 11:29 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     4847 b- defN 23-Jun-30 01:18 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3481 b- defN 23-Jun-28 23:49 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    12724 b- defN 23-Jun-30 08:45 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/RECORD
-12 files, 62211 bytes uncompressed, 19268 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx    12719 b- defN 23-Jun-30 08:51 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 08:51 aicoder-0.1.8.dist-info/RECORD
+12 files, 62206 bytes uncompressed, 19263 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/LICENSE
+Filename: aicoder-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/METADATA
+Filename: aicoder-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/WHEEL
+Filename: aicoder-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/entry_points.txt
+Filename: aicoder-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/top_level.txt
+Filename: aicoder-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.1.7.dist-info/RECORD
+Filename: aicoder-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/main.py

```diff
@@ -90,15 +90,15 @@
     # Create subparsers
     full_generator_parser = subparsers.add_parser('full-generator', help='Generate a full program from the prompt.')
     file_generator_parser = subparsers.add_parser('file-generator', help='Generate a file based on others as templates.')
     file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on the given prompt.')
     file_commentor_parser = subparsers.add_parser('file-comments', help='Ask to add comments to a file.')
     file_security_parser = subparsers.add_parser('file-security', help='Ask to search security vulnerabilities and backdoors in a file.')
     file_optimizer_parser = subparsers.add_parser('file-optimizer', help='Ask to optimize a file in terms of clean code and efficiency.')
-    file_bug_fixer_parser = subparsers.add_parser('file-bug-fixer', help='Ask to fix bugs in a file.')
+    file_bug_fixer_parser = subparsers.add_parser('file-bugfixer', help='Ask to fix bugs in a file.')
 
     # Add common arguments to each subparser
     for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser]:
         add_common_arguments(subparser)
 
     # Add specific arguments to each subparser
     full_generator_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
@@ -135,23 +135,23 @@
     
     # Parse arguments
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
     api_key = os.environ.get("INPUT_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
 
-    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bug-fixer"]:
+    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
 
         if args.mode == "file-generator":
             template_files = list(os.environ.get("TEMPALTE_FILES").split(",")) or args.template_files
                 
-        elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bug-fixer"]:
+        elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bugfixer"]:
             check_path = os.environ.get("CHECK_PATH") or args.path
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         sys.exit(1)
     
     if not api_key:
@@ -189,25 +189,25 @@
     
     # If file enhancer mode
     elif args.mode == 'file-generator':
         file_generator(prompt, api_key, github_token, model, template_files, orig_branch, to_branch)
         exit(0)
     
     # If file commentor mode
-    elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bug-fixer']:
+    elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bugfixer']:
         # pompt is optional for all these modes except file-enhancer
         if args.mode == 'file-enhancer':
             f = enhancer
         elif args.mode == 'file-comments':
             f = add_comments
         elif args.mode == 'file-security':
             f = check_security
         elif args.mode == 'file-optimizer':
             f = optimize_file
-        elif args.mode == 'file-bug-fixer':
+        elif args.mode == 'file-bugfixer':
             f = fix_bugs
         
         # Check if path is file or folder
         if os.path.isfile(check_path):
             logger.debug(f"Given path {check_path} is a file.")
             f(prompt, api_key, github_token, model, check_path, orig_branch, to_branch)
```

## Comparing `aicoder-0.1.7.dist-info/LICENSE` & `aicoder-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.1.7.dist-info/RECORD` & `aicoder-0.1.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=3k5YLO_cyLZh6d0vGf6P7GN50PexLORBy0EUs9pXaJQ,12662
 aicoder/AICoderFull.py,sha256=ThwfD0mSBiCzuMRNsZCUY_wL4gRUVHXRXkg3oc0dqks,8124
 aicoder/AICoderPartial.py,sha256=PAJfK6SymyM7uRg4eeuVlSQjl3sfcb10Stg8-2wrfYI,4847
 aicoder/AICoderPrompts.py,sha256=ZQGA2rNfSHzYdmc914960_HOJagGO_AuRXn_08sMeW4,3481
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=1KUIHIGMcyr4UI9LVBp8y-TfUpBFfzh0LzfMZTl_TSE,12724
-aicoder-0.1.7.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.1.7.dist-info/METADATA,sha256=RXcLylsyIJiy-7CeZNiiM-b5XsqrodrS7TFlEJADk64,473
-aicoder-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.1.7.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.1.7.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.1.7.dist-info/RECORD,,
+aicoder/main.py,sha256=yxtJpdQ9CLQiJxyY0XkJWGXpIH53Mlh49QWtEK5fHy8,12719
+aicoder-0.1.8.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.1.8.dist-info/METADATA,sha256=5_eM0DjkLdnxtwp5jnSQ8IGJF0h-EVmJrNhXiIzNEzo,473
+aicoder-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.1.8.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.1.8.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.1.8.dist-info/RECORD,,
```

