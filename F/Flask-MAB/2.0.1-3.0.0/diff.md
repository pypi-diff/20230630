# Comparing `tmp/Flask-MAB-2.0.1.tar.gz` & `tmp/Flask-MAB-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-MAB-2.0.1.tar", last modified: Thu Jan 10 15:32:17 2019, max compression
+gzip compressed data, was "Flask-MAB-3.0.0.tar", last modified: Fri Jun 30 19:57:45 2023, max compression
```

## Comparing `Flask-MAB-2.0.1.tar` & `Flask-MAB-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,62 @@
-drwxr-xr-x   0 mgthesecond   (501) staff       (20)        0 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/
-drwxr-xr-x   0 mgthesecond   (501) staff       (20)        0 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/
--rw-r--r--   0 mgthesecond   (501) staff       (20)      800 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/PKG-INFO
--rw-r--r--   0 mgthesecond   (501) staff       (20)      332 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/SOURCES.txt
--rw-r--r--   0 mgthesecond   (501) staff       (20)        1 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/dependency_links.txt
--rw-r--r--   0 mgthesecond   (501) staff       (20)        1 2014-01-28 21:53:38.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/not-zip-safe
--rw-r--r--   0 mgthesecond   (501) staff       (20)       55 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/requires.txt
--rw-r--r--   0 mgthesecond   (501) staff       (20)       10 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/Flask_MAB.egg-info/top_level.txt
--rw-r--r--   0 mgthesecond   (501) staff       (20)      800 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/PKG-INFO
--rw-r--r--   0 mgthesecond   (501) staff       (20)    10834 2019-01-10 00:28:30.000000 Flask-MAB-2.0.1/README.rst
-drwxr-xr-x   0 mgthesecond   (501) staff       (20)        0 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/flask_mab/
--rw-r--r--   0 mgthesecond   (501) staff       (20)     8297 2019-01-10 15:31:29.000000 Flask-MAB-2.0.1/flask_mab/__init__.py
--rw-r--r--   0 mgthesecond   (501) staff       (20)     6584 2019-01-10 15:31:29.000000 Flask-MAB-2.0.1/flask_mab/bandits.py
--rw-r--r--   0 mgthesecond   (501) staff       (20)     1602 2019-01-10 01:43:02.000000 Flask-MAB-2.0.1/flask_mab/debug_panels.py
--rw-r--r--   0 mgthesecond   (501) staff       (20)      356 2019-01-10 01:43:02.000000 Flask-MAB-2.0.1/flask_mab/mab.py
--rw-r--r--   0 mgthesecond   (501) staff       (20)     1748 2014-11-04 02:56:50.000000 Flask-MAB-2.0.1/flask_mab/storage.py
--rw-r--r--   0 mgthesecond   (501) staff       (20)      181 2019-01-10 15:32:17.000000 Flask-MAB-2.0.1/setup.cfg
--rw-r--r--   0 mgthesecond   (501) staff       (20)     1227 2019-01-10 15:31:29.000000 Flask-MAB-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.182747 Flask-MAB-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.166746 Flask-MAB-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.170747 Flask-MAB-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.170747 Flask-MAB-3.0.0/Flask_MAB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-06-30 19:57:45.000000 Flask-MAB-3.0.0/Flask_MAB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-30 19:57:45.000000 Flask-MAB-3.0.0/Flask_MAB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:57:45.000000 Flask-MAB-3.0.0/Flask_MAB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-30 19:57:45.000000 Flask-MAB-3.0.0/Flask_MAB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-30 19:57:45.000000 Flask-MAB-3.0.0/Flask_MAB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-06-30 19:57:45.178747 Flask-MAB-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.174747 Flask-MAB-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.174747 Flask-MAB-3.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   261566 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/_static/debug_toolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32304 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/_static/flask_mab.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/bandits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/caveats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/debug_toolbar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/flask_mab.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/docs/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.174747 Flask-MAB-3.0.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/example_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/example_app_with_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.174747 Flask-MAB-3.0.0/example/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/static/btnstyles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.174747 Flask-MAB-3.0.0/example/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/templates/btnclick.html
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/example/templates/ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.178747 Flask-MAB-3.0.0/flask_mab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/bandits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/debug_panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.166746 Flask-MAB-3.0.0/flask_mab/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.178747 Flask-MAB-3.0.0/flask_mab/templates/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/flask_mab/templates/panels/mab-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:57:45.182747 Flask-MAB-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:57:45.178747 Flask-MAB-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_app_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_bandits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_corner_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_request_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/test_request_flow_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-30 19:57:14.000000 Flask-MAB-3.0.0/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-MAB-2.0.1/README.rst` & `Flask-MAB-3.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Flask-MAB
 =========
 
