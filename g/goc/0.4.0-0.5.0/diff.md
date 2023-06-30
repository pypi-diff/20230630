# Comparing `tmp/goc-0.4.0.tar.gz` & `tmp/goc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goc-0.4.0.tar", max compression
+gzip compressed data, was "goc-0.5.0.tar", max compression
```

## Comparing `goc-0.4.0.tar` & `goc-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2826 2023-06-29 12:41:14.732571 goc-0.4.0/README.md
--rw-r--r--   0        0        0     2949 2023-06-30 12:49:46.648908 goc-0.4.0/goc/goc.py
--rw-r--r--   0        0        0      414 2023-06-30 12:49:46.649369 goc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 goc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3469 2023-06-30 14:34:39.385378 goc-0.5.0/README.md
+-rw-r--r--   0        0        0     3020 2023-06-30 14:34:39.385624 goc-0.5.0/goc/goc.py
+-rw-r--r--   0        0        0      414 2023-06-30 14:34:39.385857 goc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4047 1970-01-01 00:00:00.000000 goc-0.5.0/PKG-INFO
```

### Comparing `goc-0.4.0/README.md` & `goc-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,43 +27,60 @@
 ```
 
 ## Usage
 
 To execute the script, run the following command:
 
 ```bash
-goc [arguments]
+goc [mode] [arguments]
 ```
 
-Replace `[arguments]` with the appropriate options based on your requirement:
+Replace [mode] with one of the following options:
 
-- **Document Latest Commit**:
+diff: Generate documentation for the git diff between commits or files.
+commit: Generate a commit message for the current git diff.
+Replace [arguments] based on the mode selected:
+
+For the diff mode, provide the arguments to specify the commits or files to compare.
+For the commit mode, no additional arguments are needed.
+
+- **Generate documentation for the diff between two commits**:
   ```bash
-  goc
+  goc diff [commit_a] [commit_b]
   ```
 
 - **Document Comparison vs Current Commit**:
   ```bash
-  goc [commit_hash]
+  goc diff [commit_hash]
+  ```
+
+- **Document Comparison of a single commit**:
+  ```bash
+  goc diff [commit_hash]^!
   ```
 
-- **Document Comparison of Two Commits**:
+- **Document Staged Changes**:
   ```bash
-  goc [commit_a] [commit_b]
+  goc diff --staged
+  ```
+
+- **Automatically generate commit message and commit**:
+  ```bash
+  goc commit
   ```
 
 ## Output
 
 The script generates Markdown documentation by utilizing the OpenAI GPT-3.5 Turbo model. The resulting documentation will be displayed in the console output.
 
 
 ## Examples
 
 ```bash
-$ goc a0f72101be85667a362425c2cdc30ef794e2a738
+$ goc diff a0f72101be85667a362425c2cdc30ef794e2a738
 ## Commit Details
 
 - **Commit Type:** Code update
 - **Commit Scope:** goc.py, pyproject.toml
 - **Commit Description:**
 
 ### goc.py
@@ -74,14 +91,19 @@
 
 ### pyproject.toml
 1. Updated the version to `"0.2.0"`.
 
 Please review and merge these changes.
 ```
 
+```bash
+$ goc commit
+Committing with message: "Update git diff handling, handle case when no diff is found"
+```
+
 ## Note
 
 Make sure you have the necessary permissions and access to the Git repository you intend to analyze. Also, ensure that the repository is properly cloned on your local machine.
 
 ## Disclaimer
 
 This tool relies on the OpenAI GPT-3.5 Turbo model for generating documentation. The accuracy and quality of the generated content depend on the model's training data and the provided input. Please review and validate the generated documentation before using it in your projects.
```

### Comparing `goc-0.4.0/goc/goc.py` & `goc-0.5.0/goc/goc.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,24 +18,25 @@
     ]
     return prompt_chain
 
 def document_git_diff_wrap(args):
     fmt_args = " ".join(args)
     cmd = f"git diff {fmt_args}"
     git_diff = exec_bash_cmd(cmd)
+    if len(git_diff) == 0:
+        print('No Git Diff Found')
+        return []
     prompt_chain = [
         'I send you a git diff, and you write documentation of the commit in markdown',
         git_diff
     ]
     return prompt_chain
 
 def git_commit_wrap():
-    # compare latest 2 commits
-    commit_hash = exec_bash_cmd("git log | egrep '^commit ' | head -n 1 | awk '{print $NF}'")
-    cmd = f"git diff {commit_hash}"
+    cmd = f"git diff --staged"
     git_diff = exec_bash_cmd(cmd)
     prompt_chain = [
         'I send you a git diff, and you write a commit message in 50 characters or less, do not include "git commit"',
         git_diff
     ]
     return prompt_chain
 
