# Comparing `tmp/aicoder-0.1.6-py3-none-any.whl.zip` & `tmp/aicoder-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20764 bytes, number of entries: 12
+Zip file size: 20848 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    12662 b- defN 23-Jun-29 12:24 aicoder/AICoder.py
 -rw-r--r--  2.0 unx     8124 b- defN 23-Jun-29 11:29 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     4841 b- defN 23-Jun-29 18:56 aicoder/AICoderPartial.py
+-rw-r--r--  2.0 unx     4847 b- defN 23-Jun-30 01:18 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3481 b- defN 23-Jun-28 23:49 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    11973 b- defN 23-Jun-30 00:52 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 00:52 aicoder-0.1.6.dist-info/RECORD
-12 files, 61454 bytes uncompressed, 19184 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx    12724 b- defN 23-Jun-30 08:45 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 08:46 aicoder-0.1.7.dist-info/RECORD
+12 files, 62211 bytes uncompressed, 19268 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/LICENSE
+Filename: aicoder-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/METADATA
+Filename: aicoder-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/WHEEL
+Filename: aicoder-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/entry_points.txt
+Filename: aicoder-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/top_level.txt
+Filename: aicoder-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.1.6.dist-info/RECORD
+Filename: aicoder-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoderPartial.py

```diff
@@ -3,15 +3,15 @@
 import colorlog
 import subprocess
 import os
 from github import Github
 from .AICoderPrompts import MODIFY_FILE, FILE_FROM_TEMPALTES
 from .AICoder import AICoder
 
-
+# Setting up logger
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
@@ -60,15 +60,15 @@
         # Create needed folders
         self.create_folder(final_file_path)
 
         # Prepare message
         logger.info(f"Generating {final_file_path} file from templates {', '.join(template_file_paths)}...")
         msg = FILE_FROM_TEMPALTES.replace("__FINAL_FILE_PATH__", final_file_path).replace("__PROMPT__", prompt)
         for f_path in template_file_paths:
-            with open(template_file_paths, "r") as f:
+            with open(f_path, "r") as f:
                 f_path_content = f.read()
                 msg += f"\nThe template file {f_path} has the following content:\n\n{f_path_content}\n\n"
         
         # Get new content
         new_content = self.contact(msg)
         new_content = self.remove_fences(new_content)
```

## aicoder/main.py