-.. image:: https://badges.gitter.im/flask_mab/Lobby.svg
-   :alt: Join the chat at https://gitter.im/flask_mab/Lobby
-   :target: https://gitter.im/flask_mab/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-
 .. image:: https://travis-ci.org/DeaconDesperado/flask_mab.png?:target: https://travis-ci.org/DeaconDesperado/flask_mab
 
 Flask-MAB is an implementation of multi-armed bandit test pattern as a flask middleware.
 
 It can be used to test the effectiveness of virtually any parts of your app using user signals.
 
 If you can pass it, we can test it!
```

### Comparing `Flask-MAB-2.0.1/flask_mab/__init__.py` & `Flask-MAB-3.0.0/flask_mab/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,62 +22,71 @@
 try:
     from flask import _app_ctx_stack as stack
 except ImportError:
     from flask import _request_ctx_stack as stack
 
 __version__ = "2.0.1"
 
+
 def choose_arm(bandit):
     """Route decorator for registering an impression conveinently
 
     :param bandit: The bandit/experiment to register for
     :type bandit: string
     """
+
     def decorator(func):
-        #runs @ service init
-        if not hasattr(func, 'bandits'):
+        # runs @ service init
+        if not hasattr(func, "bandits"):
             func.bandits = []
         func.bandits.append(bandit)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
-            #runs at endpoint hit
+            # runs at endpoint hit
             add_args = []
             for bandit in func.bandits:
-                #Fetch from request first here?
+                # Fetch from request first here?
                 arm_id, arm_value = suggest_arm_for(bandit)
                 add_args.append((bandit, arm_value))
             kwargs.update(add_args)
             return func(*args, **kwargs)
+
         return wrapper
+
     return decorator
 
 
 def reward_endpt(bandit, reward_val=1):
     """Route decorator for rewards.
 
     :param bandit: The bandit/experiment to register rewards
                    for using arm found in cookie.
     :type bandit: string
     :param reward: The amount of reward this endpoint should
                    give its winning arm
     :type reward: float
     """
+
     def decorator(func):
-        if not hasattr(func, 'rewards'):
+        if not hasattr(func, "rewards"):
             func.rewards = []
         func.rewards.append((bandit, reward_val))
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             for bandit, reward_amt in func.rewards:
                 if bandit in request.bandits.keys():
-                    request.bandits_reward.add((bandit, request.bandits[bandit], reward_amt))
+                    request.bandits_reward.add(
+                        (bandit, request.bandits[bandit], reward_amt)
+                    )
             return func(*args, **kwargs)
+
         return wrapper
+
     return decorator
 
 
 class BanditMiddleware(object):
     """The main flask extension.
     Sets up all the necessary tracking for the bandit experiments
     """
