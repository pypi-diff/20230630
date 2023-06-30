# Comparing `tmp/trilium_py-0.7.6-py3-none-any.whl.zip` & `tmp/trilium_py-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27592 bytes, number of entries: 12
+Zip file size: 27780 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
--rw-r--r--  2.0 unx    31298 b- defN 23-Jun-16 08:33 trilium_py/client.py
+-rw-r--r--  2.0 unx    32257 b- defN 23-Jun-30 07:11 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    11024 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/RECORD
-12 files, 88749 bytes uncompressed, 25922 bytes compressed:  70.8%
+-rwxrwx---  2.0 unx    35184 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    11046 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-30 07:22 trilium_py-0.8.0.dist-info/RECORD
+12 files, 89730 bytes uncompressed, 26110 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.7.6.dist-info/LICENSE.txt
+Filename: trilium_py-0.8.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.7.6.dist-info/METADATA
+Filename: trilium_py-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.7.6.dist-info/WHEEL
+Filename: trilium_py-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.7.6.dist-info/top_level.txt
+Filename: trilium_py-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.7.6.dist-info/RECORD
+Filename: trilium_py-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -2,14 +2,15 @@
 import re
 import urllib.parse
 
 import magic
 import markdown2
 import requests
 from bs4 import BeautifulSoup
+from loguru import logger
 from natsort import natsort
 
 from .utils.markdown_math import sanitizeInput, reconstructMath
 from .utils.param_util import format_query_string, clean_param
 from .utils.time_util import get_yesterday, get_today
 
 
@@ -33,15 +34,15 @@
         data = {'password': password}
 
         res = requests.post(url, data=data)
         if res.status_code == 201:
             self.token = res.json()['authToken']
             return self.token
         else:
-            print(res.json()['message'])
+            logger.info(res.json()['message'])
             return None
 
     def logout(self, token_to_destroy: str = None) -> bool:
         """
         destroy token
         """
 
@@ -53,15 +54,15 @@
 
         url = f'{self.server_url}/etapi/auth/logout'
         headers = {
             'Authorization': token_to_destroy,
         }
         res = requests.post(url, headers=headers)
         if res.status_code == 204:
-            print('logout successfully')
+            logger.info('logout successfully')
             return True
         return False
 
     def app_info(self) -> dict:
         """
 
         :return:
@@ -130,51 +131,41 @@
             "noteId": noteId,
             "branchId": branchId
         }
         res = requests.post(url, json=clean_param(params), headers=self.get_header())
 
         return res.json()
 
-    def create_file_note(self, parentNoteId: str, title: str, file_data: str, content_file: str,
-                         type: str = 'file', mime: str = None,
-                         content=None, notePosition: int = None, prefix: str = None,
+    def create_file_note(self, parentNoteId: str, title: str, file_path: str,
+                         type: str = 'file', mime: str = "application/octet-stream",
+                         content='<p></p>', notePosition: int = None, prefix: str = None,
                          isExpanded: str = None, noteId: str = None,
                          branchId: str = None):
         '''
+        Upload ordinary file as a sub-note
+
         Create a note
         set file name attribute
-        Update its content with image binary content
+        Update its content with raw file binary content
         :param parentNoteId:
         :param title:
-        :param file_data: file object from buffer.
-        :param content_file: file path in file system.
+        :param file_path: file path in file system.
         :param type:
         :param mime:
         :param content:
         :param notePosition:
         :param prefix:
         :param isExpanded:
         :param noteId:
         :param branchId:
         :return:
         '''
 
         url = f'{self.server_url}/etapi/create-note'
 
-        if not mime:
-            # if mime not specified, get mime info by python-magic package
-            if file_data:
-                mime = magic.from_buffer(file_data, mime=True)
-            elif content_file:
-                mime = magic.from_file(file_data, mime=True)
-
-        if not mime:
-            # just in case python-magic not working, give a default mime
-            mime = "image/png"
-
         params = {
             "parentNoteId": parentNoteId,
             "title": title,
             "type": type,
             "mime": mime,
             "content": content,
             "notePosition": notePosition,
@@ -186,26 +177,22 @@
 
         res_file = requests.post(url, json=clean_param(params),
                                  headers={'content-type': 'application/json', 'Authorization': self.token, })
         res_file_json = res_file.json()
         new_noteId = res_file_json['note']['noteId']
 
         # set file name
-        content_file_name = os.path.basename(content_file)
+        file_path_name = os.path.basename(file_path)
         self.create_attribute(attributeId=None, noteId=new_noteId, type='label', name='originalFileName',
-                              value=content_file_name, isInheritable=False)
+                              value=file_path_name, isInheritable=False)
 
         # upload file, set note content
         url = f'{self.server_url}/etapi/notes/{new_noteId}/content'
-        # content-type here will affect the result
-        # not working, encoding issue? automated force encoding to utf-8 and lost data
-        if not file_data:
-            file_data = open(content_file, 'rb').read()
+        file_data = open(file_path, 'rb').read()
         res = requests.put(url, data=file_data,
-                           # headers={'content-type': 'text/plain', 'Authorization': self.token, })
                            headers={
                                'content-type': 'application/octet-stream',
                                'Content-Transfer-Encoding': 'binary',
                                'Authorization': self.token,
                            })
         if res.status_code == 204:
             return res_file_json
@@ -214,14 +201,16 @@
     def create_image_note(self, parentNoteId: str, title: str, image_file: str, type: str = 'image', mime: str = None,
                           content=None,
                           notePosition: int = None, prefix: str = None,
                           isExpanded: str = None, noteId: str = None,
                           branchId: str = None):
 
         '''
+        Upload image as a sub-note
+
         Create a note
         set file name attribute
         Update its content with image binary content
 
         :param parentNoteId:
         :param title:
         :param image_file:
@@ -434,15 +423,15 @@
             format = 'markdown'
         else:
             format = 'html'
         params = {
             "format": format,
         }
         r = requests.get(url, params=clean_param(params), headers=self.get_header())
-        print(r.status_code)
+        logger.info(r.status_code)
         with open(savePath, 'wb') as fd:
             for chunk in r.iter_content(chunk_size=chunk_size):
                 fd.write(chunk)
         return True
 
     def get_today_note_content(self):
         date = get_today()
@@ -540,15 +529,15 @@
 
             if "todo-list__label" in todo_description:
                 todo_item_html = f'''<li>{todo_description}</li>'''
             else:
                 todo_item_html = f'''<li><label class="todo-list__label"><input disabled="disabled" type="checkbox"/ > <span class = "todo-list__label__description">{todo_description}</span></label></li>'''
 
             if not todo_labels:
-                print('new empty page')
+                logger.info('new empty page')
                 todo_item_html = f'''<p>TODO:</p><ul class="todo-list">{todo_item_html}</ul>'''
                 todo_item = BeautifulSoup(todo_item_html, 'html.parser')
                 soup.insert(0, todo_item)
             else:
                 last_todo_label = todo_labels[-1]
                 if not last_todo_label.text.strip():
                     # replace last empty todo item
@@ -565,15 +554,15 @@
             # free mem
             soup.decompose()
             del soup
 
             return self.set_today_note_content(new_content)
 
         except Exception as e:
-            print(e)
+            logger.info(e)
             return False
 
     def update_todo(self, todo_index, todo_description):
         """update a todo item description"""
         todo_description = todo_description.strip()
         content = self.get_today_note_content()
         soup = BeautifulSoup(content, 'html.parser')
@@ -669,66 +658,56 @@
             self.delete_yesterday_todo(i)
 
     def upload_md_file(self, file: str, parentNoteId: str):
         md_file = os.path.abspath(file).replace('\\', '/').replace('//', '/')
         md_full_name = os.path.basename(md_file)
         md_name = md_full_name[:-3]
         md_folder = os.path.dirname(md_file)
-        print(md_file)
-        # print(md_name)
-        # print(md_folder)
+        logger.info(md_file)
+        # logger.info(md_name)
+        # logger.info(md_folder)
 
         # convert md to html
         with open(md_file, 'r', encoding='utf-8') as f:
             content = f.read()
 
             # fix logseq image size format
             logseq_image_pat = r'(\!\[.*\]\(.*\))\{.*?:height.*width.*}'
             content = re.sub(logseq_image_pat, r'\1', content)
 
             if not re.search(re.escape("$"), content):
                 # extra format support
                 # https://github.com/trentm/python-markdown2/wiki/Extras
                 html = markdown2.markdown(content, extras=['fenced-code-blocks', 'strike', 'tables', 'task_list'])
-                # print(html)
+                # logger.info(html)
             else:
                 no_latex_part, latex_code_part = sanitizeInput(content)
                 html = reconstructMath(markdown2.markdown(no_latex_part,
                                                           extras=['fenced-code-blocks', 'strike', 'tables',
                                                                   'task_list']),
                                        latex_code_part)
+        note_id = ''
 
         # detect images
         pat = '<img (.*?) />'
         images = re.findall(pat, html)
 
-        if not images:
-            res = self.create_note(
-                parentNoteId=parentNoteId,
-                title=md_name,
-                type="text",
-                content=html,
-            )
+        res = self.create_note(
+            parentNoteId=parentNoteId,
+            title=md_name,
+            type="text",
+            content=html,
+        )
+        note_id = res['note']['noteId']
+        # logger.info(note_id)
 
-        else:
+        if images:
             # images require manually upload and url need to be replaced
-            print('found images:')
-            print(images)
-
-            # create empty note, replace it later
-            res = self.create_note(
-                parentNoteId=parentNoteId,
-                title=md_name,
-                type="text",
-                content='importing...',
-            )
-            # print(res)
-
-            note_id = res['note']['noteId']
-            # print(note_id)
+            logger.info('found images:')
+            logger.info(images)
 
             # process images
             for match in images:
                 # extract image url and name
                 image_names = re.findall('alt="(.*?)"', match)
                 image_paths = re.findall('src="(.*?)"', match)
 
@@ -769,76 +748,124 @@
                     image_name = os.path.basename(image_path)
 
                 res = self.create_image_note(
                     parentNoteId=note_id,
                     title=image_name,
                     image_file=image_file_path,
                 )
-                # print(res)
+                # logger.info(res)
                 image_note_id = res['note']['noteId']
                 # fix path with `/` in it, the param should be quoted. e.g. relative url from obsidian
                 image_url = f"api/images/{image_note_id}/{urllib.parse.quote(res['note']['title'], safe='')}"
-                print(image_url)
+                logger.info(image_url)
 
                 html = html.replace(image_path, image_url)
 
                 # add relation for image
                 self.create_attribute(attributeId=None, noteId=note_id, type='relation', name='imageLink',
                                       value=image_note_id, isInheritable=False)
 
             # replace note content
             res = self.update_note_content(note_id, html)
-            # print(res)
+            # logger.info(res)
+
+        # detect files
+        pat = '<a href="(.*?)">(.*)</a>'
+        a_links = re.findall(pat, html)
+        logger.info(a_links)
+        for link, link_name in a_links:
+
+            # fix file path
+            file_path = ''
+            if link.startswith(('http:', 'https:')):
+                # skip online link
+                continue
+            if os.path.exists(link):
+                # absolute file path
+                file_path = link
+            else:
+                file_path = os.path.join(md_folder, link).replace('\\', '/')
+                # unquote path, incase the url is quoted
+                file_path_unquote = urllib.parse.unquote(file_path)
+
+                # skip if path does not point to a valid file
+                if os.path.isdir(file_path) or os.path.isdir(file_path_unquote):
+                    continue
+
+                # try both raw path and unquoted path
+                if os.path.exists(file_path_unquote):
+                    file_path = file_path_unquote
+
+            # upload file
+            if os.path.exists(file_path):
+                logger.info(file_path)
+
+                res = self.create_file_note(
+                    parentNoteId=note_id,
+                    title=link_name,
+                    file_path=file_path,
+                )
+                logger.info(res)
+
+                # update file link
+                file_note_id = res['note']['noteId']
+                # fix path with `/` in it, the param should be quoted. e.g. relative url from obsidian
+                file_url = f"#root/{note_id}/{file_note_id}"
+
+                html = html.replace(link, file_url)
+
+            # replace note content
+            res = self.update_note_content(note_id, html)
 
-            return res
+        return res
 
     def upload_md_folder(self, parentNoteId: str, mdFolder: str, includePattern=[],
                          ignoreFolder=[], ignoreFile=[]):
         if not includePattern:
             includePattern = ['.md', ]
 
         # note tree
         # record for noteId
         note_tree = {'.': parentNoteId}
-        print(mdFolder)
+        logger.info(mdFolder)
 
         mdFolder = os.path.expandvars(os.path.expanduser(mdFolder))
 
         for root, dirs, files in os.walk(mdFolder, topdown=True):
             root_folder_name = os.path.basename(root)
 
             rel_path = os.path.relpath(root, start=mdFolder)
             if any(x in rel_path for x in ignoreFolder):
                 continue
 
-            print('==============')
-            print(f'root {root}')
-            print(f'root_folder_name {root_folder_name}')
-            print(f'rel_path {rel_path}')
+            logger.info('==============')
+            logger.info(f'root {root}')
+            logger.info(f'root_folder_name {root_folder_name}')
+            logger.info(f'rel_path {rel_path}')
 
             current_parent_note_id = note_tree[rel_path]
 
-            print(f'files')
+            logger.info(f'files')
             for name in natsort.natsorted(files):
                 # only include markdown files
                 if any(x == name for x in ignoreFile):
                     continue
 
                 if any(x in name for x in includePattern):
                     file_path = os.path.join(root, name)
-                    print(file_path)
+                    logger.info(file_path)
                     self.upload_md_file(file=file_path, parentNoteId=current_parent_note_id)
 
-            print(f'dirs')
+            logger.info(f'dirs')
             for name in natsort.natsorted(dirs):
                 if all(x not in name for x in ignoreFolder):
                     dir_path = os.path.join(root, name)
-                    print(dir_path)
+                    logger.info(dir_path)
                     rel_path = os.path.relpath(dir_path, start=mdFolder)
-                    print(rel_path)
+                    logger.info(rel_path)
                     res = self.create_note(
                         parentNoteId=current_parent_note_id,
                         title=name,
                         type="text",
                         content=name,
                     )
                     res['note']['noteId']
@@ -847,10 +874,10 @@
         return True
 
     def backup(self, backup_name):
         url = f'{self.server_url}/etapi/backup/{backup_name}'
 
         res = requests.put(url, headers=self.get_header())
         if res.status_code == 204:
-            print('backup successfully')
+            logger.info('backup successfully')
             return True
         return False
```

## Comparing `trilium_py-0.7.6.dist-info/LICENSE.txt` & `trilium_py-0.8.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.7.6.dist-info/METADATA` & `trilium_py-0.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.7.6
+Version: 0.8.0
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -25,14 +25,15 @@
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: BeautifulSoup4
 Requires-Dist: requests
 Requires-Dist: markdown2[all]
 Requires-Dist: natsort
+Requires-Dist: loguru
 Requires-Dist: python-magic-bin ; platform_system == "Windows"
 Requires-Dist: python-magic ; sys_platform == "darwin"
 Requires-Dist: python-magic ; sys_platform == "linux"
 
 # 🐍 trilium-py
 
 Python client for ETAPI of Trilium Note.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.7.6 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.8.0 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -11,27 +11,27 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.6, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: BeautifulSoup4 Requires-Dist: requests
-Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: python-
-magic-bin ; platform_system == "Windows" Requires-Dist: python-magic ;
-sys_platform == "darwin" Requires-Dist: python-magic ; sys_platform == "linux"
-# ð trilium-py Python client for ETAPI of Trilium Note. [![Downloads](https:
-//static.pepy.tech/badge/trilium-py)](https://pepy.tech/project/trilium-py) [!
-[Supported Versions](https://img.shields.io/pypi/pyversions/trilium-py.svg)]
-(https://pypi.org/project/trilium-py) [![Supported Versions](https://
-img.shields.io/pypi/v/trilium-py?color=%2334D058&label=pypi%20package)](https:/
-/pypi.org/project/trilium-py) [![PyPI license](https://img.shields.io/pypi/l/
-trilium-py.svg)](https://pypi.python.org/pypi/trilium-py/) [![Maintenance]
-(https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
-Naereen/StrapDown.js/graphs/commit-activity) [https://moe-counter--
-nriver1.repl.co/get/@Nriver_trilium-py]
+Requires-Dist: markdown2[all] Requires-Dist: natsort Requires-Dist: loguru
+Requires-Dist: python-magic-bin ; platform_system == "Windows" Requires-Dist:
+python-magic ; sys_platform == "darwin" Requires-Dist: python-magic ;
+sys_platform == "linux" # ð trilium-py Python client for ETAPI of Trilium
+Note. [![Downloads](https://static.pepy.tech/badge/trilium-py)](https://
+pepy.tech/project/trilium-py) [![Supported Versions](https://img.shields.io/
+pypi/pyversions/trilium-py.svg)](https://pypi.org/project/trilium-py) [!
+[Supported Versions](https://img.shields.io/pypi/v/trilium-
+py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/trilium-py)
+[![PyPI license](https://img.shields.io/pypi/l/trilium-py.svg)](https://
+pypi.python.org/pypi/trilium-py/) [![Maintenance](https://img.shields.io/badge/
+Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/
+commit-activity) [https://moe-counter--nriver1.repl.co/get/@Nriver_trilium-py]
 # ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
 Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
 (Basic) Usage](#-basic-usage) - [ð Initialization](#-initialization) - [ð
 Application Information](#-application-information) - [ð Search note](#-
 search-note) - [ð­ Create Note](#-create-note) - [ð¼ï¸ Create Image note]
 (#ï¸-create-image-note) - [ð Get note](#-get-note) - [ð Update note](#-
 update-note) - [ðï¸ Delete note](#ï¸-delete-note) - [ð Day note](#-day-
```

## Comparing `trilium_py-0.7.6.dist-info/RECORD` & `trilium_py-0.8.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=Tb7_ozH_C5AWNINpmZyj2klxCfuutyNDZagf5pI2hGA,31298
+trilium_py/client.py,sha256=d9hwU4cq9fQdt2AvLxKZgYC4khvY8YIm8IG6Pmru6s0,32257
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/markdown_math.py,sha256=ORQwEXAPtcf2-NaYKx4Pr5q5B8CtupVRYt04JD-c3EY,8656
 trilium_py/utils/param_util.py,sha256=BOiblP1F-jMgggx8L_QxCH3s8-FIdG1kAM-4ykSbZ5E,675
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=U1Qn5UFzQO-Bi9DGjq2OEiVzCi6x5KXsyRKF-AOJV64,470
-trilium_py-0.7.6.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.7.6.dist-info/METADATA,sha256=rsBP9AAbt2thtfHGK75duLbVWSzCM8Gusxtnwes6_lQ,11024
-trilium_py-0.7.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-trilium_py-0.7.6.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.7.6.dist-info/RECORD,,
+trilium_py-0.8.0.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.8.0.dist-info/METADATA,sha256=wtdiVdt8ZaV54bvZxJ5TMoyjGt4A8LdJxETkESBC184,11046
+trilium_py-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+trilium_py-0.8.0.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.8.0.dist-info/RECORD,,
```

