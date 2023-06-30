# Comparing `tmp/llvd-3.0.3.tar.gz` & `tmp/llvd-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvd-3.0.3.tar", last modified: Thu Dec 15 13:05:09 2022, max compression
+gzip compressed data, was "llvd-3.0.4.tar", last modified: Fri Jun 30 12:30:41 2023, max compression
```

## Comparing `llvd-3.0.3.tar` & `llvd-3.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:05:09.022583 llvd-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-15 13:04:53.000000 llvd-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2022-12-15 13:05:09.022583 llvd-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2022-12-15 13:04:53.000000 llvd-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:05:09.022583 llvd-3.0.3/llvd/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/process_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2022-12-15 13:04:53.000000 llvd-3.0.3/llvd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:05:09.022583 llvd-3.0.3/llvd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-15 13:05:09.000000 llvd-3.0.3/llvd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 13:05:09.022583 llvd-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2022-12-15 13:04:53.000000 llvd-3.0.3/setup.py
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.429427 llvd-3.0.4/
+-rw-r--r--   0 df-4       (501) staff       (20)     1093 2023-03-16 10:32:53.000000 llvd-3.0.4/LICENSE
+-rw-r--r--   0 df-4       (501) staff       (20)     5316 2023-06-30 12:30:41.429313 llvd-3.0.4/PKG-INFO
+-rw-r--r--   0 df-4       (501) staff       (20)     4766 2023-03-16 10:32:53.000000 llvd-3.0.4/README.md
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.428517 llvd-3.0.4/llvd/
+-rwxr-xr-x   0 df-4       (501) staff       (20)       90 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/__init__.py
+-rw-r--r--   0 df-4       (501) staff       (20)    13880 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/app.py
+-rw-r--r--   0 df-4       (501) staff       (20)     3200 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/cli.py
+-rw-r--r--   0 df-4       (501) staff       (20)      555 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/config.py
+-rw-r--r--   0 df-4       (501) staff       (20)     3572 2023-06-30 12:29:51.000000 llvd-3.0.4/llvd/downloader.py
+-rw-r--r--   0 df-4       (501) staff       (20)      136 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/exceptions.py
+-rw-r--r--   0 df-4       (501) staff       (20)      642 2023-06-30 12:07:01.000000 llvd-3.0.4/llvd/process_io.py
+-rw-r--r--   0 df-4       (501) staff       (20)     1601 2023-03-16 10:32:53.000000 llvd-3.0.4/llvd/utils.py
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-06-30 12:30:41.429160 llvd-3.0.4/llvd.egg-info/
+-rw-r--r--   0 df-4       (501) staff       (20)     5316 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/PKG-INFO
+-rw-r--r--   0 df-4       (501) staff       (20)      323 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/SOURCES.txt
+-rw-r--r--   0 df-4       (501) staff       (20)        1 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/dependency_links.txt
+-rw-r--r--   0 df-4       (501) staff       (20)       39 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/entry_points.txt
+-rw-r--r--   0 df-4       (501) staff       (20)      166 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/requires.txt
+-rw-r--r--   0 df-4       (501) staff       (20)        5 2023-06-30 12:30:41.000000 llvd-3.0.4/llvd.egg-info/top_level.txt
+-rw-r--r--   0 df-4       (501) staff       (20)       38 2023-06-30 12:30:41.429467 llvd-3.0.4/setup.cfg
+-rw-r--r--   0 df-4       (501) staff       (20)     1269 2023-03-16 10:32:53.000000 llvd-3.0.4/setup.py
```

### Comparing `llvd-3.0.3/LICENSE` & `llvd-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/PKG-INFO` & `llvd-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.3
+Version: 3.0.4
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
+License: UNKNOWN
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -183,7 +184,9 @@
     <img src="https://raw.githubusercontent.com/knowbee/hosting/master/assets/progress_llvd.png" width="auto" height="auto"/>
 </p>
 
 <a name="author"/>
 
 # Author
 Igwaneza Bruce
+
+
```

### Comparing `llvd-3.0.3/README.md` & `llvd-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/llvd/app.py` & `llvd-3.0.4/llvd/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from requests import Session
 from llvd import config
 from llvd.exceptions import EmptyCourseList
 from llvd.downloader import download_subtitles, download_video, download_exercises
 from click_spinner import spinner
 import re
 from llvd.utils import clean_name
-import traceback
 import click
 import sys
 from llvd import config
+import subprocess
 class App:
     def __init__(
         self, email, password, course_slug, resolution, caption, exercise, throttle
     ):
         self.email = email
         self.password = password
         self.course_slug = course_slug[0]
@@ -50,37 +50,43 @@
                 if cookies.get("li_at") == None:
                     return None
                 return 200
 
         except ConnectionResetError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionResetError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
 
         except requests.exceptions.ConnectionError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
 
     def run(self, cookies=None):
         """
         Main function, tries to login the user and when it succeeds, tries to download the course
         """
         try:
 
             if cookies is not None:
                 self.cookies["JSESSIONID"] = cookies.get("JSESSIONID")
                 self.cookies["li_at"] = cookies.get("li_at")
                 self.headers["Csrf-Token"] = cookies.get("JSESSIONID")
