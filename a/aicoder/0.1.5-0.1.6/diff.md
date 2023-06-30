# Comparing `tmp/aicoder-0.1.5-py3-none-any.whl.zip` & `tmp/aicoder-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20674 bytes, number of entries: 12
+Zip file size: 20764 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12662 b- defN 23-Jun-29 12:24 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8124 b- defN 23-Jun-29 11:29 aicoder/AICoderFull.py
 -rw-r--r--  2.0 unx     4841 b- defN 23-Jun-29 18:56 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3481 b- defN 23-Jun-28 23:49 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    11858 b- defN 23-Jun-29 19:34 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jun-29 19:37 aicoder-0.1.5.dist-info/RECORD
-12 files, 61339 bytes uncompressed, 19094 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx    11973 b- defN 23-Jun-30 00:52 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/RECORD
+12 files, 61454 bytes uncompressed, 19184 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/LICENSE
+Filename: aicoder-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/METADATA
+Filename: aicoder-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/WHEEL
+Filename: aicoder-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/entry_points.txt
+Filename: aicoder-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/top_level.txt
+Filename: aicoder-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.1.5.dist-info/RECORD
+Filename: aicoder-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/main.py

```diff
@@ -3,15 +3,15 @@
 import sys
 import string
 import random
 import requests
 import logging
 import colorlog
 
-from time import sleep
+from concurrent.futures import ThreadPoolExecutor
 
 from aicoder.AICoderFull import AICoderFull
 from aicoder.AICoderPartial import AICoderPartial
 
 # Logger setup
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
@@ -39,127 +39,140 @@
 
 # Function to enhance a file
 def enhancer(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
     aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
     aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch)
 
 # Function to add comments to a file
-def add_comments(api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
-    prompt = "Given some code, add useful comments to the file inside the code to easily understand what it does."
-    aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch)
+def add_comments(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
+    final_prompt = "Given some code, add useful comments to the file inside the code to easily understand what it does."
+    if prompt:
+        final_prompt = "\n" + prompt
+    aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
 
 # Function to check for security vulnerabilities in a file
-def check_security(api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
-    prompt = "Given some code, search for security vulnerabilities and potential backdoors on it and if any, create a new code fixing it (if possible). Return only the fixed code with the comments. If you changed anything, add at the end of the code comments explaining the changes."
-    aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch)
+def check_security(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
+    final_prompt = "Given some code, search for security vulnerabilities and potential backdoors on it and if any, create a new code fixing it (if possible). Return only the fixed code with the comments. If you changed anything, add at the end of the code comments explaining the changes."
+    if prompt:
+        final_prompt = "\n" + prompt
+    aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
 
 # Function to optimize a file
-def optimize_file(api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
-    prompt = "Given some code, optimize it. Return code that keeping the same functionality and respecting the class and function names, it's more clean, simple, don't have duplice code, don't have code smells and is more efficient if possible. If you cannot find any way to improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes."
-    aicoderpartial = AICoderPartial(prompt, api_key, github_token, model)
-    aicoderpartial.modify_file(file_path, prompt, orig_branch, new_branch)
+def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
+    final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
+    final_prompt += "Don't remove comments, just improve them if possible. If you cannot improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes. "
+    final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if the code can be improved the different functionalities must be keeped."
+    if prompt:
+        final_prompt = "\n" + prompt
+    aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
 
 # Function to add common arguments to a parser
 def add_common_arguments(parser):
     parser.add_argument('--api-key', default=None, type=str, help='Input API key')
     parser.add_argument('--model', default="gpt-4", type=str, help='Model to use')
 
 # Main function
 def main():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="mode")  # Create subparsers
 
     # Create subparsers
     full_generator_parser = subparsers.add_parser('full-generator', help='Generate a full program from the prompt.')
     file_generator_parser = subparsers.add_parser('file-generator', help='Generate a file based on others as templates.')
-    file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on others as templates.')
-    file_commentor_parser = subparsers.add_parser('file-commentor', help='Ask to add comments to a file.')
+    file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on the given prompt.')
+    file_commentor_parser = subparsers.add_parser('file-comments', help='Ask to add comments to a file.')
     file_security_parser = subparsers.add_parser('file-security', help='Ask to search security vulnerabilities and backdoors in a file.')
     file_optimizer_parser = subparsers.add_parser('file-optimizer', help='Ask to optimize a file in terms of clean code and efficiency.')
 
     # Add common arguments to each subparser
     for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser]:
         add_common_arguments(subparser)
 
     # Add specific arguments to each subparser
     full_generator_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
+    
     file_generator_parser.add_argument('--template-files', nargs='+', help='List of template files')
     file_generator_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_generator_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_generator_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_generator_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
+    
     file_enhancer_parser.add_argument('--path', type=str, help='Path to file to enhance')
     file_enhancer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_enhancer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_enhancer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     file_enhancer_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
+    
     file_commentor_parser.add_argument('--path', type=str, help='Path to file to enhance')
     file_commentor_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_commentor_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_commentor_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
+    
     file_security_parser.add_argument('--path', type=str, help='Path to file to enhance')
     file_security_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_security_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_security_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
+    
     file_optimizer_parser.add_argument('--path', type=str, help='Path to file to enhance')
     file_optimizer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_optimizer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_optimizer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
+    file_optimizer_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url. In this case, it\'s optional')
     
     # Parse arguments
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
     api_key = os.environ.get("INPUT_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
 
-    if args.mode in ["file-generator", "file-enhancer", "file-commentor", "file-security", "file-optimizer"]:
+    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
 
         if args.mode == "file-generator":
             template_files = list(os.environ.get("TEMPALTE_FILES").split(",")) or args.template_files
         
         elif args.mode == "file-enhancer":
             modify_file_path = os.environ.get("MODIFY_FILE_PATH") or args.path
         
-        elif args.mode in ["file-commentor", "file-security", "file-optimizer"]:
+        elif args.mode in ["file-comments", "file-security", "file-optimizer"]:
             check_path = os.environ.get("CHECK_PATH") or args.path
     
-    if not prompt and not args.mode in ["file-commentor", "file-security", "file-optimizer"]:
+    if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         sys.exit(1)
     
     if not api_key:
         logger.error("Error: Missing API key.")
         sys.exit(1)
     
     # If prompt is file path, read it
     if prompt and os.path.isfile(prompt):
         logger.debug(f"Prompt read from {prompt}")
         with open(prompt, "r") as f:
             prompt = f.read()
     
     # If prompt is url, download it
-    if prompt and prompt.startswith("http"):
+    elif prompt and prompt.startswith("http"):
         logger.debug(f"Prompt downloaded from {prompt}")
         prompt = requests.get(prompt).text
     
     # If full generator mode
     if args.mode == 'full-generator':
         full_generator(prompt, api_key, github_token, model)
         exit(0)
     
     ### Checks for partial generators
     
     if not github_token:
         logger.warning("No Github token. PRs won't be created automatically.")
-        sleep(3)
     
     if github_token and not orig_branch:
         logger.error("Error: No orig branch. PRs won't be created automatically. Stopping.")
         exit(1)
     
     if github_token and not to_branch:
         logger.error("Error: No to branch. PRs won't be created automatically. Stopping.")
@@ -172,45 +185,33 @@
     
     # If file enhancer mode
     elif args.mode == 'file-generator':
         file_generator(prompt, api_key, github_token, model, template_files, orig_branch, to_branch)
         exit(0)
     
     # If file commentor mode
-    elif args.mode in ['file-commentor', 'file-security', 'file-optimizer']:
-        if args.mode == 'file-commentor':
+    elif args.mode in ['file-comments', 'file-security', 'file-optimizer']:
+        # pompt is optional for these modes and usually None
+        if args.mode == 'file-comments':
             f = add_comments
         elif args.mode == 'file-security':
             f = check_security
         elif args.mode == 'file-optimizer':
             f = optimize_file
         
         # Check if path is file or folder
         if os.path.isfile(check_path):
             logger.debug(f"Given path {check_path} is a file.")
-            f(api_key, github_token, model, check_path, orig_branch, to_branch)
+            f(prompt, api_key, github_token, model, check_path, orig_branch, to_branch)
         
         elif os.path.isdir(check_path):
             logger.debug(f"Given path {check_path} is a folder.")
-            for root, dirs, files in os.walk(check_path):
-                for file in files:
-                    logger.debug(f"Checking file: {check_path}")
-                    f(api_key, github_token, model, os.path.join(root, file), orig_branch, to_branch)
-
+            with ThreadPoolExecutor(max_workers=3) as executor:
+                for root, dirs, files in os.walk(check_path):
+                    for file in files:
+                        logger.debug(f"Checking file: {check_path}")
+                        executor.submit(f, prompt, api_key, github_token, model, os.path.join(root, file), orig_branch, to_branch)
         exit(0)
 
     
 if __name__ == "__main__":
     main()
-
-# Changes made:
-# 1. Removed unused imports.
-# 2. Removed redundant comments.
-# 3. Simplified the get_random_string function.
-# 4. Simplified the main function by removing redundant checks and conditions.
-# 5. Simplified the argument parsing by removing redundant checks and conditions.
-# 6. Simplified the file checking process by removing redundant checks and conditions.
-# 7. Removed redundant exit calls.
-# 8. Simplified the prompt reading process by removing redundant checks and conditions.
-# 9. Simplified the prompt downloading process by removing redundant checks and conditions.
-# 10. Simplified the mode checking process by removing redundant checks and conditions.
-# 11. Simplified the file or folder checking process by removing redundant checks and conditions.
```

