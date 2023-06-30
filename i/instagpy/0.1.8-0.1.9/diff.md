# Comparing `tmp/instagpy-0.1.8.tar.gz` & `tmp/instagpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.8.tar", last modified: Thu Jun 22 07:19:41 2023, max compression
+gzip compressed data, was "instagpy-0.1.9.tar", last modified: Fri Jun 30 10:30:15 2023, max compression
```

## Comparing `instagpy-0.1.8.tar` & `instagpy-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.859039 instagpy-0.1.8/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3572 2023-06-22 07:19:41.859039 instagpy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-06-22 07:00:19.000000 instagpy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.843408 instagpy-0.1.8/instagpy/
--rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.8/instagpy/__init__.py
--rw-rw-rw-   0        0        0      974 2023-06-22 07:17:43.000000 instagpy-0.1.8/instagpy/config.py
--rw-rw-rw-   0        0        0    24516 2023-06-22 06:11:52.000000 instagpy-0.1.8/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2140 2023-06-14 13:31:23.000000 instagpy-0.1.8/instagpy/path.py
--rw-rw-rw-   0        0        0     1421 2023-06-21 13:28:30.000000 instagpy-0.1.8/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.8/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2914 2023-06-14 09:37:23.000000 instagpy-0.1.8/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:19:41.859039 instagpy-0.1.8/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3572 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 07:19:41.000000 instagpy-0.1.8/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:19:41.859039 instagpy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-06-22 07:19:09.000000 instagpy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:30:15.655834 instagpy-0.1.9/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3572 2023-06-30 10:30:15.655834 instagpy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-06-22 07:00:19.000000 instagpy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 10:30:15.640207 instagpy-0.1.9/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-06-07 10:27:42.000000 instagpy-0.1.9/instagpy/__init__.py
+-rw-rw-rw-   0        0        0      974 2023-06-30 10:26:36.000000 instagpy-0.1.9/instagpy/config.py
+-rw-rw-rw-   0        0        0    25211 2023-06-30 10:26:01.000000 instagpy-0.1.9/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2140 2023-06-14 13:31:23.000000 instagpy-0.1.9/instagpy/path.py
+-rw-rw-rw-   0        0        0     1421 2023-06-21 13:28:30.000000 instagpy-0.1.9/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2729 2023-06-07 14:13:48.000000 instagpy-0.1.9/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2914 2023-06-26 16:39:13.000000 instagpy-0.1.9/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 10:30:15.640207 instagpy-0.1.9/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3572 2023-06-30 10:30:15.000000 instagpy-0.1.9/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-06-30 10:30:15.000000 instagpy-0.1.9/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 10:30:15.000000 instagpy-0.1.9/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-30 10:30:15.000000 instagpy-0.1.9/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-30 10:30:15.000000 instagpy-0.1.9/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 10:30:15.655834 instagpy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-30 10:30:04.000000 instagpy-0.1.9/setup.py
```

### Comparing `instagpy-0.1.8/LICENSE` & `instagpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/PKG-INFO` & `instagpy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.8 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.9 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.8/README.md` & `instagpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy/config.py` & `instagpy-0.1.9/instagpy/config.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy/instagpy.py` & `instagpy-0.1.9/instagpy/instagpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             self.session.proxies = config.PROXY
             self.session.verify = False
         self.session.headers.update(
             {"User-Agent": random.choice(config._USER_AGENTS)})
         make_request(path.BASE_URL, session=self.session)
         response = requests.get(path.LOGIN_URL)
         if not response.cookies:
-            for _ in range(self.max_retries):
+            for _ in range(config.MAX_RETRIES):
                 response = self.session.get(path.LOGIN_URL)
                 if response.cookies:
                     break
         csrf_token = dict(response.cookies)["csrftoken"]
         self.session.headers.update(
             {'x-csrftoken': csrf_token, 'X-Requested-With': "XMLHttpRequest", 'Referer': path.BASE_URL})
         self.session.cookies = response.cookies
@@ -299,27 +299,34 @@
         user['media_count'] = user_info['edge_owner_to_timeline_media']['count']
         user['website'] = user_info['external_url']
         if print_formatted:
             for key, value in user.items():
                 print(f"{key} : {value}")
         return user
 
-    def get_user_friends(self, username, followers_list=False, followings_list=False, end_cursor=None, max=None):
+    def get_user_friends(self, username, followers_list=False, followings_list=False, end_cursor=None, total=None):
         """Fetch follower or following list of a user.
 
         Args:
             username (str): Instagram Username.
             followers_list (bool, optional): Set True if want to extract user's followers list. Defaults to False.
             followings_list (bool, optional): Set True if want to extract user's followings list. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
-            max (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
+            total (int, optional): Total number of results to extract. Defaults to None. -- Gets all by default.
 
         Returns:
             list: All followers or followings.
         """
+        def filter_data(response):
+            filtered_data = []
+            for each_entry in response:
+                if total is not None and (len(user_friends) + len(filtered_data)) >= total:
+                    return filtered_data
+                filtered_data.append(each_entry)
+            return filtered_data
         if (not followers_list and not followings_list) or (followers_list and followings_list):
             raise Exception(
                 "Set either the followers_list or the followings_list to True.")
         if not self.logged_in():
             self.login()
         user = self.get_user_basic_details(username)
         count = user['follower_count'] if followers_list else user['following_count'] if followings_list else None
