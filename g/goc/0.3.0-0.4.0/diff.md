# Comparing `tmp/goc-0.3.0.tar.gz` & `tmp/goc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goc-0.3.0.tar", max compression
+gzip compressed data, was "goc-0.4.0.tar", max compression
```

## Comparing `goc-0.3.0.tar` & `goc-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2826 2023-06-29 12:41:14.732571 goc-0.3.0/README.md
--rw-r--r--   0        0        0     1642 2023-06-29 12:11:57.261384 goc-0.3.0/goc/goc.py
--rw-r--r--   0        0        0      414 2023-06-29 12:41:39.532537 goc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 goc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-06-29 12:41:14.732571 goc-0.4.0/README.md
+-rw-r--r--   0        0        0     2949 2023-06-30 12:49:46.648908 goc-0.4.0/goc/goc.py
+-rw-r--r--   0        0        0      414 2023-06-30 12:49:46.649369 goc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 goc-0.4.0/PKG-INFO
```

### Comparing `goc-0.3.0/README.md` & `goc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `goc-0.3.0/goc/goc.py` & `goc-0.4.0/goc/goc.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,36 +24,80 @@
     git_diff = exec_bash_cmd(cmd)
     prompt_chain = [
         'I send you a git diff, and you write documentation of the commit in markdown',
         git_diff
     ]
     return prompt_chain
 
+def git_commit_wrap():
+    # compare latest 2 commits
+    commit_hash = exec_bash_cmd("git log | egrep '^commit ' | head -n 1 | awk '{print $NF}'")
+    cmd = f"git diff {commit_hash}"
+    git_diff = exec_bash_cmd(cmd)
+    prompt_chain = [
+        'I send you a git diff, and you write a commit message in 50 characters or less, do not include "git commit"',
+        git_diff
+    ]
+    return prompt_chain
+
 def execute_prompt_chain(prompt_chain):
     resp = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "assistant", "content": cmd}
             for cmd in prompt_chain
         ]
     )    
     return resp
 
 def parse_gpt_resp(resp):
-    md_output = resp['choices'][-1]['message']['content']
-    return md_output
+    gpt_output = resp['choices'][-1]['message']['content']
+    return gpt_output
+
+def do_git_commit(gpt_output):
+    gpt_output = gpt_output.split('\n')[0]
+    if gpt_output[0] != '"':
+        gpt_output = f'"{gpt_output}"'
+    cmd = f'git commit -m {gpt_output}'
+    exec_bash_cmd(cmd)
+
+def print_help_text():
+    helptext = """
+Usage: goc <mode> <args>
+
+Modes:
+  diff <args>      Generate documentation for the git diff between commits or files.
+  commit           Generate a commit message for the current git diff.
+
+Options:
+  help             Show this help text.
+
+"""
+    print(helptext)
 
 def goc():
     n_args = len(sys.argv) - 1
     if n_args == 0:
-        # compare the latest 2 commits
-        prompt_chain = document_latest_commit()
+        print('No Arguments, Please run "goc <mode> <args>"')
     elif n_args > 0:
-        # just pass the args directly into git diff
-        prompt_chain = document_git_diff_wrap(sys.argv[1:])
+        mode = sys.argv[1]
+        if mode == 'help':
+            print_help_text()
+            return
+        if mode == 'diff':
+            # just pass the args directly into git diff
+            prompt_chain = document_git_diff_wrap(sys.argv[2:])
+        elif mode == 'commit':
+            # get description of the current diff
+            prompt_chain = git_commit_wrap()
+
     resp = execute_prompt_chain(prompt_chain)
-    md_output = parse_gpt_resp(resp)
-    print(md_output)
+    gpt_output = parse_gpt_resp(resp)
+    if mode == 'diff':
+        print(gpt_output)
+    elif mode == 'commit':
+        print('Committing with message: ' + gpt_output)
+        do_git_commit(gpt_output)
 
 
 if __name__ == '__main__':
     goc()
```

### Comparing `goc-0.3.0/PKG-INFO` & `goc-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goc
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/djentleman/goc
 Author: Todd Perry
 Author-email: toddperry171@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