@@ -88,49 +97,48 @@
         :param app: An optional Flask application
         """
         if app is not None:
             self.init_app(app)
 
     def _register_storage(self, app):
         storage_engine = getattr(
-                flask_mab.storage,
-                app.config.get('MAB_STORAGE_ENGINE', 'BanditStorage'))
-        storage_opts = app.config.get('MAB_STORAGE_OPTS', tuple())
+            flask_mab.storage, app.config.get("MAB_STORAGE_ENGINE", "BanditStorage")
+        )
+        storage_opts = app.config.get("MAB_STORAGE_OPTS", tuple())
         storage_backend = storage_engine(*storage_opts)
-        app.extensions['mab'].bandit_storage = storage_backend
+        app.extensions["mab"].bandit_storage = storage_backend
 
     def init_app(self, app):
         """Attach Multi Armed Bandit to application and configure
 
         :param app: A flask application instance
         """
-        app.config.setdefault('MAB_COOKIE_NAME', 'MAB')
-        app.config.setdefault('MAB_COOKIE_PATH', '/')
-        app.config.setdefault('MAB_COOKIE_TTL', None)
-        app.config.setdefault('MAB_DEBUG_HEADERS', True)
-        if not hasattr(app, 'extensions'):
+        app.config.setdefault("MAB_COOKIE_NAME", "MAB")
+        app.config.setdefault("MAB_COOKIE_PATH", "/")
+        app.config.setdefault("MAB_COOKIE_TTL", None)
+        app.config.setdefault("MAB_DEBUG_HEADERS", True)
+        if not hasattr(app, "extensions"):
             app.extensions = {}
-        app.extensions['mab'] = Mab(app)
+        app.extensions["mab"] = Mab(app)
         self._register_storage(app)
-        if hasattr(app, 'teardown_appcontext'):
+        if hasattr(app, "teardown_appcontext"):
             app.teardown_appcontext(self.teardown)
         else:
             app.teardown_request(self.teardown)
 
-        app.extensions['mab'].bandits = {}
-        app.extensions['mab'].reward_endpts = []
-        app.extensions['mab'].pull_endpts = []
+        app.extensions["mab"].bandits = {}
+        app.extensions["mab"].reward_endpts = []
+        app.extensions["mab"].pull_endpts = []
 
-        app.extensions['mab'].debug_headers = app.config.get('MAB_DEBUG_HEADERS', True)
-        app.extensions['mab'].cookie_name = app.config.get('MAB_COOKIE_NAME', "MAB")
+        app.extensions["mab"].debug_headers = app.config.get("MAB_DEBUG_HEADERS", True)
+        app.extensions["mab"].cookie_name = app.config.get("MAB_COOKIE_NAME", "MAB")
         self._init_detection(app)
 
     def teardown(self, *args, **kwargs):
-        """Stub for old flask versions
-        """
+        """Stub for old flask versions"""
         pass
 
     def _init_detection(self, app):
         """
         Attaches all request before/after handlers for bandits.
 
         Nested functions are as follows