+                
+                # remove empty files
+                command = 'find . -depth -type f -size 0 -exec rm {} +'
+                subprocess.run(command, shell=True)
+
+                # proceed to download
                 self.download()
             else:
                 with Session() as session:
                     site = session.get(config.login_url)
                     bs_content = bs(site.content, "html.parser")
 
                     csrf = bs_content.find("input", {"name": "csrfToken"}).get("value")
@@ -102,15 +108,15 @@
                         )
                         sys.exit(0)
                     else:
                         self.create_course_dirs(self.course_slug)
                         self.download()
 
         except ConnectionError:
-            click.echo(click.style(f"Failed to connect", fg="red"))
+            click.echo(click.style(f"ConnectionError: Failed to connect", fg="red"))
 
     @staticmethod
     def create_course_dirs(course_slug):
         """
         Create file system path for courses
         """
         if not os.path.exists(f"{course_slug}"):
@@ -136,34 +142,35 @@
         PATH = "path"
         try:
             if self.course_type == PATH:
                 self.download_courses_from_path()
             else:
                 self.download_entire_course()
         except TypeError as e:
-            print(e)
-            click.echo(
-                click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
-                    fg="red",
-                )
-            )
+            print("retrying...")
+            self.download_entire_course()
+            # click.echo(
+            #     click.style(
+            #         f"TypeError: {e}\n",
+            #         fg="red",
+            #     )
+            # )
 
         except ConnectionResetError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionResetError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
 
         except requests.exceptions.ConnectionError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
 
     def download_courses_from_path(self):
 
         try:
@@ -190,15 +197,15 @@
                     f"\nDownloading course {index+1}/{total_courses}: {course_token}"
                 )
                 self.course_slug = course_token
                 self.create_course_dirs(course_token)
                 self.download_entire_course(skip_done_alert=suppress)
 
         except EmptyCourseList as e:
-            click.echo(click.style(f"Error parsing learning path.\n{e}", fg="red"))
+            click.echo(click.style(f"EmptyCourseList: Error parsing learning path.\n{e}", fg="red"))
 
         except Exception as e:
             click.echo(
                 click.style(
                     f"Error fetching courses from learning path!\n{e}", fg="red"
                 )
             )
@@ -232,16 +239,25 @@
         video_index = 1
         self.chapter_path = (
             f"./{self.course_slug}/{chapters_index_padded}. {clean_name(chapter_name)}"
         )
         if not os.path.exists(chapter_path):
             os.makedirs(chapter_path)
 
+        current_files = []
+        for file in os.listdir(chapter_path):
+            if file.endswith(".mp4") and ". " in file:
+                ff = re.split("\d+\. ", file)[1].replace(".mp4", "")
+                current_files.append(ff)
+
+        # unique videos by checking if the video name is in the current files
+        videos = [video for video in videos if clean_name(video["title"]) not in current_files]
+
         for video in videos:
-            self.current_video_index = video_index
+            self.current_video_index = video_index + len(current_files)
             page_json, video_name = self.fetch_video(video)
 
             try:
                 download_url = page_json["elements"][0]["selectedVideo"]["url"][
                     "progressiveUrl"
                 ]
                 try:
@@ -253,50 +269,42 @@
                     int(page_json["elements"][0]["selectedVideo"]["durationInSeconds"])
                     * 1000
                 )
 
                 click.echo(
                     click.style(
                         f"\nCurrent: {chapters_index_padded}. {clean_name(chapter_name)}/"
-                        f"{video_index:0=2d}. {video_name}.mp4 @{self.video_format}p"
+                        f"{video_index + len(current_files):0=2d}. {video_name}.mp4 @{self.video_format}p"
                     )
                 )
-                current_files = []
-                for file in os.listdir(chapter_path):
-                    if file.endswith(".mp4") and ". " in file:
-                        ff = re.split("\d+\. ", file)[1].replace(".mp4", "")
-                        current_files.append(ff)
             except Exception as e:
                 if "url" in str(e):
                     click.echo(
                         click.style(
                             f"This video is locked, you probably "
                             f"need a premium account",
                             fg="red",
                         )
                     )
                 else:
                     click.echo(
                         click.style(f"Failed to download {video_name}", fg="red")
                     )
             finally:
-                if clean_name(video_name) not in current_files:
-                    download_video(
-                        download_url,
-                        video_index,
-                        video_name,
-                        chapter_path,
-                        delay,
-                    )
-                else:
-                    click.echo(f"Skipping already existing video...")
+                download_video(
+                    download_url,
+                    self.current_video_index,
+                    video_name,
+                    chapter_path,
+                    delay,
+                )
                 if subtitles is not None and self.caption:
                     subtitle_lines = subtitles["lines"]
                     download_subtitles(
-                        video_index,
+                        self.current_video_index,
                         subtitle_lines,
                         video_name,
                         chapter_path,
                         duration_in_ms,
                     )
             video_index += 1
 