## Comparing `aicoder-0.1.5.dist-info/LICENSE` & `aicoder-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.1.5.dist-info/RECORD` & `aicoder-0.1.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=3k5YLO_cyLZh6d0vGf6P7GN50PexLORBy0EUs9pXaJQ,12662
 aicoder/AICoderFull.py,sha256=ThwfD0mSBiCzuMRNsZCUY_wL4gRUVHXRXkg3oc0dqks,8124
 aicoder/AICoderPartial.py,sha256=ORsww0_CenhiLu2H-pajES2Kn7r0idnWPUPcz02h7O4,4841
 aicoder/AICoderPrompts.py,sha256=ZQGA2rNfSHzYdmc914960_HOJagGO_AuRXn_08sMeW4,3481
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=KrwiF5q8ld9_yRSSCQZbVG0jCjnqjC6J0_AlC8BgfTo,11858
-aicoder-0.1.5.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.1.5.dist-info/METADATA,sha256=6LIBeTv797s7ikj01k4lcobacNyubXa_-LWN-BZPT04,473
-aicoder-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.1.5.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.1.5.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.1.5.dist-info/RECORD,,
+aicoder/main.py,sha256=SfZk3j4pRXGEXHX2qr5FPSU4kIZBTN2aPWrewUbE088,11973
+aicoder-0.1.6.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.1.6.dist-info/METADATA,sha256=6gadBDfeFA7Bg3J-z0RW0YkbZfF2bf7QDsPecfuTCcQ,473
+aicoder-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.1.6.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.1.6.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.1.6.dist-info/RECORD,,
```