@@ -138,72 +146,80 @@
         * detect_last_bandits: Loads any arms already assigned to this user
                                from the cookie.
         * persist_bandits:     Saves bandits down to storage engine at the end
                                of the request
         * remember_bandit_arms: Sets the cookie for all requests that pulled an arm
         * send_debug_header: Attaches a header for the MAB to the HTTP response for easier debugging
         """
+
         @app.before_request
         def detect_last_bandits():
-            bandits = request.cookies.get(app.extensions['mab'].cookie_name)
+            bandits = request.cookies.get(app.extensions["mab"].cookie_name)
             request.bandits_save = False
             request.bandits_reward = set()
             if bandits:
                 request.bandits = json.loads(bandits)
             else:
                 request.bandits = {}
 
         @app.after_request
         def persist_bandits(response):
-            app.extensions['mab'].bandit_storage.save(app.extensions['mab'].bandits)
+            app.extensions["mab"].bandit_storage.save(app.extensions["mab"].bandits)
             return response
 
         @app.after_request
         def remember_bandit_arms(response):
             if request.bandits_save:
-                for bandit_id,arm in request.bandits.items():
-                    #hook event for saving an impression here
-                    app.extensions['mab'].bandits[bandit_id].pull_arm(arm)
+                for bandit_id, arm in request.bandits.items():
+                    # hook event for saving an impression here
+                    app.extensions["mab"].bandits[bandit_id].pull_arm(arm)
 
             for bandit_id, arm, reward_amt in request.bandits_reward:
                 try:
-                    app.extensions['mab'].bandits[bandit_id].reward_arm(arm, reward_amt)
-                    #hook event for saving a reward line here
+                    app.extensions["mab"].bandits[bandit_id].reward_arm(arm, reward_amt)
+                    # hook event for saving a reward line here
                 except KeyError:
                     raise MABConfigException("Bandit %s not found" % bandit_id)
 
             response.set_cookie(
-                    app.extensions['mab'].cookie_name,
-                    json.dumps(request.bandits))
+                app.extensions["mab"].cookie_name,
+                json.dumps(request.bandits),
+                secure=True,
+                httponly=True,
+                samesite="Lax",
+            )
             return response
 
         @app.after_request
         def send_debug_header(response):
-            if app.extensions['mab'].debug_headers and request.bandits_save:
-                response.headers['X-MAB-Debug'] = "STORE; "+';'.join(
-                        ['%s:%s' % (key, val) for key, val in request.bandits.items()])
-            elif app.extensions['mab'].debug_headers:
-                response.headers['X-MAB-Debug'] = "SAVED; "+';'.join(['%s:%s' % (key, val) for key, val in request.bandits.items()])
+            if app.extensions["mab"].debug_headers and request.bandits_save:
+                response.headers["X-MAB-Debug"] = "STORE; " + ";".join(
+                    ["%s:%s" % (key, val) for key, val in request.bandits.items()]
+                )
+            elif app.extensions["mab"].debug_headers:
+                response.headers["X-MAB-Debug"] = "SAVED; " + ";".join(
+                    ["%s:%s" % (key, val) for key, val in request.bandits.items()]
+                )
             return response
 
         app.add_bandit = types.MethodType(add_bandit, app)
 
 
 def add_bandit(app, name, bandit=None):
     """Attach a bandit for an experiment
 
     :param name: The name of the experiment, will be used for lookups
     :param bandit: The bandit to use for this experiment
     :type bandit: Bandit
     """
-    saved_bandits = app.extensions['mab'].bandit_storage.load()
+    saved_bandits = app.extensions["mab"].bandit_storage.load()
     if name in saved_bandits.keys():
-        app.extensions['mab'].bandits[name] = saved_bandits[name]
+        app.extensions["mab"].bandits[name] = saved_bandits[name]
     else:
-        app.extensions['mab'].bandits[name] = bandit
+        app.extensions["mab"].bandits[name] = bandit
 
 
 def suggest_arm_for(key):
     """Get an experimental outcome by id.  The primary way the implementor interfaces with their
     experiments.
 
     Suggests arms if not in cookie, using cookie val if present