```diff
@@ -56,93 +56,102 @@
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
 
 # Function to optimize a file
 def optimize_file(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
-    final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
+    final_prompt = "Given some code, optimize it without loosing functionality. Return a code that keeping the same functionality and respecting the class and function names, it's more clean and beautiful, simple, don't have duplice code, don't have code smells and is more efficient if possible. "
     final_prompt += "Don't remove comments, just improve them if possible. If you cannot improve the code just return the same code. If you changed anything, add at the end of the code comments explaining the changes. "
-    final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if the code can be improved the different functionalities must be keeped."
+    final_prompt += "Be careful with chunks of code that looks similar but aren't exactly the same, even if part of the code can be improved the different functionalities must be keeped."
+    if prompt:
+        final_prompt = "\n" + prompt
+    aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
+    aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
+
+# Function to fix bugs in a file
+def fix_bugs(prompt: str, api_key: str, github_token: str, model: str, file_path: str, orig_branch: str, new_branch: str):
+    final_prompt = "Given some code and keeping the same functionality fix all the bugs in it. Also, don't remove comments, just improve them if possible."
     if prompt:
         final_prompt = "\n" + prompt
     aicoderpartial = AICoderPartial(final_prompt, api_key, github_token, model)
     aicoderpartial.modify_file(file_path, final_prompt, orig_branch, new_branch)
 
 # Function to add common arguments to a parser
 def add_common_arguments(parser):
     parser.add_argument('--api-key', default=None, type=str, help='Input API key')
     parser.add_argument('--model', default="gpt-4", type=str, help='Model to use')
+    parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
 
 # Main function
 def main():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="mode")  # Create subparsers
 
     # Create subparsers
     full_generator_parser = subparsers.add_parser('full-generator', help='Generate a full program from the prompt.')
     file_generator_parser = subparsers.add_parser('file-generator', help='Generate a file based on others as templates.')
     file_enhancer_parser = subparsers.add_parser('file-enhancer', help='Enhance a file based on the given prompt.')
     file_commentor_parser = subparsers.add_parser('file-comments', help='Ask to add comments to a file.')
     file_security_parser = subparsers.add_parser('file-security', help='Ask to search security vulnerabilities and backdoors in a file.')
     file_optimizer_parser = subparsers.add_parser('file-optimizer', help='Ask to optimize a file in terms of clean code and efficiency.')
+    file_bug_fixer_parser = subparsers.add_parser('file-bug-fixer', help='Ask to fix bugs in a file.')
 
     # Add common arguments to each subparser
     for subparser in [full_generator_parser, file_generator_parser, file_enhancer_parser, file_commentor_parser, file_security_parser, file_optimizer_parser]:
         add_common_arguments(subparser)
 
     # Add specific arguments to each subparser
     full_generator_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
     
     file_generator_parser.add_argument('--template-files', nargs='+', help='List of template files')
     file_generator_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_generator_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_generator_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
-    file_generator_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
     
     file_enhancer_parser.add_argument('--path', type=str, help='Path to file to enhance')
     file_enhancer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_enhancer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_enhancer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
-    file_enhancer_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url.')
     
-    file_commentor_parser.add_argument('--path', type=str, help='Path to file to enhance')
+    file_commentor_parser.add_argument('--path', type=str, help='Path to file or folder to add comments')
     file_commentor_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_commentor_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_commentor_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     
-    file_security_parser.add_argument('--path', type=str, help='Path to file to enhance')
+    file_security_parser.add_argument('--path', type=str, help='Path to file or folder to search vulnerabilities')
     file_security_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_security_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_security_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     
-    file_optimizer_parser.add_argument('--path', type=str, help='Path to file to enhance')
+    file_optimizer_parser.add_argument('--path', type=str, help='Path to file or folder to optimize')
     file_optimizer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
     file_optimizer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
     file_optimizer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
-    file_optimizer_parser.add_argument('--prompt', default=None, type=str, help='Input prompt. It can be string, a file path or a url. In this case, it\'s optional')
+
+    file_bug_fixer_parser.add_argument('--path', type=str, help='Path to file or folder to fix bugs')
+    file_bug_fixer_parser.add_argument('--github-token', default=None, type=str, help='Github token')
+    file_bug_fixer_parser.add_argument('--orig-branch', default=None, type=str, help='Branch to upload the changes.')
+    file_bug_fixer_parser.add_argument('--to-branch', default=None, type=str, help='Branch to send the PR to.')
     
     # Parse arguments
     args = parser.parse_args()
     prompt = os.environ.get("INPUT_PROMPT") or (args.prompt if hasattr(args,"prompt") else None)
     api_key = os.environ.get("INPUT_API_KEY") or (args.api_key if hasattr(args,"api_key") else None)
     model = os.environ.get("INPUT_MODEL") or (args.model if hasattr(args,"model") else None)
 
-    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer"]:
+    if args.mode in ["file-generator", "file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bug-fixer"]:
         github_token = os.environ.get("GITHUB_TOKEN") or args.github_token
         orig_branch = os.environ.get("ORIGIN_BRANCH") or args.orig_branch
         to_branch = os.environ.get("TO_BRANCH") or args.to_branch
 
         if args.mode == "file-generator":
             template_files = list(os.environ.get("TEMPALTE_FILES").split(",")) or args.template_files
-        
-        elif args.mode == "file-enhancer":
-            modify_file_path = os.environ.get("MODIFY_FILE_PATH") or args.path
-        
-        elif args.mode in ["file-comments", "file-security", "file-optimizer"]:
+                
+        elif args.mode in ["file-enhancer", "file-comments", "file-security", "file-optimizer", "file-bug-fixer"]:
             check_path = os.environ.get("CHECK_PATH") or args.path
     
     if not prompt and not args.mode in ["file-comments", "file-security", "file-optimizer"]:
         logger.error("Error: Missing prompt.")
         sys.exit(1)
     
     if not api_key:
@@ -173,34 +182,33 @@
     if github_token and not orig_branch:
         logger.error("Error: No orig branch. PRs won't be created automatically. Stopping.")
         exit(1)
     
     if github_token and not to_branch:
         logger.error("Error: No to branch. PRs won't be created automatically. Stopping.")
         exit(1)
-
-    # If file enhancer mode
-    if args.mode == 'file-enhancer':
-        enhancer(prompt, api_key, github_token, model, modify_file_path, orig_branch, to_branch)
-        exit(0)
     
     # If file enhancer mode
     elif args.mode == 'file-generator':
         file_generator(prompt, api_key, github_token, model, template_files, orig_branch, to_branch)
         exit(0)
     
     # If file commentor mode
-    elif args.mode in ['file-comments', 'file-security', 'file-optimizer']:
-        # pompt is optional for these modes and usually None
-        if args.mode == 'file-comments':
+    elif args.mode in ['file-enhancer', 'file-comments', 'file-security', 'file-optimizer', 'file-bug-fixer']:
+        # pompt is optional for all these modes except file-enhancer
+        if args.mode == 'file-enhancer':
+            f = enhancer
+        elif args.mode == 'file-comments':
             f = add_comments
         elif args.mode == 'file-security':
             f = check_security
         elif args.mode == 'file-optimizer':
             f = optimize_file
+        elif args.mode == 'file-bug-fixer':
+            f = fix_bugs
         
         # Check if path is file or folder
         if os.path.isfile(check_path):
             logger.debug(f"Given path {check_path} is a file.")
             f(prompt, api_key, github_token, model, check_path, orig_branch, to_branch)
         
         elif os.path.isdir(check_path):
```