@@ -353,40 +360,40 @@
                     end_cursor = data['page_info']['end_cursor']
                     data = data['edges']
                 else:
                     data = response['users']
                     if 'next_max_id' in response.keys():
                         end_cursor = response['next_max_id']
                     has_next_page = response['big_list']
-                user_friends.extend(data)
+                user_friends.extend(filter_data(data))
 
                 print(
                     f"{user['username']} : {len(user_friends)} / {count}", end="\r")
-                if not has_next_page or (max is not None and len(user_friends) >= max):
+                if not has_next_page or (total is not None and len(user_friends) >= total):
                     return user_friends
 
                 self.shuffle_session()
 
             except ConnectionError as error:
                 print(error)
                 continue
 
             except Exception as error:
                 print(error)
                 return user_friends
 
-    def get_profile_media(self, username, end_cursor=None, from_date=None, to_date=None, max=None):
+    def get_profile_media(self, username, end_cursor=None, from_date=None, to_date=None, total=None):
         """Returns all media/posts of the given Instagram Profile.
 
         Args:
             username (str): Instagram Username.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             from_date (str, optional): FORMAT - 'Year-Month-Date' Fetch posts starting from a specified period of time. Defaults to None.
             to_date (str, optional): FORMAT - 'Year-Month-Date'  Fetch posts upto a specified period of time. Defaults to None.
-            max (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
+            total (int, optional): Total number of results to extract. Defaults to None. -- Gets all by default.
 
         Returns:
             list: All Posts of the given Instagram user.
         """
         def filter_by_date(user_posts):
             posts_data = []
             for each_post in user_posts:
@@ -395,15 +402,15 @@
                 if from_date is not None:
                     if post_date <= from_date:
                         continue
                 if to_date is not None:
                     if post_date >= to_date:
                         continue
                 posts_data.append(each_post)
-                if max is not None and (len(user_posts_data) + len(posts_data)) >= max:
+                if total is not None and (len(user_posts_data) + len(posts_data)) >= total:
                     return posts_data
             return posts_data
 
         user = self.get_user_basic_details(username)
         user_id = user['id']
         user_posts_data = []
         if from_date is not None:
@@ -438,15 +445,15 @@
                     print(error)
                     return user_posts_data
 
                 if from_date:
                     if any(datetime.datetime.fromtimestamp(post['node']['taken_at_timestamp']) <= from_date for post in data['edges']):
                         return user_posts_data
 
-                if not has_next_page or (max is not None and len(user_posts_data) >= max):
+                if not has_next_page or (total is not None and len(user_posts_data) >= total):
                     return user_posts_data
 
                 self.shuffle_session()
 
         except Exception as e:
             print(e)
 
@@ -503,26 +510,33 @@
             'bloks_version': path.ABOUT_USER_QUERY, 'style_id': 'instagram'}, 'bloks_versioning_id': path.ABOUT_USER_QUERY}
         response = make_request(path.ABOUT_USER_URL, method='POST', data=data)
         if print_formatted:
             return utils.format_about_data(response)
         self.shuffle_session()
         return response
 
-    def get_hashtag_posts(self, hashtag=None, end_cursor=None, max=None):
+    def get_hashtag_posts(self, hashtag=None, end_cursor=None, total=None):
         """Get media posts from hashtags.
 
         Args:
             # hashtag. Defaults to None.
             hashtag (str): Hashtag that you want to extract data from. Accepts both formats i.e. hashtag or
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
-            max (int, optional): Number of results per request to extract from Instagram Database. Defaults to None.
+            total (int, optional): Total number of results to extract. Defaults to None. -- Gets all by default.
 
         Returns:
             dict: Hashtag posts data.
         """
+        def filter_data(response):
+            filtered_data = []
+            for each_entry in response:
+                if total is not None and (len(hashtag_posts) + len(filtered_data)) >= total:
+                    return filtered_data
+                filtered_data.append(each_entry)
+            return filtered_data
         if hashtag is None:
             raise Exception("No hashtag was given.")
         if not self.logged_in():
             self.login()
         hashtag = hashtag.lstrip("#")
         hashtag_posts = []
         url = path.GRAPHQL_URL
@@ -536,18 +550,18 @@
                 response = make_request(url, params=query_params)
                 data = response['data']['hashtag']['edge_hashtag_to_media']
                 has_next_page = data['page_info']['has_next_page']
                 end_cursor = data['page_info']['end_cursor']
                 count = data['count']
                 data = data['edges']
 
-                hashtag_posts.extend(data)
+                hashtag_posts.extend(filter_data(data))
                 print(
                     f"#{hashtag} : {len(hashtag_posts)} / {count}", end="\r")
-                if not has_next_page or (max is not None and len(hashtag_posts) >= max):
+                if not has_next_page or (total is not None and len(hashtag_posts) >= total):
                     return hashtag_posts
 
                 self.shuffle_session()
 
             except ConnectionError as error:
                 print(error)
                 continue
```

### Comparing `instagpy-0.1.8/instagpy/path.py` & `instagpy-0.1.9/instagpy/path.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy/request_util.py` & `instagpy-0.1.9/instagpy/request_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy/session_util.py` & `instagpy-0.1.9/instagpy/session_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy/utils.py` & `instagpy-0.1.9/instagpy/utils.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.8/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.9/instagpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.8 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.9 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.8/setup.py` & `instagpy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