@@ -211,23 +227,25 @@
     :param key: The bandit/experiment to get a suggested arm for
     :type key: string
     :param also_pull: Should we register a pull/impression at the same time as suggesting
     :raises KeyError: in case requested experiment does not exist
     """
     app = current_app
     try:
-        #Try to get the selected bandits from cookie
-        arm = app.extensions['mab'].bandits[key][request.bandits[key]]
+        # Try to get the selected bandits from cookie
+        arm = app.extensions["mab"].bandits[key][request.bandits[key]]
         return arm["id"], arm["value"]
     except (AttributeError, TypeError, KeyError) as err:
-        #Assign an arm for a new client
+        # Assign an arm for a new client
         try:
-            arm = app.extensions['mab'].bandits[key].suggest_arm()
+            arm = app.extensions["mab"].bandits[key].suggest_arm()
             request.bandits[key] = arm["id"]
             request.bandits_save = True
             return arm["id"], arm["value"]
         except KeyError:
             raise MABConfigException("Bandit %s not found" % key)
 
+
 class MABConfigException(Exception):
     """Raised when internal state in MAB setup is invalid"""
+
     pass
```

### Comparing `Flask-MAB-2.0.1/flask_mab/bandits.py` & `Flask-MAB-3.0.0/flask_mab/bandits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 from random import random, choice, uniform, betavariate
 from math import log, exp, expm1
 
+
 class Bandit(object):
     """The primary bandit interface.  Don't use this unless you really
     want uniform random arm selection (which defeats the whole purpose, really)
 
     Used as a control to test against and as an interface to define methods against.
     """
 
     @classmethod
     def fromdict(cls, dict_spec):
-        extra_args = dict([(key, value) for key, value in dict_spec.items() if key not in ["arms", "pulls", "reward", "values", "bandit_type", "confidence"]])
+        extra_args = dict(
+            [
+                (key, value)
+                for key, value in dict_spec.items()
+                if key
+                not in [
+                    "arms",
+                    "pulls",
+                    "reward",
+                    "values",
+                    "bandit_type",
+                    "confidence",
+                ]
+            ]
+        )
 
         bandit = globals()[dict_spec["bandit_type"]](**extra_args)
         bandit.arms = dict_spec["arms"]
         bandit.pulls = dict_spec["pulls"]
         bandit.reward = dict_spec["reward"]
         bandit.values = dict_spec["values"]
         bandit.confidence = dict_spec.get("confidence", [0.0] * len(bandit.arms))
@@ -44,41 +59,46 @@
         if ind > -1:
             self.reward[ind] += reward
         self._update(ind, reward)
 
     def _update(self, arm_index, reward):
         n = max(1, self.pulls[arm_index])
         current = self.confidence[arm_index]
-        self.confidence[arm_index] = ((n - 1) / float(n)) * current + (1 / float(n)) * reward
+        self.confidence[arm_index] = ((n - 1) / float(n)) * current + (
+            1 / float(n)
+        ) * reward
 
     def suggest_arm(self):
         """Uniform random for default bandit.
 
         Just uses random.choice to choose between arms
         """
         return self[random.choice(self.arms)]
 
     def __getitem__(self, key):
         ind = self.arms.index(key)
         if ind > -1:
             arm = {
-                    "id":self.arms[ind],
-                    "pulls":self.pulls[ind],
-                    "reward":self.reward[ind],
-                    "value":self.values[ind]
-                    }
+                "id": self.arms[ind],
+                "pulls": self.pulls[ind],
+                "reward": self.reward[ind],
+                "value": self.values[ind],
+            }
             return arm
         else:
             raise KeyError("Arm is not found in this bandit")
 
     def __str__(self):
-        output = '%s  ' % self.__class__.__name__
-        output += '; '.join(['%s:%s' % (key, val) for key, val in self.__dict__.items()])
+        output = "%s  " % self.__class__.__name__
+        output += "; ".join(
+            ["%s:%s" % (key, val) for key, val in self.__dict__.items()]
+        )
         return output
 
+
 class EpsilonGreedyBandit(Bandit):
     """Epsilon Greedy Bandit implementation.  Aggressively favors the present winner.
 
     Will assign winning arm 1.0 - epsilon of the time, uniform random between arms
     epsilon % of the time.
 
     Will "exploit" the present winner more often with lower values of epsilon, "explore"