## Comparing `aicoder-0.1.6.dist-info/LICENSE` & `aicoder-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.1.6.dist-info/RECORD` & `aicoder-0.1.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aicoder/AICoder.py,sha256=3k5YLO_cyLZh6d0vGf6P7GN50PexLORBy0EUs9pXaJQ,12662
 aicoder/AICoderFull.py,sha256=ThwfD0mSBiCzuMRNsZCUY_wL4gRUVHXRXkg3oc0dqks,8124
-aicoder/AICoderPartial.py,sha256=ORsww0_CenhiLu2H-pajES2Kn7r0idnWPUPcz02h7O4,4841
+aicoder/AICoderPartial.py,sha256=PAJfK6SymyM7uRg4eeuVlSQjl3sfcb10Stg8-2wrfYI,4847
 aicoder/AICoderPrompts.py,sha256=ZQGA2rNfSHzYdmc914960_HOJagGO_AuRXn_08sMeW4,3481
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=SfZk3j4pRXGEXHX2qr5FPSU4kIZBTN2aPWrewUbE088,11973
-aicoder-0.1.6.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.1.6.dist-info/METADATA,sha256=6gadBDfeFA7Bg3J-z0RW0YkbZfF2bf7QDsPecfuTCcQ,473
-aicoder-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.1.6.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.1.6.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.1.6.dist-info/RECORD,,
+aicoder/main.py,sha256=1KUIHIGMcyr4UI9LVBp8y-TfUpBFfzh0LzfMZTl_TSE,12724
+aicoder-0.1.7.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.1.7.dist-info/METADATA,sha256=RXcLylsyIJiy-7CeZNiiM-b5XsqrodrS7TFlEJADk64,473
+aicoder-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.1.7.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.1.7.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.1.7.dist-info/RECORD,,
```