@@ -342,43 +350,34 @@
             if kwargs.get("skip_done_alert"):
                 return
             click.echo(
                 "\nYour download is complete. Begin your learning journey now.! :)"
             )
 
         except requests.exceptions.TooManyRedirects:
-            click.echo(click.style(f"Your cookie is expired", fg="red"))
-        except KeyError:
-            click.echo(click.style(f"That course is not found", fg="red"))
-
-        except TypeError:
-            click.echo(
-                click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
-                    fg="red",
-                )
-            )
+            click.echo(click.style(f"TooManyRedirects: Your cookie is expired", fg="red"))
+        except KeyError as e:
+            click.echo(click.style(f"KeyError: That course is not found {e}", fg="red"))
 
         except ConnectionResetError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionResetError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
 
         except requests.exceptions.ConnectionError:
             click.echo(
                 click.style(
-                    f"There is a connection error. Please check your connectivity.\n",
+                    f"ConnectionError: There is a connection error. Please check your connectivity.\n",
                     fg="red",
                 )
             )
         except Exception as e:
             if os.path.exists(
                 f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
             ):
                 os.remove(
                     f"{self.chapter_path}/{self.current_video_index:0=2d}. {clean_name(self.current_video_name)}.mp4"
                 )
-            traceback.print_exc()
             self.download_entire_course()
```

### Comparing `llvd-3.0.3/llvd/cli.py` & `llvd-3.0.4/llvd/cli.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/llvd/config.py` & `llvd-3.0.4/llvd/config.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/llvd/downloader.py` & `llvd-3.0.4/llvd/downloader.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,18 @@
     """
     if delay:
         throttle(delay)
     maximum_retries = 5
     with open(f"{path}/{index:0=2d}. {clean_name(filename)}.mp4", "wb") as f:
         download_size = 0
         while maximum_retries > 0:
-            requests.adapters.HTTPAdapter(max_retries=maximum_retries)
-            response = requests.get(
+            adapter = requests.adapters.HTTPAdapter(max_retries=maximum_retries)
+            session = requests.Session()
+            session.mount(url, adapter)
+            response = session.get(
                 url,
                 stream=True,
                 headers={"Accept-Encoding": None, "Content-Encoding": "gzip"},
             )
             download_size = response.headers.get("content-length")
             if download_size is None and maximum_retries > 0:
                 maximum_retries -= 1
@@ -39,27 +41,25 @@
         for chunk in response.iter_content(chunk_size=1024):
             if chunk:
                 f.write(chunk)
                 pbar.set_description("Downloading video... ")
                 pbar.update(len(chunk))
         pbar.close()
 
-
 def download_subtitles(index, subs, video_name, path, video_duration):
     """Write to a file (subtitle file) caption matching the right time."""
     with open(f"{path}/{index:0=2d}. {clean_name(video_name).strip()}.srt", "wb") as f:
         click.echo("Downloading subtitles..")
         for i, sub in enumerate(subs, start=1):
             starts_at = sub["transcriptStartAt"]
             ends_at = subs[i]["transcriptStartAt"] if i < len(subs) else video_duration
             caption = sub["caption"]
             line = f"{i}\n{subtitles_time_format(starts_at)} --> {subtitles_time_format(ends_at)}\n{caption}\n\n"
             f.write(line.encode("utf8"))
 
-
 def download_exercises(links, path):
     """Download exercises."""
     for link in links:
         filename = re.split("exercises/(.+).zip", link)[1]
         filepath = f"{path}/{clean_name(filename)}.zip"
         with open(filepath, "wb") as f:
             # Set up the request
@@ -92,8 +92,8 @@
                     f.write(chunk)
                     if pbar:
                         pbar.update(len(chunk))
 
             # Close the progress bar
             if pbar:
                 pbar.close()
-            print("\n")
+            print("\n")
```

### Comparing `llvd-3.0.3/llvd/process_io.py` & `llvd-3.0.4/llvd/process_io.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/llvd/utils.py` & `llvd-3.0.4/llvd/utils.py`

 * *Files identical despite different names*

### Comparing `llvd-3.0.3/llvd.egg-info/PKG-INFO` & `llvd-3.0.4/llvd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: llvd
-Version: 3.0.3
+Version: 3.0.4
 Summary: Linkedin Learning Video Downloader CLI Tool
 Home-page: https://github.com/knowbee/llvd.git
 Author: Igwaneza Bruce
 Author-email: knowbeeinc@gmail.com
+License: UNKNOWN
 Platform: any
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -183,7 +184,9 @@
     <img src="https://raw.githubusercontent.com/knowbee/hosting/master/assets/progress_llvd.png" width="auto" height="auto"/>
 </p>
 
 <a name="author"/>
 
 # Author
 Igwaneza Bruce
+
+
```

### Comparing `llvd-3.0.3/setup.py` & `llvd-3.0.4/setup.py`

 * *Files identical despite different names*