@@ -90,16 +110,15 @@
     """
 
     def __init__(self, epsilon=0.1):
         super(EpsilonGreedyBandit, self).__init__()
         self.epsilon = epsilon
 
     def suggest_arm(self):
-        """Get an arm according to the EpsilonGreedy Strategy
-        """
+        """Get an arm according to the EpsilonGreedy Strategy"""
         random_determination = random()
         if random_determination > self.epsilon:
             key = self._ind_max()
         else:
             key = choice(self.arms)
 
         return self[key]
@@ -109,17 +128,19 @@
 
     def __str__(self):
         return Bandit.__str__(self)
 
     def __repr(self):
         return Bandit.__str__(self)
 
+
 def all_same(items):
     return all(x == items[0] for x in items)
 
+
 class NaiveStochasticBandit(Bandit):
     """A naive weighted random Bandit.  Favors the winner by giving it greater weight
     in random selection.
 
     Winner will eventually flatten out the losers if margin is great enough
     """
 
@@ -127,73 +148,73 @@
         super(NaiveStochasticBandit, self).__init__()
 
     def _compute_weights(self):
         weights = []
         for ind, n in enumerate(self.pulls):
             reward = self.reward[ind]
             try:
-                weights.append(1.0 * (float(reward)/float(n)))
+                weights.append(1.0 * (float(reward) / float(n)))
             except ZeroDivisionError:
-                weights.append(1.0/len(self.arms))
+                weights.append(1.0 / len(self.arms))
         return weights
 
     def suggest_arm(self):
-        """Get an arm according to the Naive Stochastic Strategy
-        """
+        """Get an arm according to the Naive Stochastic Strategy"""
         weights = self._compute_weights()
         random_determination = uniform(0.0, 1.0)
 
         cum_weight = 0.0
         for ind, weight in enumerate(weights):
             cum_weight += weight
             if cum_weight > random_determination:
                 return self[self.arms[ind]]
         return self[self.arms[0]]
 
 
 class SoftmaxBandit(NaiveStochasticBandit):
-
     def __init__(self, tau=0.1):
         super(SoftmaxBandit, self).__init__()
         self.tau = tau
 
     def _compute_weights(self):
         weights = []
         total_reward = sum([exp(x / self.tau) for x in self.confidence])
         for ind, n in enumerate(self.pulls):
             weights.append(exp(self.confidence[ind] / self.tau) / total_reward)
         return weights
 
 
 class AnnealingSoftmaxBandit(SoftmaxBandit):
-
     def __init__(self):
         super(AnnealingSoftmaxBandit, self).__init__()
         self.tau = 1
 
     def _compute_weights(self):
         t = sum(self.pulls) + 1
-        self.tau = 1 / log(t +  0.0000001)
+        self.tau = 1 / log(t + 0.0000001)
 
         weights = []
         total_reward = sum([exp(x / self.tau) for x in self.confidence])
         for ind, n in enumerate(self.pulls):
             weights.append(exp(self.confidence[ind] / self.tau) / total_reward)
         return weights
 
-class ThompsonBandit(NaiveStochasticBandit):
 
-    def __init__(self, prior=(1.0,1.0)):
+class ThompsonBandit(NaiveStochasticBandit):
+    def __init__(self, prior=(1.0, 1.0)):
         super(ThompsonBandit, self).__init__()
         self.prior = prior
 
     def _compute_weights(self):
         sampled_theta = []
         for ind, n in enumerate(self.arms):
-            dist = betavariate(self.prior[0] + self.reward[ind], self.prior[1]+self.pulls[ind]-self.reward[ind])
+            dist = betavariate(
+                self.prior[0] + self.reward[ind],
+                self.prior[1] + self.pulls[ind] - self.reward[ind],
+            )
             sampled_theta += [dist]
         return sampled_theta
 
     def suggest_arm(self):
         weights = self._compute_weights()
         return self[self.arms[weights.index(max(weights))]]
```

### Comparing `Flask-MAB-2.0.1/flask_mab/debug_panels.py` & `Flask-MAB-3.0.0/flask_mab/debug_panels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from flask import current_app
 from flask_debugtoolbar.panels import DebugPanel
 from jinja2 import PackageLoader, ChoiceLoader
 import json
 
-package_loader = PackageLoader('flask_mab', 'templates')
+package_loader = PackageLoader("flask_mab", "templates")
+
 
 def _maybe_patch_jinja_loader(jinja_env):
     """Patch the jinja_env loader to include
     templates folder if necessary.
     """
     if not isinstance(jinja_env.loader, ChoiceLoader):
         jinja_env.loader = ChoiceLoader([jinja_env.loader, package_loader])
     elif package_loader not in jinja_env.loader.loaders:
         jinja_env.loader.loaders.append(package_loader)
 
-class BanditDebugPanel(DebugPanel):
 
+class BanditDebugPanel(DebugPanel):
     name = "Multi-Armed Bandit"
     has_content = True
 
     def __init__(self, *args, **kwargs):
         super(BanditDebugPanel, self).__init__(*args, **kwargs)
         _maybe_patch_jinja_loader(self.jinja_env)
 
     def nav_title(self):
         return "Multi-Armed Bandit"
 
     def title(self):
         return "Multi-Armed Bandit"
 
     def url(self):
-        return ''
+        return ""
 
     def process_request(self, request):
-        self.raw_cookie = request.cookies.get(current_app.extensions['mab'].cookie_name, '{}')
+        self.raw_cookie = request.cookies.get(
+            current_app.extensions["mab"].cookie_name, "{}"
+        )
 
     def content(self):
         context = self.context.copy()
-        context['cookie_name'] = current_app.extensions['mab'].cookie_name
-        context['raw_cookie'] = self.raw_cookie
-        context['storage_engine'] = current_app.config.get("MAB_STORAGE_ENGINE")
-        context['storage_opts'] = current_app.config.get('MAB_STORAGE_OPTS', tuple())
-        context['bandits'] = current_app.extensions['mab'].bandits.items()
-        return self.render('panels/mab-panel.html', context)
+        context["cookie_name"] = current_app.extensions["mab"].cookie_name
+        context["raw_cookie"] = self.raw_cookie
+        context["storage_engine"] = current_app.config.get("MAB_STORAGE_ENGINE")
+        context["storage_opts"] = current_app.config.get("MAB_STORAGE_OPTS", tuple())
+        context["bandits"] = current_app.extensions["mab"].bandits.items()
+        return self.render("panels/mab-panel.html", context)
```

### Comparing `Flask-MAB-2.0.1/flask_mab/storage.py` & `Flask-MAB-3.0.0/flask_mab/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,63 +2,68 @@
 Defines various storage engines for the MAB
 interface
 """
 
 import json
 import flask_mab.bandits
 