@@ -70,34 +71,41 @@
 
 Options:
   help             Show this help text.
 
 """
     print(helptext)
 
-def goc():
+def get_args():
     n_args = len(sys.argv) - 1
     if n_args == 0:
         print('No Arguments, Please run "goc <mode> <args>"')
+        mode = 'help'
     elif n_args > 0:
         mode = sys.argv[1]
-        if mode == 'help':
-            print_help_text()
-            return
-        if mode == 'diff':
-            # just pass the args directly into git diff
-            prompt_chain = document_git_diff_wrap(sys.argv[2:])
-        elif mode == 'commit':
-            # get description of the current diff
-            prompt_chain = git_commit_wrap()
+    return mode
 
-    resp = execute_prompt_chain(prompt_chain)
-    gpt_output = parse_gpt_resp(resp)
+def goc():
+    mode = get_args()
+    prompt_chain = []
+    if mode == 'help':
+        print_help_text()
+        return
     if mode == 'diff':
-        print(gpt_output)
+        # just pass the args directly into git diff
+        prompt_chain = document_git_diff_wrap(sys.argv[2:])
     elif mode == 'commit':
-        print('Committing with message: ' + gpt_output)
-        do_git_commit(gpt_output)
+        # get description of the current diff
+        prompt_chain = git_commit_wrap()
+
+    if len(prompt_chain) > 0:
+        resp = execute_prompt_chain(prompt_chain)
+        gpt_output = parse_gpt_resp(resp)
+        if mode == 'diff':
+            print(gpt_output)
+        elif mode == 'commit':
+            print('Committing with message: ' + gpt_output)
+            do_git_commit(gpt_output)
 
 
 if __name__ == '__main__':
     goc()
```

### Comparing `goc-0.4.0/PKG-INFO` & `goc-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goc
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/djentleman/goc
 Author: Todd Perry
 Author-email: toddperry171@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -44,43 +44,60 @@
 ```
 
 ## Usage
 
 To execute the script, run the following command:
 
 ```bash
-goc [arguments]
+goc [mode] [arguments]
 ```
 
-Replace `[arguments]` with the appropriate options based on your requirement:
+Replace [mode] with one of the following options:
 
-- **Document Latest Commit**:
+diff: Generate documentation for the git diff between commits or files.
+commit: Generate a commit message for the current git diff.
+Replace [arguments] based on the mode selected:
+
+For the diff mode, provide the arguments to specify the commits or files to compare.
+For the commit mode, no additional arguments are needed.
+
+- **Generate documentation for the diff between two commits**:
   ```bash
-  goc
+  goc diff [commit_a] [commit_b]
   ```
 
 - **Document Comparison vs Current Commit**:
   ```bash
-  goc [commit_hash]
+  goc diff [commit_hash]
+  ```
+
+- **Document Comparison of a single commit**:
+  ```bash
+  goc diff [commit_hash]^!
   ```
 
-- **Document Comparison of Two Commits**:
+- **Document Staged Changes**:
   ```bash
-  goc [commit_a] [commit_b]
+  goc diff --staged
+  ```
+
+- **Automatically generate commit message and commit**:
+  ```bash
+  goc commit
   ```
 
 ## Output
 
 The script generates Markdown documentation by utilizing the OpenAI GPT-3.5 Turbo model. The resulting documentation will be displayed in the console output.
 
 
 ## Examples
 
 ```bash
-$ goc a0f72101be85667a362425c2cdc30ef794e2a738
+$ goc diff a0f72101be85667a362425c2cdc30ef794e2a738
 ## Commit Details
 
 - **Commit Type:** Code update
 - **Commit Scope:** goc.py, pyproject.toml
 - **Commit Description:**
 
 ### goc.py
@@ -91,14 +108,19 @@
 
 ### pyproject.toml
 1. Updated the version to `"0.2.0"`.
 
 Please review and merge these changes.
 ```
 
+```bash
+$ goc commit
+Committing with message: "Update git diff handling, handle case when no diff is found"
+```
+
 ## Note
 
 Make sure you have the necessary permissions and access to the Git repository you intend to analyze. Also, ensure that the repository is properly cloned on your local machine.
 
 ## Disclaimer
 
 This tool relies on the OpenAI GPT-3.5 Turbo model for generating documentation. The accuracy and quality of the generated content depend on the model's training data and the provided input. Please review and validate the generated documentation before using it in your projects.
```