+
 class BanditEncoder(json.JSONEncoder):
     """Json serializer for Bandits"""
+
     def default(self, obj):
         if isinstance(obj, flask_mab.bandits.Bandit):
             dict_repr = obj.__dict__
-            dict_repr['bandit_type'] = obj.__class__.__name__
+            dict_repr["bandit_type"] = obj.__class__.__name__
             return dict_repr
         return json.JSONEncoder.default(self, obj)
 
+
 class BanditDecoder(json.JSONDecoder):
     """Json Marshaller for Bandits"""
+
     def decode(self, obj):
         dict_repr = json.loads(obj)
         for key in dict_repr.keys():
-            if 'bandit_type' not in dict_repr[key].keys():
+            if "bandit_type" not in dict_repr[key].keys():
                 raise TypeError("Serialized object is not a valid bandit")
             dict_repr[key] = flask_mab.bandits.Bandit.fromdict(dict_repr[key])
         return dict_repr
 
+
 class BanditStorage(object):
-    """The base interface for a storage engine, implements no-ops for tests
-    """
+    """The base interface for a storage engine, implements no-ops for tests"""
 
     def flush(self):
         pass
 
     def save(self, bandits):
         pass
 
     def load(self):
         return {}
 
+
 class JSONBanditStorage(BanditStorage):
     """Json based file storage
 
     Saves to local file
     """
+
     def __init__(self, filepath):
         self.file_handle = filepath
 
     def flush(self):
-        open(self.file_handle, 'w').truncate()
+        open(self.file_handle, "w").truncate()
 
     def save(self, bandits):
         json_bandits = json.dumps(bandits, indent=4, cls=BanditEncoder)
-        open(self.file_handle, 'w').write(json_bandits)
+        open(self.file_handle, "w").write(json_bandits)
 
     def load(self):
         try:
-            with open(self.file_handle, 'r') as bandit_file:
+            with open(self.file_handle, "r") as bandit_file:
                 bandits = bandit_file.read()
 
             return json.loads(bandits, cls=BanditDecoder)
         except (ValueError, IOError):
             return {}
-
```

