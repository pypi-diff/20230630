# Comparing `tmp/jipdate-2.0.1.tar.gz` & `tmp/jipdate-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jipdate-2.0.1.tar", last modified: Thu Jun  1 13:23:57 2023, max compression
+gzip compressed data, was "jipdate-2.0.2.tar", last modified: Fri Jun 30 07:34:44 2023, max compression
```

## Comparing `jipdate-2.0.1.tar` & `jipdate-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       66 2022-01-05 21:22:55.225653 jipdate-2.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2021-09-27 12:17:51.864950 jipdate-2.0.1/LICENSE
--rw-r--r--   0        0        0      460 2022-01-05 21:22:55.225653 jipdate-2.0.1/README.md
--rw-r--r--   0        0        0      604 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/Makefile
--rw-r--r--   0        0        0      142 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/_static/css/mystyle.css
--rw-r--r--   0        0        0      618 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/about.rst
--rw-r--r--   0        0        0     5130 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/conf.py
--rw-r--r--   0        0        0     7345 2022-01-12 10:13:55.631749 jipdate-2.0.1/docs/config.rst
--rw-r--r--   0        0        0      181 2023-05-31 10:40:14.000989 jipdate-2.0.1/docs/index.rst
--rw-r--r--   0        0        0     2700 2023-06-01 13:10:59.581924 jipdate-2.0.1/docs/install.rst
--rw-r--r--   0        0        0     2195 2023-05-31 10:40:14.012989 jipdate-2.0.1/docs/jipcreate.rst
--rw-r--r--   0        0        0     6277 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/jipdate.rst
--rw-r--r--   0        0        0     2259 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/jipstatus.rst
--rw-r--r--   0        0        0     1576 2022-01-05 21:22:55.225653 jipdate-2.0.1/docs/problems.rst
--rw-r--r--   0        0        0     1461 2023-05-31 10:40:14.004989 jipdate-2.0.1/docs/run.rst
--rw-r--r--   0        0        0       57 2023-06-01 13:23:12.698786 jipdate-2.0.1/jipdate/__init__.py
--rw-r--r--   0        0        0     3547 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/cfg.py
--rwxr-xr-x   0        0        0    10353 2023-05-31 10:40:14.016989 jipdate-2.0.1/jipdate/jipcreate.py
--rwxr-xr-x   0        0        0    19627 2023-05-31 10:40:14.016989 jipdate-2.0.1/jipdate/jipdate.py
--rwxr-xr-x   0        0        0    19865 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jipfp.py
--rwxr-xr-x   0        0        0     8518 2023-06-01 13:13:27.390894 jipdate-2.0.1/jipdate/jipsearch.py
--rwxr-xr-x   0        0        0     9912 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jipstatus.py
--rw-r--r--   0        0        0     3610 2023-05-31 10:40:13.992989 jipdate-2.0.1/jipdate/jiralogin.py
--rw-r--r--   0        0        0      664 2023-06-01 12:33:43.359601 jipdate-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 jipdate-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-06-02 15:53:59.296976 jipdate-2.0.2/.github/workflows/jipdate-pipeline.yml
+-rw-r--r--   0        0        0       66 2022-01-05 21:22:55.225653 jipdate-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2021-09-27 12:17:51.864950 jipdate-2.0.2/LICENSE
+-rw-r--r--   0        0        0      460 2022-01-05 21:22:55.225653 jipdate-2.0.2/README.md
+-rw-r--r--   0        0        0      604 2022-01-05 21:22:55.225653 jipdate-2.0.2/docs/Makefile
+-rw-r--r--   0        0        0      142 2022-01-05 21:22:55.225653 jipdate-2.0.2/docs/_static/css/mystyle.css
+-rw-r--r--   0        0        0      618 2022-01-05 21:22:55.225653 jipdate-2.0.2/docs/about.rst
+-rw-r--r--   0        0        0     5201 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/conf.py
+-rw-r--r--   0        0        0     7345 2022-01-12 10:13:55.631749 jipdate-2.0.2/docs/config.rst
+-rw-r--r--   0        0        0      181 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/index.rst
+-rw-r--r--   0        0        0     2700 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/install.rst
+-rw-r--r--   0        0        0     2195 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/jipcreate.rst
+-rw-r--r--   0        0        0     6277 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/jipdate.rst
+-rw-r--r--   0        0        0     2259 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/jipstatus.rst
+-rw-r--r--   0        0        0     1576 2022-01-05 21:22:55.225653 jipdate-2.0.2/docs/problems.rst
+-rw-r--r--   0        0        0     1461 2023-06-02 15:53:59.296976 jipdate-2.0.2/docs/run.rst
+-rw-r--r--   0        0        0       57 2023-06-30 07:23:47.325986 jipdate-2.0.2/jipdate/__init__.py
+-rw-r--r--   0        0        0     3536 2023-06-02 15:53:59.296976 jipdate-2.0.2/jipdate/cfg.py
+-rwxr-xr-x   0        0        0    11840 2023-06-28 11:52:46.908251 jipdate-2.0.2/jipdate/jipcreate.py
+-rwxr-xr-x   0        0        0    20639 2023-06-28 11:53:18.088546 jipdate-2.0.2/jipdate/jipdate.py
+-rwxr-xr-x   0        0        0    20332 2023-06-28 11:50:12.854765 jipdate-2.0.2/jipdate/jipfp.py
+-rwxr-xr-x   0        0        0    12695 2023-06-28 11:53:21.976583 jipdate-2.0.2/jipdate/jipsearch.py
+-rwxr-xr-x   0        0        0    10560 2023-06-28 11:53:21.976583 jipdate-2.0.2/jipdate/jipstatus.py
+-rw-r--r--   0        0        0     3688 2023-06-02 15:53:59.296976 jipdate-2.0.2/jipdate/jiralogin.py
+-rw-r--r--   0        0        0      664 2023-06-02 15:53:59.296976 jipdate-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 jipdate-2.0.2/PKG-INFO
```

### Comparing `jipdate-2.0.1/LICENSE` & `jipdate-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/Makefile` & `jipdate-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/about.rst` & `jipdate-2.0.2/docs/about.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/conf.py` & `jipdate-2.0.2/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,151 +15,156 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
-project = u'Jipdate'
-copyright = u'2019, Linaro, Joakim Bech'
-author = u'Linaro, Joakim Bech'
+project = "Jipdate"
+copyright = "2019, Linaro, Joakim Bech"
+author = "Linaro, Joakim Bech"
 
 # The short X.Y version
-version = u''
+version = ""
 # The full version, including alpha/beta/rc tags
-release = u''
+release = ""
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.todo',
-    'sphinx.ext.imgmath',
-    'sphinx.ext.ifconfig',
+    "sphinx.ext.todo",
+    "sphinx.ext.imgmath",
+    "sphinx.ext.ifconfig",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
-exclude_patterns = [u'_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
-html_style = 'css/mystyle.css'
+html_style = "css/mystyle.css"
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
 # 'searchbox.html']``.
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'Jipdatedoc'
+htmlhelp_basename = "Jipdatedoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'Jipdate.tex', u'Jipdate Documentation',
-     u'Linaro, Joakim Bech', 'manual'),
+    (
+        master_doc,
+        "Jipdate.tex",
+        "Jipdate Documentation",
+        "Linaro, Joakim Bech",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'jipdate', u'Jipdate Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "jipdate", "Jipdate Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'Jipdate', u'Jipdate Documentation',
-     author, 'Jipdate', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "Jipdate",
+        "Jipdate Documentation",
+        author,
+        "Jipdate",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for todo extension ----------------------------------------------
```

### Comparing `jipdate-2.0.1/docs/config.rst` & `jipdate-2.0.2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/install.rst` & `jipdate-2.0.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/jipcreate.rst` & `jipdate-2.0.2/docs/jipcreate.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/jipdate.rst` & `jipdate-2.0.2/docs/jipdate.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/jipstatus.rst` & `jipdate-2.0.2/docs/jipstatus.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/problems.rst` & `jipdate-2.0.2/docs/problems.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/docs/run.rst` & `jipdate-2.0.2/docs/run.rst`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/jipdate/cfg.py` & `jipdate-2.0.2/jipdate/cfg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging as log
 import os
 import sys
 import yaml
 
-TEST_SERVER = { 'url' : 'https://dev-projects.linaro.org' }
-PRODUCTION_SERVER = { 'url' : 'https://projects.linaro.org' }
+TEST_SERVER = {"url": "https://dev-projects.linaro.org"}
+PRODUCTION_SERVER = {"url": "https://projects.linaro.org"}
 
 args = None
 
 # Config file paths and name, basically we allow the user to store the
 # .config.yml/config.yml in either the application directory, the $HOME
 # directory or the  $HOME/.config/jipdate directory.
 config_app_dir = sys.path[0]
-config_home_config_dir = os.environ['HOME'] + "/.config/jipdate"
-config_home_dir = os.environ['HOME']
+config_home_config_dir = os.environ["HOME"] + "/.config/jipdate"
+config_home_dir = os.environ["HOME"]
 config_locations = [config_app_dir, config_home_dir, config_home_config_dir]
 config_path = config_home_config_dir
 
 # Config filenames
 config_filename = ".jipdate.yml"
 config_legacy_filename = "config.yml"
 
@@ -27,16 +27,16 @@
 yml_config = None
 
 
 ################################################################################
 # Global config file used by different scripts
 ################################################################################
 def create_default_config():
-    """ Creates a default YAML config file for use with jipdate (default
-    location is $HOME/.config/jipdate """
+    """Creates a default YAML config file for use with jipdate (default
+    location is $HOME/.config/jipdate"""
     yml_cfg = """# Config file for jipdate
 # For use in future (backwards compatibility)
 version: 1
 
 # Jira server information
 #server:
 #  url: https://linaro.atlassian.net
@@ -68,20 +68,20 @@
 separator: ' | '
 text-editor: True"""
     global config_path
     global config_filename
 
     if not os.path.exists(config_path):
         os.makedirs(config_path)
-    with open(config_path + "/" + config_filename, 'w') as f:
+    with open(config_path + "/" + config_filename, "w") as f:
         f.write(yml_cfg)
 
 
 def get_config_file():
-    """ Returns the location for the config file (including the path). """
+    """Returns the location for the config file (including the path)."""
     global config_locations
     global config_legacy_filename
     global config_path
     global config_filename
 
     for d in config_locations:
         for f in [config_filename, config_legacy_filename]:
@@ -93,28 +93,28 @@
     return config_path + "/" + config_filename
 
 
 def get_server(use_test_server=False):
     # Get Jira Server details. Check first if using the test server
     # then try user config file, then default from cfg.py
     if use_test_server is False:
-        server = yml_config.get('server', PRODUCTION_SERVER)
+        server = yml_config.get("server", PRODUCTION_SERVER)
     else:
-        server = yml_config.get('test_server', TEST_SERVER)
+        server = yml_config.get("test_server", TEST_SERVER)
 
     return server
 
 
 def initiate_config():
-    """ Reads the config file (yaml format) and returns the sets the global
+    """Reads the config file (yaml format) and returns the sets the global
     instance.
     """
     global yml_config
     global config_file
 
     config_file = get_config_file()
     if not os.path.isfile(config_file):
         create_default_config()
 
     log.debug("Using config file: %s" % config_file)
-    with open(config_file, 'r') as yml:
+    with open(config_file, "r") as yml:
         yml_config = yaml.load(yml, Loader=yaml.FullLoader)
```

### Comparing `jipdate-2.0.1/jipdate/jipcreate.py` & `jipdate-2.0.2/jipdate/jipstatus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,240 +1,369 @@
 #!/usr/bin/env python3
 from argparse import ArgumentParser
 from subprocess import call
 from time import gmtime, strftime
+from jinja2 import Template
 
+import datetime
 import json
 import logging as log
 import os
 import re
 import sys
 import tempfile
 import yaml
 
 # Local files
 from jipdate import cfg
 from jipdate import jiralogin
+from jipdate import __version__
 
-################################################################################
-# Argument parser
-################################################################################
-def get_parser():
-    """ Takes care of script argument parsing. """
-    parser = ArgumentParser(description='Script used to create tickets in Jira')
+import pprint
 
-    parser.add_argument('-f', '--file', required=False, action="store", \
-            default=None, \
-            help='Create issue from FILE.')
-
-    parser.add_argument('-u', '--user', required=False, action="store", \
-            default=None, \
-            help='Query Jira with another Jira username \
-            (first.last or first.last@linaro.org)')
-
-    parser.add_argument('-v', required=False, action="store_true", \
-            default=False, \
-            help='Output some verbose debugging info')
-
-    parser.add_argument('--dry-run', required=False, action="store_true", \
-            default=False, \
-            help='Do not make any changes to JIRA')
+pprint = pprint.PrettyPrinter().pprint
 
-    return parser
 
-################################################################################
-# Jira functions
-################################################################################
-def parse_issue_file(new_issue_file):
-    """ Reads new issue file and parse it into a python object
+def add_domain(user):
     """
+    Helper function that appends @linaro.org to the username. It does nothing if
+    it is already included.
+    """
+    if "@" not in user:
+        user = user + "@linaro.org"
+    return user
+
+
+def default_jql():
+    project = cfg.args.project
+    team = cfg.args.team
+
+    if team and project:
+        jql = "(project = %s or assignee in membersOf('%s')) " % (project, team)
+    elif team:
+        jql = "assignee in membersOf('%s') " % team
+    elif project:
+        jql = "project =  '%s' " % project
+    else:
+        # cfg.args.user is a list with 1 or more users
+        # we construct the query as:
+        # (assignee = 'user1' or assignee = 'user2' )
+        users = list(map(add_domain, cfg.args.user))
+        jql = (
+            "(" + " or ".join(map(lambda str: "assignee = '" + str + "'", users)) + ")"
+        )
+
+    return jql
+
+
+def enumerate_updates(jira):
+    since = datetime.datetime.now() - datetime.timedelta(days=int(cfg.args.days))
+
+    jql = default_jql()
+    jql += "AND updatedDate > -%sd" % cfg.args.days
+    log.debug(jql)
+
+    my_issues = jira.search_issues(
+        jql, expand="changelog", fields="summary,comment,components,assignee,created"
+    )
+    if my_issues.total > my_issues.maxResults:
+        my_issues = jira.search_issues(
+            jql,
+            expand="changelog",
+            fields="summary,comment,components,assignee,created",
+            maxResults=my_issues.total,
+        )
+
+    for issue in my_issues:
+        changelog = issue.changelog
+        comments = issue.fields.comment.comments
+
+        status = {}
+        status["issue"] = str(issue)
+        if issue.fields.assignee:
+            status["assignee"] = issue.fields.assignee.displayName
+        else:
+            status["assignee"] = "Unassigned"
+        status["summary"] = issue.fields.summary
+        status["comments"] = []
+        status["resolution"] = None
+        status["components"] = issue.fields.components
+
+        created = datetime.datetime.strptime(
+            issue.fields.created, "%Y-%m-%dT%H:%M:%S.%f%z"
+        )
+        if created.replace(tzinfo=None) > since:
+            status["resolution"] = "Created"
+
+        for comment in comments:
+            when = datetime.datetime.strptime(comment.created, "%Y-%m-%dT%H:%M:%S.%f%z")
+            if when.replace(tzinfo=None) < since:
+                continue
+
+            status["comments"].append(comment.body)
+
+        for history in changelog.histories:
+            when = datetime.datetime.strptime(history.created, "%Y-%m-%dT%H:%M:%S.%f%z")
+            if when.replace(tzinfo=None) < since:
+                continue
+            for item in history.items:
+                if item.field == "resolution":
+                    status["resolution"] = item.toString
+
+        if len(status["comments"]) != 0 or status["resolution"]:
+            yield (status)
+
+
+def enumerate_pending(jira):
+    since = datetime.datetime.now() - datetime.timedelta(days=7)
+
+    jql = default_jql()
+    jql += "AND status = 'In Progress' \
+            AND issuetype != Initiative \
+            AND issuetype != Epic"
+    log.debug(jql)
+
+    my_issues = jira.search_issues(
+        jql, expand="changelog", fields="summary,assignee,created,components"
+    )
+    if my_issues.total > my_issues.maxResults:
+        my_issues = jira.search_issues(
+            jql,
+            expand="changelog",
+            fields="summary,assignee,created,components",
+            maxResults=my_issues.total,
+        )
+
+    for issue in my_issues:
+        status = {}
+        status["issue"] = str(issue)
+        if issue.fields.assignee:
+            status["assignee"] = issue.fields.assignee.displayName
+        else:
+            status["assignee"] = "Unassigned"
+        status["summary"] = issue.fields.summary
+        status["components"] = issue.fields.components
+
+        created = datetime.datetime.strptime(
+            issue.fields.created, "%Y-%m-%dT%H:%M:%S.%f%z"
+        )
+        status["new"] = created.replace(tzinfo=None) > since
+
+        yield (status)
+
 
-    if not os.path.isfile(new_issue_file):
-        sys.exit(-1)
+################################################################################
+# Argument parser
+################################################################################
+def get_parser():
+    """Takes care of script argument parsing."""
+    parser = ArgumentParser(description="Script used to update comments in Jira")
 
-    log.debug("Using issue file: %s" % new_issue_file)
-    with open(new_issue_file, 'r') as yml:
-        yml_issues = yaml.load(yml, Loader=yaml.FullLoader)
+    parser.add_argument(
+        "--test",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Use the test server",
+    )
+
+    parser.add_argument(
+        "-u",
+        "--user",
+        required=False,
+        action="append",
+        default=None,
+        help="Query Jira with another Jira username \
+            (first.last or first.last@linaro.org)",
+    )
+
+    parser.add_argument(
+        "-p",
+        "--project",
+        required=False,
+        action="store",
+        default=None,
+        type=str.upper,
+        help="Query Jira for only a specifc project",
+    )
+
+    parser.add_argument(
+        "-t",
+        "--team",
+        required=False,
+        action="store",
+        default=None,
+        type=str.lower,
+        help="Query Jira for only issues assigned to members of a specific tema (eg. linaro-landing-team-qualcomm)",
+    )
+
+    parser.add_argument(
+        "--days",
+        required=False,
+        action="store",
+        default=7,
+        help="Period of the report in days",
+    )
+
+    parser.add_argument(
+        "--html",
+        required=False,
+        nargs="?",
+        action="store",
+        const="status.html",
+        help="Store output to HTML file",
+    )
+
+    parser.add_argument(
+        "--version", action="version", version=f"%(prog)s, {__version__}"
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Output some verbose debugging info",
+    )
 
-    return yml_issues
+    return parser
 
 
 def initialize_logger(args):
-    LOG_FMT = ("[%(levelname)s] %(funcName)s():%(lineno)d   %(message)s")
+    LOG_FMT = "[%(levelname)s] %(funcName)s():%(lineno)d   %(message)s"
     lvl = log.ERROR
-    if args.v:
+    if args.verbose:
         lvl = log.DEBUG
 
     log.basicConfig(
         # filename="core.log",
         level=lvl,
         format=LOG_FMT,
-        filemode='w')
+        filemode="w",
+    )
 
 
-jira_field_to_yaml = {
-        'issuetype' : 'IssueType',
-        'project' : 'Project',
-        'summary' : 'Summary',
-        'description' : 'Description',
-        'assignee' : 'AssigneeEmail',
-        'customfield_10014' : 'EpicLink',
-        'customfield_10104' : 'ClientStakeholder',
-        'timetracking' : 'OriginalEstimate',
-        'components' : 'Components',
-        'customfield_10020' : 'Sprint',
-        'duedate' : 'Due date',
-        'customfield_10011' : 'Epic Name',
-        'customfield_10034' : 'Share Visibility',
-        }
+################################################################################
+# Template for outout
+################################################################################
+output = """
+{%- for assignee in assignees %}
+{{assignee}}:
+{%- for issue in updates | selectattr('assignee', 'equalto', assignee) | list %}
+{%- if loop.index == 1 %}
+ * Past
+{%- endif %}
+   * [{{issue['issue']}}]{% if issue['components'] |length > 0 %} [{{issue['components']|join(',')}}]{% endif %} {{issue['summary']}} {% if issue['resolution'] %}- was {{issue['resolution']|lower}}{% endif %}
+  {%- for c in issue['comments'] %}
+    {%- for cc in c.splitlines() %}
+    {% if loop.index == 1 %} *{% else %}  {% endif %} {{cc}}
+    {%- endfor %}
+  {%- endfor %}
+{%- endfor %}
+{%- for issue in pendings | selectattr('assignee', 'equalto', assignee) | list %}
+{%- if loop.index == 1 %}
+ * Ongoing
+{%- endif %}
+   * [{{issue['issue']}}]{% if issue['components'] |length > 0 %} [{{issue['components']|join(',')}}]{% endif %} {{issue['summary']}}
+ {%- endfor %}
+{% endfor %}
+"""
+
+output_html = """
+<html>
+<body>
+{%- for assignee in assignees %}
+{{assignee}}:
+<ul>
+{%- for issue in updates | selectattr('assignee', 'equalto', assignee) | list %}
+{%- if loop.index == 1 %}
+<li>Past</li>
+    <ul>
+{%- endif %}
+        <li>[<a href="{{url}}/browse/{{issue['issue']}}">{{issue['issue']}}</a>]{% if issue['components'] |length > 0 %} [{{issue['components']|join(',')}}]{% endif %} {{issue['summary']}} {% if issue['resolution'] %} - was {{issue['resolution']|lower}}{% endif %}</li>
+        {%- for c in issue['comments'] %}
+        {%- if loop.index == 1 %}
+            <ul>
+        {%- endif %}
+                <li>{{'<br>'.join(c.splitlines())}}</li>
+        {%- if loop.index == loop.length %}
+            </ul>
+        {%- endif %}
+        {%- endfor %}
+{%- if loop.index == loop.length %}
+    </ul>
+{%- endif %}
+{%- endfor %}
+{%- for issue in pendings | selectattr('assignee', 'equalto', assignee) | list %}
+{%- if loop.index == 1 %}
+<li>Ongoing</li>
+    <ul>
+{%- endif %}
+        <li>[<a href="{{url}}/browse/{{issue['issue']}}">{{issue['issue']}}</a>]{% if issue['components'] |length > 0 %} [{{issue['components']|join(',')}}]{% endif %} {{issue['summary']}}</li>
+{%- if loop.index == loop.length %}
+    </ul>
+{%- endif %}
+{%- endfor %}
+</ul>
+{% endfor %}
+</body>
+</html>
+"""
+
 
 ################################################################################
 # Main function
 ################################################################################
 def main():
     argv = sys.argv
     parser = get_parser()
-    created_cards = {}
 
     # The parser arguments (cfg.args) are accessible everywhere after this call.
     cfg.args = parser.parse_args()
 
     initialize_logger(cfg.args)
 
     # This initiates the global yml configuration instance so it will be
     # accessible everywhere after this call.
     cfg.initiate_config()
 
-    if not cfg.args.file:
-        log.error("No file provided\n")
-        parser.print_help()
-        sys.exit(os.EX_USAGE)
-
-    jira, username = jiralogin.get_jira_instance(False)
-
-    if cfg.args.file is not None:
-        filename = cfg.args.file
-        issues = parse_issue_file(filename)
-        for issue in issues:
-            # We should only find one project and one issue type otherwise something is wrong
-            issue_fields_dict = {}
-            try:
-                issue_meta_data = jira.createmeta(projectKeys=issue['Project'], issuetypeNames=issue['IssueType'], expand='projects.issuetypes.fields')
-                issue_fields_dict = issue_meta_data['projects'][0]['issuetypes'][0]['fields']
-                log.debug(f"Project: {issue['Project']}")
-                log.debug(f"IssueType: {issue['IssueType']}")
-                log.debug(f"issue fields dict: {issue_fields_dict}")
-            except (IndexError, KeyError):
-                print(f"Please specify 'Project' and 'IssueType'.")
-
-            if issue_fields_dict:
-                fields = {
-                    'project': {'key': issue['Project']},
-                    'issuetype': {'name': issue['IssueType']},
-                }
-
-                if 'Summary' in issue.keys():
-                    fields['summary'] = issue['Summary']
-
-                if 'Description' in issue.keys():
-                    fields['description'] = issue['Description']
-
-                if 'OriginalEstimate' in issue.keys():
-                    fields['timetracking'] = {'originalEstimate': issue['OriginalEstimate']}
-
-                if 'AssigneeEmail' in issue.keys():
-                    assignee = jira.search_assignable_users_for_issues(query=issue['AssigneeEmail'], project=issue['Project'])
-                    log.debug(f"Assignee email: {issue['AssigneeEmail']}")
-                    log.debug(f"Assignee: {assignee}")
-                    # We assume that the first entry in the returned user array is the one we want
-                    if len(assignee) > 0:
-                        fields['assignee'] = {'id': assignee[0].accountId}
-
-                if 'EpicLink' in issue.keys():
-                    if issue['EpicLink'] in created_cards.keys():
-                        fields['customfield_10014'] = created_cards[issue['EpicLink']]
-                    else:
-                        fields['customfield_10014'] = issue['EpicLink']
-
-                if 'ClientStakeholder' in issue.keys():
-                    csh_fields_dict = issue_meta_data['projects'][0]['issuetypes'][0]['fields']['customfield_10104']['allowedValues']
-                    for s in csh_fields_dict:
-                        if s['value'] == issue['ClientStakeholder']:
-                            fields['customfield_10104'] = [{'self':s['self'], 'value': s['value'], 'id': str(s['id'])}]
-
-                if 'Components' in issue.keys():
-                    components = jira.project_components(issue['Project'])
-                    comparr = []
-                    for c in components:
-                        for comp in issue['Components'].split(','):
-                            if c.name == comp.strip():
-                                comparr.append({'id': str(c.id)})
-                    if len(comparr) > 0:
-                        fields['components'] = comparr
-
-                sprint_found = True  # Only indicate sprint not found in case a sprint has been specified.
-                if 'Sprint' in issue.keys():
-                    sprint_found = False
-                    boards_in_project = jira.boards(projectKeyOrID=issue['Project'])
-                    log.debug(f"Boards:")
-                    for board in boards_in_project:
-                        log.debug(f"* {board}")
-                        sprints_in_board = jira.sprints(board_id=board.id)
-                        log.debug(f" + Sprints:")
-                        for sprint in sprints_in_board:
-                            log.debug(f"  - {sprint}")
-                            if sprint.name == issue['Sprint']:
-                                fields['customfield_10020'] = sprint.id
-                                sprint_found = True
-
-                if 'Due date' in issue.keys():
-                    fields['duedate'] = str(issue['Due date'])
-
-                if 'IssueType' in issue.keys() and issue['IssueType'] == 'Epic':
-                    if 'Epic Name' in issue.keys():
-                        fields['customfield_10011'] = issue['Epic Name']
-                    else:
-                        fields['customfield_10011'] = issue['Summary']
-
-                if 'Share Visibility' in issue.keys():
-                    share_visibility = []
-                    for shared_with in issue['Share Visibility']:
-                        tmp_share = jira.search_assignable_users_for_issues(query=shared_with, project=issue['Project'])[0]
-                        share_visibility.append({'id': tmp_share.accountId})
-                    log.debug(f"shared with: {issue['Share Visibility']}")
-                    log.debug(f"share_visibility: {share_visibility}")
-                    # We assume that the first entry in the returned user array is the one we want
-                    if len(share_visibility) > 0:
-                        fields['customfield_10034'] = share_visibility
-
-                if sprint_found:
-                    # Check if all feilds are possible to set in this issuetype and project.
-                    for field in fields.keys():
-                        if field not in issue_fields_dict.keys():
-                            print(f"Field {field} set by script but not possible for issuetype and project in Jira.")
-                            sys.exit(os.EX_USAGE)
-
-                    # Check fields required by Jira.
-                    for field in issue_fields_dict.keys():
-                        if issue_fields_dict[field]['required'] and not issue_fields_dict[field]['hasDefaultValue']:
-                            if field not in fields.keys():
-                                print(f"Field {jira_field_to_yaml[field]} required but not set.")
-                                sys.exit(os.EX_USAGE)
-
-                    if cfg.args.dry_run:
-                        print(f"This issue would have been created when running without '--dry-run':")
-                        created_cards [ issue['Summary'] ] = f"new_issue, {issue['Summary']}"
-                        for field in fields.keys():
-                            print(f"{field}: {fields[field]}")
-                    else:
-                        server = cfg.get_server()
-                        new_issue = jira.create_issue(fields=fields)
-                        created_cards [ issue['Summary'] ] = str(new_issue)
-                        print(f"New issue created: {server.get('url')}/browse/{new_issue}")
-                else:
-                    print('Sprint \"' + issue['Sprint'] + '\" not found in project ' + issue['Project'])
-    else:
-        log.error("Trying to run script with unsupported configuration. Try using --help.")
-        sys.exit(os.EX_USAGE)
+    jira, username = jiralogin.get_jira_instance(cfg.args.test)
+
+    if cfg.args.user is None:
+        cfg.args.user = [username]
+
+    updates = list(enumerate_updates(jira))
+    pendings = list(enumerate_pending(jira))
+
+    assignees = sorted(
+        set([u["assignee"] for u in updates]) | set([p["assignee"] for p in pendings])
+    )
+    # Move "Unassigned" issues to the end
+    assignees.sort(key="Unassigned".__eq__)
+
+    template = Template(output)
+    print(
+        template.render(
+            assignees=assignees,
+            updates=updates,
+            pendings=pendings,
+            url=jira.client_info(),
+        )
+    )
+
+    if cfg.args.html:
+        f = open(cfg.args.html, "w")
+        template = Template(output_html)
+        f.write(
+            template.render(
+                assignees=assignees,
+                updates=updates,
+                pendings=pendings,
+                url=jira.client_info(),
+            )
+        )
+        f.close()
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `jipdate-2.0.1/jipdate/jipdate.py` & `jipdate-2.0.2/jipdate/jipdate.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 import sys
 import tempfile
 import yaml
 
 # Local files
 from jipdate import cfg
 from jipdate import jiralogin
+from jipdate import __version__
+
 
 ################################################################################
 # Helper functions
 ################################################################################
 def print_status(status):
-    """ Helper function printing your status """
+    """Helper function printing your status"""
     print("This is your status:")
     print("\n---\n")
-    print("\n".join(l.strip('\n') for l in status))
+    print("\n".join(l.strip("\n") for l in status))
 
 
 def open_editor(filename):
     """
     Function that tries to find the best suited editor to use and then
     opens the status file in the editor.
     """
     if "EDITOR" in os.environ:
-        editor = os.environ['EDITOR']
+        editor = os.environ["EDITOR"]
     elif "VISUAL" in os.environ:
-        editor = os.environ['VISUAL']
+        editor = os.environ["VISUAL"]
     elif os.path.exists("/usr/bin/editor"):
         editor = "/usr/bin/editor"
     elif os.path.exists("/usr/bin/vim"):
         editor = "/usr/bin/vim"
     elif os.path.exists("/usr/bin/vi"):
         editor = "/usr/bin/vi"
     else:
@@ -52,129 +54,197 @@
     This will open the user provided file and if there has not been any file
     provided it will create and open a temporary file instead.
     """
     log.debug("filename: %s\n" % filename)
     if filename:
         return open(filename, "w")
     else:
-        return tempfile.NamedTemporaryFile(mode='w+t', delete=False)
+        return tempfile.NamedTemporaryFile(mode="w+t", delete=False)
 
 
 def add_domain(user):
     """
     Helper function that appends @linaro.org to the username. It does nothing if
     it is already included.
     """
-    if '@' not in user:
+    if "@" not in user:
         user = user + "@linaro.org"
     return user
 
 
 def email_to_name(email):
-    """ Converts 'first.last@linaro.org' to 'First Last'. """
+    """Converts 'first.last@linaro.org' to 'First Last'."""
     n = email.split("@")[0].title()
     return n.replace(".", " ")
 
+
 ################################################################################
 # Argument parser
 ################################################################################
 def get_parser():
-    """ Takes care of script argument parsing. """
-    parser = ArgumentParser(description='Script used to update comments in Jira')
+    """Takes care of script argument parsing."""
+    parser = ArgumentParser(description="Script used to update comments in Jira")
 
-    parser.add_argument('-e', required=False, action="store_true", \
-            default=False, \
-            help='Only include epics (no initiatives or stories). Used in combination \
-            with "-q"')
-
-    parser.add_argument('-f', '--file', required=False, action="store", \
-            default=None, \
-            help='Load status update from FILE.  NOTE: -q will overwrite the \
-            content of FILE')
-
-    parser.add_argument('-l', required=False, action="store_true", \
-            default=False, \
-            help='Get the last comment from Jira')
-
-    parser.add_argument('-p', required=False, action="store_true", \
-            default=False, \
-            help='Print Jira query result to stdout (no editor or jira updates)')
-
-    parser.add_argument('-q', required=False, action="store_true", \
-            default=False, \
-            help='Query Jira for issue(s) assigned to you')
-
-    parser.add_argument('-s', required=False, action="store_true", \
-            default=False, \
-            help='Be silent, only show jira updates and not entire status file')
-
-    parser.add_argument('-t', required=False, action="store_true", \
-            default=False, \
-            help='Use the test server')
-
-    parser.add_argument('-u', '--user', required=False, action="store", \
-            default=None, \
-            help='Query Jira with another Jira username \
-            (first.last or first.last@linaro.org)')
-
-    parser.add_argument('-v', required=False, action="store_true", \
-            default=False, \
-            help='Output some verbose debugging info')
-
-    parser.add_argument('-x', required=False, action="store_true", \
-            default=False, \
-            help='EXCLUDE stories and sub-tasks from gathered Jira issues. Used in combination \
-            with "-q"')
-
-    parser.add_argument('--all', required=False, action="store_true", \
-            default=False, \
-            help='Load all Jira issues, not just the once marked in progress.')
-
-    parser.add_argument('--dry-run', required=False, action="store_true", \
-            default=False, \
-            help='Do not make any changes to JIRA')
+    parser.add_argument(
+        "-e",
+        required=False,
+        action="store_true",
+        default=False,
+        help='Only include epics (no initiatives or stories). Used in combination \
+            with "-q"',
+    )
+
+    parser.add_argument(
+        "-f",
+        "--file",
+        required=False,
+        action="store",
+        default=None,
+        help="Load status update from FILE.  NOTE: -q will overwrite the \
+            content of FILE",
+    )
+
+    parser.add_argument(
+        "-l",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Get the last comment from Jira",
+    )
+
+    parser.add_argument(
+        "-p",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Print Jira query result to stdout (no editor or jira updates)",
+    )
+
+    parser.add_argument(
+        "-q",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Query Jira for issue(s) assigned to you",
+    )
+
+    parser.add_argument(
+        "-s",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Be silent, only show jira updates and not entire status file",
+    )
+
+    parser.add_argument(
+        "-t",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Use the test server",
+    )
+
+    parser.add_argument(
+        "-u",
+        "--user",
+        required=False,
+        action="store",
+        default=None,
+        help="Query Jira with another Jira username \
+            (first.last or first.last@linaro.org)",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Output some verbose debugging info",
+    )
+
+    parser.add_argument(
+        "--version", action="version", version=f"%(prog)s, {__version__}"
+    )
+
+    parser.add_argument(
+        "-x",
+        required=False,
+        action="store_true",
+        default=False,
+        help='EXCLUDE stories and sub-tasks from gathered Jira issues. Used in combination \
+            with "-q"',
+    )
+
+    parser.add_argument(
+        "--all",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Load all Jira issues, not just the once marked in progress.",
+    )
+
+    parser.add_argument(
+        "--dry-run",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Do not make any changes to JIRA",
+    )
 
     return parser
 
+
 ################################################################################
 # Jira functions
 ################################################################################
 def update_jira(jira, i, c, t, ts=None):
     """
     This is the function that do the actual updates to Jira and in this case it
     is adding comments to a certain issue.
     """
-    if t['transition']:
-        if t['resolution']:
-            log.debug("Updating Jira issue: %s with transition: %s (%s)" %
-                   (i, t['transition'], t['resolution']))
-            jira.transition_issue(i, t['transition'], fields={'resolution':{'id': t['resolution']}})
+    if t["transition"]:
+        if t["resolution"]:
+            log.debug(
+                "Updating Jira issue: %s with transition: %s (%s)"
+                % (i, t["transition"], t["resolution"])
+            )
+            jira.transition_issue(
+                i, t["transition"], fields={"resolution": {"id": t["resolution"]}}
+            )
         else:
-            log.debug("Updating Jira issue: %s with transition: %s" % (i, t['transition']))
-            jira.transition_issue(i, t['transition'])
+            log.debug(
+                "Updating Jira issue: %s with transition: %s" % (i, t["transition"])
+            )
+            jira.transition_issue(i, t["transition"])
 
     if c != "":
         log.debug("Updating Jira issue: %s with comment:" % i)
-        log.debug("-- 8< --------------------------------------------------------------------------")
+        log.debug(
+            "-- 8< --------------------------------------------------------------------------"
+        )
         log.debug("%s" % c)
-        log.debug("-- >8 --------------------------------------------------------------------------\n\n")
+        log.debug(
+            "-- >8 --------------------------------------------------------------------------\n\n"
+        )
         jira.add_comment(i, c)
         if ts:
             jira.add_worklog(i, timeSpent=ts, comment=c)
 
 
 def write_last_jira_comment(f, jira, issue):
-    """ Pulls the last comment from Jira from an issue and writes it to the file
+    """Pulls the last comment from Jira from an issue and writes it to the file
     object.
     """
     c = jira.comments(issue)
     if len(c) > 0:
         try:
-            comment = "# Last comment:\n# ---8<---\n# %s\n# --->8---\n" % \
-                        "\n# ".join(c[-1].body.splitlines())
+            comment = "# Last comment:\n# ---8<---\n# %s\n# --->8---\n" % "\n# ".join(
+                c[-1].body.splitlines()
+            )
             f.write(comment)
         except UnicodeEncodeError:
             log.debug("Can't encode character")
 
 
 def get_jira_issues(jira, username):
     """
@@ -188,25 +258,25 @@
     user = cfg.args.user
     last_comment = cfg.args.l
 
     issue_types = ["Sub-task", "Epic"]
     if not epics_only:
         issue_types.append("Initiative")
         if not exclude_stories:
-            issue_types.extend(["Story", "Sub-task", "Bug"])
+            issue_types.extend(["Story", "Task", "Sub-task", "Bug"])
     issue_type = "issuetype in (%s)" % ", ".join(issue_types)
 
-    status = "status in (\"In Progress\")"
+    status = 'status in ("In Progress")'
     if all_status:
         status = "status not in (Resolved, Closed)"
 
     if user is None:
         user = "currentUser()"
     else:
-        user = "\"%s\"" % add_domain(user)
+        user = '"%s"' % add_domain(user)
 
     jql = "%s AND assignee = %s AND %s" % (issue_type, user, status)
     log.debug(jql)
 
     my_issues = jira.search_issues(jql)
     if my_issues.total > my_issues.maxResults:
         my_issues = jira.search_issues(jql, maxResults=my_issues.total)
@@ -224,16 +294,18 @@
     f.write(subject)
 
     f.write(msg)
     log.debug("Found issue:")
     for issue in my_issues:
         log.debug("%s : %s" % (issue, issue.fields.summary))
 
-        if (merge_issue_header()):
-            f.write("[%s%s%s]\n" % (issue, get_header_separator(), issue.fields.summary))
+        if merge_issue_header():
+            f.write(
+                "[%s%s%s]\n" % (issue, get_header_separator(), issue.fields.summary)
+            )
         else:
             f.write("[%s]\n" % issue)
             f.write("# Header: %s\n" % issue.fields.summary)
 
         f.write("# Type: %s\n" % issue.fields.issuetype)
         f.write("# Status: %s\n" % issue.fields.status)
         f.write(get_extra_comments())
@@ -242,21 +314,27 @@
         f.write("\n")
 
     f.close()
     return (filename, my_issues)
 
 
 def should_update():
-    """ A yes or no dialogue. """
+    """A yes or no dialogue."""
     while True:
         server = cfg.get_server()
-        print("Server to update: %s\n" % server.get('url'));
-        answer = input("Are you sure you want to update Jira with the " +
-                           "information above? [y/n] ").lower().strip()
-        if answer in set(['y', 'n']):
+        print("Server to update: %s\n" % server.get("url"))
+        answer = (
+            input(
+                "Are you sure you want to update Jira with the "
+                + "information above? [y/n] "
+            )
+            .lower()
+            .strip()
+        )
+        if answer in set(["y", "n"]):
             return answer
         else:
             print("Incorrect input: %s" % answer)
 
 
 def parse_status_file(jira, filename, issues):
     """
@@ -279,31 +357,31 @@
 
     # Regexp to mach a tag that indicates to stop processing completely:
     # [FIN]
     regex_fin = r"^\[FIN\]\n$"
 
     # Regexp to match for a status update, this will remove 'Status' from the
     # match:
-    regex_status = r'(?:^Status:) *(.+)\n$'
+    regex_status = r"(?:^Status:) *(.+)\n$"
 
     # Contains the status text, it could be a file or a status email
     status = ""
 
     # Regexp to match for a time spent update, this will remove 'Time spent:'
     # from the match:
-    regex_timespent = r'(^Time spent:) \d+\w\n$'
+    regex_timespent = r"(^Time spent:) \d+\w\n$"
 
     # List of resolutions (when doing a transition to Resolved). Query once globally.
     resolution_map = dict([(t.name.title(), t.id) for t in jira.resolutions()])
 
     with open(filename) as f:
         status = f.readlines()
 
-    myissue = "";
-    mycomment = "";
+    myissue = ""
+    mycomment = ""
 
     # build list of {issue,comment} tuples found in status
     issue_comments = []
     for line in status:
         # New issue?
         match = re.search(regex, line)
 
@@ -324,17 +402,17 @@
 
             # IndexError: we had fetched already, but issue is not found
             # TypeError: issues is None, we haven't queried Jira yet, at all
             except (IndexError, TypeError) as e:
                 try:
                     issue = jira.issue(myissue)
                     issue_comments.append((issue, "", "", None))
-                except  Exception as e:
-                    if 'Issue Does Not Exist' in e.text:
-                        print('[{}] :  {}'.format(myissue, e.text))
+                except Exception as e:
+                    if "Issue Does Not Exist" in e.text:
+                        print("[{}] :  {}".format(myissue, e.text))
                         validissue = False
 
         # Stop parsing entirely.  This needs to be placed before regex_stop
         # or the .* will match and [FIN] won't be processed
         elif re.search(regex_fin, line):
             break
         # If we have non-JIRA issue tags, stop parsing until we find a valid tag
@@ -343,161 +421,189 @@
         elif transition and validissue:
             # If we have a match, then the new status should be first in the
             # group. Jira always expect the name of the state transitions to be
             # word capitalized, hence the call to the title() function. This
             # means that it doesn't matter if the user enter all lower case,
             # mixed or all upper case. All of them will work.
             new_status = transition.groups()[0].title()
-            (i,c,_,ts) = issue_comments[-1]
+            (i, c, _, ts) = issue_comments[-1]
             issue_comments[-1] = (i, c, new_status, ts)
         elif re.search(regex_timespent, line, re.IGNORECASE):
-            timespent = line.split(':')[1].strip()
-            (i,c,t,_) = issue_comments[-1]
+            timespent = line.split(":")[1].strip()
+            (i, c, t, _) = issue_comments[-1]
             issue_comments[-1] = (i, c, t, timespent)
         else:
             # Don't add lines with comments
-            if (line[0] != "#" and issue_comments and validissue):
-                (i,c,t,ts) = issue_comments[-1]
+            if line[0] != "#" and issue_comments and validissue:
+                (i, c, t, ts) = issue_comments[-1]
                 issue_comments[-1] = (i, c + line, t, ts)
 
     issue_upload = []
     print("These JIRA cards will be updated as follows:\n")
-    for (idx,t) in enumerate(issue_comments):
-        (issue,comment,transition,timespent) = issue_comments[idx]
+    for idx, t in enumerate(issue_comments):
+        (issue, comment, transition, timespent) = issue_comments[idx]
 
         # Strip beginning  and trailing blank lines
-        comment = comment.strip('\n')
+        comment = comment.strip("\n")
 
         # initialize here to avoid unassigned variables and useless code complexity
         resolution_id = transition_id = None
         resolution = transition_summary = ""
 
         if transition != "" and transition != str(issue.fields.status):
             # An optional 'resolution' attribute can be set when doing a transition
             # to Resolved, using the following pattern: Resolved / <resolution>
-            if (transition.startswith('Resolved') or transition.startswith('Closed')) and '/' in transition:
-                (transition, resolution) = map(str.strip, transition.split('/'))
+            if (
+                transition.startswith("Resolved") or transition.startswith("Closed")
+            ) and "/" in transition:
+                (transition, resolution) = map(str.strip, transition.split("/"))
                 if not resolution in resolution_map:
-                    print("Invalid resolution \"{}\" for issue {}".format(resolution, issue))
+                    print(
+                        'Invalid resolution "{}" for issue {}'.format(resolution, issue)
+                    )
                     print("Possible resolution: {}".format([t for t in resolution_map]))
                     sys.exit(1)
                 resolution_id = resolution_map[resolution]
 
-            transition_map = dict([(t['name'].title(), t['id']) for t in jira.transitions(issue)])
+            transition_map = dict(
+                [(t["name"].title(), t["id"]) for t in jira.transitions(issue)]
+            )
             if not transition in transition_map:
-                print("Invalid transition \"{}\" for issue {}".format(transition, issue))
+                print('Invalid transition "{}" for issue {}'.format(transition, issue))
                 print("Possible transitions: {}".format([t for t in transition_map]))
                 sys.exit(1)
 
             transition_id = transition_map[transition]
             if resolution:
-                transition_summary = " %s => %s (%s)" % (issue.fields.status, transition, resolution)
+                transition_summary = " %s => %s (%s)" % (
+                    issue.fields.status,
+                    transition,
+                    resolution,
+                )
             else:
                 transition_summary = " %s => %s" % (issue.fields.status, transition)
 
         if comment == "" and not transition_id:
-            log.debug("Issue [%s] has no comment or transitions, not updating the issue" % (issue))
+            log.debug(
+                "Issue [%s] has no comment or transitions, not updating the issue"
+                % (issue)
+            )
             continue
 
-        issue_upload.append((issue, comment,
-                             {'transition': transition_id, 'resolution': resolution_id}, timespent))
-        print("[%s]%s\n  %s" % (issue, transition_summary, "\n  ".join(comment.splitlines())))
-        if timespent: print(" Time spent: %s" % timespent)
+        issue_upload.append(
+            (
+                issue,
+                comment,
+                {"transition": transition_id, "resolution": resolution_id},
+                timespent,
+            )
+        )
+        print(
+            "[%s]%s\n  %s"
+            % (issue, transition_summary, "\n  ".join(comment.splitlines()))
+        )
+        if timespent:
+            print(" Time spent: %s" % timespent)
     print("")
 
     issue_comments = issue_upload
     if issue_comments == [] or cfg.args.dry_run or should_update() == "n":
         if issue_comments == []:
             print("No change, Jira was not updated!\n")
         else:
             print("Comments will not be written to Jira!\n")
         if not cfg.args.s:
             print_status(status)
         sys.exit()
 
     # if we found something, let's update jira
-    for (issue,comment,transition,timespent) in issue_comments:
+    for issue, comment, transition, timespent in issue_comments:
         update_jira(jira, issue, comment, transition, timespent)
 
     print("Successfully updated your Jira tickets!\n")
     if not cfg.args.s:
         print_status(status)
 
+
 def print_status_file(filename):
-    with open(filename, 'r') as f:
+    with open(filename, "r") as f:
         print(f.read())
 
+
 ################################################################################
 # Yaml
 ################################################################################
 
 
 def get_extra_comments():
-    """ Read the jipdate config file and return all option comments. """
+    """Read the jipdate config file and return all option comments."""
     try:
-        yml_iter = cfg.yml_config['comments']
+        yml_iter = cfg.yml_config["comments"]
     except:
         # Probably no "comments" section in the yml-file.
         return "\n"
 
     return ("\n".join(yml_iter) + "\n") if yml_iter is not None else "\n"
 
+
 def get_header():
-    """ Read the jipdate config file and return all option header. """
+    """Read the jipdate config file and return all option header."""
     try:
-        yml_iter = cfg.yml_config['header']
+        yml_iter = cfg.yml_config["header"]
     except:
         # Probably no "comments" section in the yml-file.
         return ""
 
     return ("\n".join(yml_iter) + "\n\n") if yml_iter is not None else "\n"
 
 
 def merge_issue_header():
-    """ Read the configuration flag which decides if the issue and issue header
-    shall be combined. """
+    """Read the configuration flag which decides if the issue and issue header
+    shall be combined."""
     try:
-        yml_iter = cfg.yml_config['use_combined_issue_header']
+        yml_iter = cfg.yml_config["use_combined_issue_header"]
     except:
         # Probably no "use_combined_issue_header" section in the yml-file.
         return False
     return yml_iter
 
 
 def get_header_separator():
-    """ Read the separator from the jipdate config file. """
+    """Read the separator from the jipdate config file."""
     try:
-        yml_iter = cfg.yml_config['separator']
+        yml_iter = cfg.yml_config["separator"]
     except:
         # Probably no "separator" section in the yml-file.
         return " | "
     return yml_iter
 
 
 def get_editor():
-    """ Read the configuration flag that will decide whether to show the text
-    editor by default or not. """
+    """Read the configuration flag that will decide whether to show the text
+    editor by default or not."""
     try:
-        yml_iter = cfg.yml_config['text-editor']
+        yml_iter = cfg.yml_config["text-editor"]
     except:
         # Probably no "text-editor" section in the yml-file.
         return True
     return yml_iter
 
+
 def initialize_logger(args):
-    LOG_FMT = ("[%(levelname)s] %(funcName)s():%(lineno)d   %(message)s")
+    LOG_FMT = "[%(levelname)s] %(funcName)s():%(lineno)d   %(message)s"
     lvl = log.ERROR
-    if args.v:
+    if args.verbose:
         lvl = log.DEBUG
 
     log.basicConfig(
         # filename="core.log",
         level=lvl,
         format=LOG_FMT,
-        filemode='w')
+        filemode="w",
+    )
 
 
 ################################################################################
 # Main function
 ################################################################################
 def main():
     argv = sys.argv
@@ -533,23 +639,26 @@
 
         if cfg.args.p:
             print_status_file(filename)
             sys.exit(os.EX_OK)
     elif cfg.args.file is not None:
         filename = cfg.args.file
     else:
-        log.error("Trying to run script with unsupported configuration. Try using --help.")
+        log.error(
+            "Trying to run script with unsupported configuration. Try using --help."
+        )
         sys.exit(os.EX_USAGE)
 
     if get_editor():
         open_editor(filename)
 
     try:
         issues
     # issues is not defined, we haven't made any query yet.
     except NameError:
         parse_status_file(jira, filename, None)
     else:
         parse_status_file(jira, filename, issues)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `jipdate-2.0.1/jipdate/jipfp.py` & `jipdate-2.0.2/jipdate/jipfp.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 import sys
 import unicodedata
 import yaml
 
 # Local files
 from jipdate import cfg
 from jipdate import jiralogin
+from jipdate import __version__
+
 
 ################################################################################
 # Class node
 ################################################################################
-class Node():
+class Node:
     """A node representing an issue in Jira"""
+
     def __init__(self, key, summary, issuetype):
         """Return a node containing the must have feature to be represented in a
         tree."""
         self.key = key
         self.summary = summary
         # Take care of some characters not supported in xml
-        self.summary = self.summary.replace("\"", "'")
+        self.summary = self.summary.replace('"', "'")
         self.summary = self.summary.replace("&", "and")
         self.issuetype = issuetype
         self.assignee = None
         self.sponsors = []
         self.description = None
         self.parent = None
         self.childrens = []
@@ -37,16 +40,24 @@
         self.color = None
         self.base_url = None
 
         self._indent = 0
         self._sortval = 3
 
     def __str__(self):
-        s =  "%s%s: %s [%s]\n"              % (" " * self._indent, self.key, self.summary, self.issuetype)
-        s += "%s     |   sponsors:    %s\n" % (" " * self._indent, ", ".join(self.sponsors))
+        s = "%s%s: %s [%s]\n" % (
+            " " * self._indent,
+            self.key,
+            self.summary,
+            self.issuetype,
+        )
+        s += "%s     |   sponsors:    %s\n" % (
+            " " * self._indent,
+            ", ".join(self.sponsors),
+        )
         s += "%s     |   assignee:    %s\n" % (" " * self._indent, self.assignee)
         s += "%s     |   description: %s\n" % (" " * self._indent, self.description)
         s += "%s     |   parent:      %s\n" % (" " * self._indent, self.parent)
         s += "%s     |   state:       %s\n" % (" " * self._indent, self.state)
         s += "%s     |   url:         %s\n" % (" " * self._indent, self.get_url())
         s += "%s     |-> color:       %s\n" % (" " * self._indent, self.get_color())
         return s
@@ -77,22 +88,22 @@
     def get_sponsor(self, sponsor):
         return self.sponsors
 
     def add_description(self, description):
         self.description = description
 
     def get_description(self, description):
-        #try:
+        # try:
         #    f.write("<richcontent TYPE=\"DETAILS\" HIDDEN=\"true\"\n>")
         #    f.write("<html>\n<head>\n</head>\n<body>\n<p>\n")
         #    f.write(issue.fields.description)
-        #except UnicodeEncodeError:
+        # except UnicodeEncodeError:
         #    vprint("UnicodeEncodeError in description in %s" % str(issue))
         #    f.write("Unicode error in description, please go to Jira\n")
-        #f.write("\n</p>\n</body>\n</html>\n</richcontent>\n")
+        # f.write("\n</p>\n</body>\n</html>\n</richcontent>\n")
         return self.description
 
     def add_parent(self, key):
         self.parent = key
 
     def get_parent(self):
         return self.key
@@ -117,19 +128,19 @@
     def set_color(self, color):
         self.color = color
 
     def get_color(self):
         if self.color is not None:
             return self.color
 
-        color = "#990000" # Red
+        color = "#990000"  # Red
         if self.state == "In Progress":
-            color = "#009900" # Green
+            color = "#009900"  # Green
         elif self.state in ["Blocked", "To Do"]:
-            color = "#ff6600" # Orange
+            color = "#ff6600"  # Orange
         return color
 
     def set_base_url(self, base_url):
         self.base_url = base_url
 
     def get_url(self):
         if self.base_url is not None:
@@ -152,43 +163,50 @@
 
         if cfg.args.s and self.issuetype == "Epic":
             fold = "false"
 
         if cfg.args.i and self.issuetype == "Initiative":
             fold = "true"
 
-        xml_start = "%s<node LINK=\"%s\" TEXT=\"%s/%s: %s\" FOLDED=\"%s\" COLOR=\"%s\">\n" % \
-                (" " * self._indent,
-                 self.get_url(),
-                 self._short_type(),
-                 self.key,
-                 self.summary,
-                 fold,
-                 self.get_color())
+        xml_start = '%s<node LINK="%s" TEXT="%s/%s: %s" FOLDED="%s" COLOR="%s">\n' % (
+            " " * self._indent,
+            self.get_url(),
+            self._short_type(),
+            self.key,
+            self.summary,
+            fold,
+            self.get_color(),
+        )
         f.write(xml_start)
 
         # Info start
-        xml_info_start = "%s<node TEXT=\"info\" FOLDED=\"true\" COLOR=\"#000000\">\n" % \
-                (" " * (self._indent + 4))
+        xml_info_start = '%s<node TEXT="info" FOLDED="true" COLOR="#000000">\n' % (
+            " " * (self._indent + 4)
+        )
         f.write(xml_info_start)
 
         # Assignee, single node
-        xml_assignee = "%s<node TEXT=\"Assignee: %s\" FOLDED=\"false\" COLOR=\"#000000\"/>\n" % \
-                (" " * (self._indent + 8),
-                        self.assignee)
+        xml_assignee = (
+            '%s<node TEXT="Assignee: %s" FOLDED="false" COLOR="#000000"/>\n'
+            % (" " * (self._indent + 8), self.assignee)
+        )
         f.write(xml_assignee)
 
         # Sponsors
-        xml_sponsor_start = "%s<node TEXT=\"Sponsors\" FOLDED=\"false\" COLOR=\"#000000\">\n" % \
-                (" " * (self._indent + 8))
+        xml_sponsor_start = (
+            '%s<node TEXT="Sponsors" FOLDED="false" COLOR="#000000">\n'
+            % (" " * (self._indent + 8))
+        )
         f.write(xml_sponsor_start)
 
         for s in self.sponsors:
-            xml_sponsor = "%s<node TEXT=\"%s\" FOLDED=\"false\" COLOR=\"#000000\"/>\n" % \
-                    (" " * (self._indent + 12), s)
+            xml_sponsor = '%s<node TEXT="%s" FOLDED="false" COLOR="#000000"/>\n' % (
+                " " * (self._indent + 12),
+                s,
+            )
             f.write(xml_sponsor)
 
         # Sponsors end
         xml_sponsor_end = "%s%s" % (" " * (self._indent + 8), "</node>\n")
         f.write(xml_sponsor_end)
 
         # Info end
@@ -199,88 +217,138 @@
         for c in sorted(self.childrens):
             c.to_xml(f, self._indent + 4)
 
         # Add the closing element
         xml_end = "%s%s" % (" " * self._indent, "</node>\n")
         f.write(xml_end)
 
+
 def open_file(filename):
     """
     This will open the user provided file and if there has not been any file
     provided it will create and open a temporary file instead.
     """
     log.debug("filename: %s\n" % filename)
     if filename:
         return open(filename, "w")
     else:
         return tempfile.NamedTemporaryFile(delete=False)
 
+
 def get_parent_key(jira, issue):
     if hasattr(issue.fields, "customfield_10005"):
-        return getattr(issue.fields, "customfield_10005");
+        return getattr(issue.fields, "customfield_10005")
     return None
 
+
 ################################################################################
 # Argument parser
 ################################################################################
 def get_parser():
-    """ Takes care of script argument parsing. """
-    parser = ArgumentParser(description='Script used to generate Freeplane mindmap files')
-
-    parser.add_argument('-i', required=False, action="store_true", \
-            default=False, \
-            help='Show Initiatives only')
-
-    parser.add_argument('-p', '--project', required=False, action="store", \
-            default="SWG", \
-            help='Project type (SWG, VIRT, KWG etc)')
-
-    parser.add_argument('-s', required=False, action="store_true", \
-            default=False, \
-            help='Show stories also')
-
-    parser.add_argument('-t', required=False, action="store_true", \
-            default=False, \
-            help='Use the test server')
-
-    parser.add_argument('-v', required=False, action="store_true", \
-            default=False, \
-            help='Output some verbose debugging info')
-
-    parser.add_argument('--all', required=False, action="store_true", \
-            default=False, \
-            help='Load all Jira issues, not just the once marked in progress.')
-
-    parser.add_argument('--desc', required=False, action="store_true", \
-            default=False, \
-            help='Add description to the issues')
-
-    parser.add_argument('--test', required=False, action="store_true", \
-            default=False, \
-            help='Run test case and then exit')
+    """Takes care of script argument parsing."""
+    parser = ArgumentParser(
+        description="Script used to generate Freeplane mindmap files"
+    )
+
+    parser.add_argument(
+        "-i",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Show Initiatives only",
+    )
+
+    parser.add_argument(
+        "-p",
+        "--project",
+        required=False,
+        action="store",
+        default="SWG",
+        help="Project type (SWG, VIRT, KWG etc)",
+    )
+
+    parser.add_argument(
+        "-s",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Show stories also",
+    )
+
+    parser.add_argument(
+        "-t",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Use the test server",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Output some verbose debugging info",
+    )
+
+    parser.add_argument(
+        "--version", action="version", version=f"%(prog)s, {__version__}"
+    )
+
+    parser.add_argument(
+        "--all",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Load all Jira issues, not just the once marked in progress.",
+    )
+
+    parser.add_argument(
+        "--desc",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Add description to the issues",
+    )
+
+    parser.add_argument(
+        "--test",
+        required=False,
+        action="store_true",
+        default=False,
+        help="Run test case and then exit",
+    )
 
     return parser
 
+
 ################################################################################
 # General nodes
 ################################################################################
 def root_nodes_start(f, key):
-    f.write("<map version=\"freeplane 1.6.0\">\n")
-    f.write("<node LINK=\"%s\" TEXT=\"%s\" FOLDED=\"false\" COLOR=\"#000000\" LOCALIZED_STYLE_REF=\"AutomaticLayout.level.root\">\n"
-        % (cfg.server + "/projects/" + key, key))
+    f.write('<map version="freeplane 1.6.0">\n')
+    f.write(
+        '<node LINK="%s" TEXT="%s" FOLDED="false" COLOR="#000000" LOCALIZED_STYLE_REF="AutomaticLayout.level.root">\n'
+        % (cfg.server + "/projects/" + key, key)
+    )
+
 
 def root_nodes_end(f):
     f.write("</node>\n</map>")
 
+
 def orphan_node_start(f):
-    f.write("<node TEXT=\"Orphans\" POSITION=\"left\" FOLDED=\"false\" COLOR=\"#000000\">\n")
+    f.write('<node TEXT="Orphans" POSITION="left" FOLDED="false" COLOR="#000000">\n')
+
 
 def orphan_node_end(f):
     f.write("</node>\n")
 
+
 ################################################################################
 # Test
 ################################################################################
 def test():
     f = open_file("test" + ".mm")
     root_nodes_start(f, "Test")
     n1 = Node("SWG-1", "My issue 1", "Initiative")
@@ -321,29 +389,32 @@
     n1.add_child(n14)
 
     n1.gen_tree()
     n1.to_xml(f)
     root_nodes_end(f)
     f.close()
 
+
 ################################################################################
 # Stories
 ################################################################################
 def build_story_node(jira, story_key, d_handled=None, epic_node=None):
     si = jira.issue(story_key)
     if si.fields.status.name in ["Closed", "Resolved"]:
         d_handled[str(si.key)] = [None, si]
         return None
 
     # To prevent UnicodeEncodeError ignore unicode
-    summary = str(si.fields.summary.encode('ascii', 'ignore').decode())
+    summary = str(si.fields.summary.encode("ascii", "ignore").decode())
     story = Node(str(si.key), summary, str(si.fields.issuetype))
 
     try:
-        assignee = str(si.fields.assignee.displayName.encode('ascii', 'ignore').decode())
+        assignee = str(
+            si.fields.assignee.displayName.encode("ascii", "ignore").decode()
+        )
     except AttributeError:
         assignee = str(si.fields.assignee)
     story.add_assignee(assignee)
 
     story.set_state(str(si.fields.status.name))
     story.set_base_url(cfg.server)
 
@@ -373,34 +444,35 @@
 def build_epics_node(jira, epic_key, d_handled=None, initiative_node=None):
     ei = jira.issue(epic_key)
 
     if ei.fields.status.name in ["Closed", "Resolved"]:
         d_handled[str(ei.key)] = [None, ei]
         return None
 
-    summary = str(ei.fields.summary.encode('ascii', 'ignore').decode())
+    summary = str(ei.fields.summary.encode("ascii", "ignore").decode())
     epic = Node(str(ei.key), summary, str(ei.fields.issuetype))
 
     try:
-        assignee = str(ei.fields.assignee.displayName.encode('ascii', 'ignore').decode())
+        assignee = str(
+            ei.fields.assignee.displayName.encode("ascii", "ignore").decode()
+        )
     except AttributeError:
         assignee = str(ei.fields.assignee)
     epic.add_assignee(assignee)
 
     epic.set_state(str(ei.fields.status.name))
 
     try:
         sponsors = ei.fields.customfield_10101
         if sponsors is not None:
             for s in sponsors:
                 epic.add_sponsor(str(s.value))
     except AttributeError:
         epic.add_sponsor("No sponsor")
 
-
     epic.set_base_url(cfg.server)
 
     if initiative_node is not None:
         epic.add_parent(initiative_node.get_key())
         initiative_node.add_child(epic)
     else:
         # This cateches when people are not using implements/implemented by, but
@@ -421,27 +493,30 @@
         if "inwardIssue" in link.raw:
             story_key = str(link.inwardIssue.key)
             build_story_node(jira, story_key, d_handled, epic)
 
     print(epic)
     return epic
 
+
 ################################################################################
 # Initiatives
 ################################################################################
 def build_initiatives_node(jira, issue, d_handled):
     if issue.fields.status.name in ["Closed", "Resolved"]:
         d_handled[str(issue.key)] = [None, issue]
         return None
 
-    summary = str(issue.fields.summary.encode('ascii', 'ignore').decode())
+    summary = str(issue.fields.summary.encode("ascii", "ignore").decode())
     initiative = Node(str(issue.key), summary, str(issue.fields.issuetype))
 
     try:
-        assignee = str(issue.fields.assignee.displayName.encode('ascii', 'ignore').decode())
+        assignee = str(
+            issue.fields.assignee.displayName.encode("ascii", "ignore").decode()
+        )
     except AttributeError:
         assignee = str(issue.fields.assignee)
     initiative.add_assignee(assignee)
 
     initiative.set_state(str(issue.fields.status.name))
 
     sponsors = None
@@ -450,15 +525,15 @@
 
     if sponsors is not None:
         for s in sponsors:
             initiative.add_sponsor(str(s.value))
     initiative.set_base_url(cfg.server)
     print(initiative)
 
-    d_handled[initiative.get_key()] = [initiative, issue] # Initiative
+    d_handled[initiative.get_key()] = [initiative, issue]  # Initiative
 
     # Deal with Epics
     for link in issue.fields.issuelinks:
         if "inwardIssue" in link.raw:
             epic_key = str(link.inwardIssue.key)
             build_epics_node(jira, epic_key, d_handled, initiative)
 
@@ -514,37 +589,40 @@
     log.debug("Orphan Stories ...")
     for i in orphans_stories:
         node = build_story_node(jira, str(i.key), d_handled)
         nodes.append(node)
 
     return nodes
 
+
 ################################################################################
 # Config files
 ################################################################################
 def get_config_file():
-    """ Returns the location for the config file (including the path). """
+    """Returns the location for the config file (including the path)."""
     for d in cfg.config_locations:
         for f in [cfg.config_filename, cfg.config_legacy_filename]:
             checked_file = d + "/" + f
             if os.path.isfile(checked_file):
                 return d + "/" + f
 
+
 def initiate_config():
-    """ Reads the config file (yaml format) and returns the sets the global
+    """Reads the config file (yaml format) and returns the sets the global
     instance.
     """
     cfg.config_file = get_config_file()
     if not os.path.isfile(cfg.config_file):
         create_default_config()
 
     log.debug("Using config file: %s" % cfg.config_file)
-    with open(cfg.config_file, 'r') as yml:
+    with open(cfg.config_file, "r") as yml:
         cfg.yml_config = yaml.load(yml)
 
+
 ################################################################################
 # Main function
 ################################################################################
 def main():
     argv = sys.argv
     parser = get_parser()
 
@@ -562,43 +640,43 @@
         exit()
 
     jira, username = jiralogin.get_jira_instance(cfg.args.t)
 
     if cfg.args.project:
         key = cfg.args.project
 
-
     # Open and initialize the file
     f = open_file(key + ".mm")
     root_nodes_start(f, key)
 
     # Temporary dictorionary to keep track the data (issues) that we already
     # have dealt with.
     d_handled = {}
 
     # Build the main tree with Initiatives beloninging to the project.
     nodes = build_initiatives_tree(jira, key, d_handled)
 
     # Take care of the orphans, i.e., those who has no connection to any
     # initiative in your project.
-    nodes_orpans  = build_orphans_tree(jira, key, d_handled)
+    nodes_orpans = build_orphans_tree(jira, key, d_handled)
 
     # FIXME: We run through this once more since, when we run it the first time
     # we will catch Epics and Stories who are not linked with
     # "implements/implemented by" but instead uses the so called "Epic" link.
-    nodes_orpans  = build_orphans_tree(jira, key, d_handled)
+    nodes_orpans = build_orphans_tree(jira, key, d_handled)
 
     # Dump the main tree to file
     for n in sorted(nodes):
         n.to_xml(f)
 
     orphan_node_start(f)
     for n in sorted(nodes_orpans):
         n.to_xml(f)
     orphan_node_end(f)
 
     # End the file
     root_nodes_end(f)
     f.close()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `jipdate-2.0.1/jipdate/jiralogin.py` & `jipdate-2.0.2/jipdate/jiralogin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,83 +3,84 @@
 import logging as log
 import sys
 
 from jipdate import cfg
 from jira import JIRA
 from jira import JIRAError
 
+
 def get_username_from_config():
-    """ Get the username for Jira from the config file. """
+    """Get the username for Jira from the config file."""
     username = None
     # First check if the username is in the config file.
     try:
-        username = cfg.yml_config['username']
+        username = cfg.yml_config["username"]
     except:
         log.debug("username not set in config")
 
     return username
 
 
 def get_username_from_env():
-    """ Get the username for Jira from the environment variable. """
+    """Get the username for Jira from the environment variable."""
     username = None
     try:
-        username = os.environ['JIRA_USERNAME']
+        username = os.environ["JIRA_USERNAME"]
     except KeyError:
         log.debug("JIRA_USERNAME environment variable not set")
 
     return username
 
 
 def get_username_from_input():
-    """ Get the username for Jira from terminal. """
+    """Get the username for Jira from terminal."""
     username = input("Username (john.doe@foo.org): ").lower().strip()
     if len(username) == 0:
         log.error("Empty username not allowed")
         sys.exit(os.EX_NOUSER)
     else:
         return username
 
 
 def store_username_in_config(username):
-    """ Append the username to the config file. """
+    """Append the username to the config file."""
     # Needs global variable or arg instead.
-    with open(cfg.config_file, 'a') as f:
+    with open(cfg.config_file, "a") as f:
         f.write("\nusername: %s" % username)
 
 
 def get_username():
-    """ Main function to get the username from various places. """
-    username = get_username_from_env() or \
-               get_username_from_config()
+    """Main function to get the username from various places."""
+    username = get_username_from_env() or get_username_from_config()
 
     if username is not None:
         return username
 
     username = get_username_from_input()
 
     if username is not None:
-        question = "Username not found in %s, want to store it? (y/n) " % \
-                        cfg.config_file
+        question = (
+            "Username not found in %s, want to store it? (y/n) " % cfg.config_file
+        )
         answer = input(question).lower().strip()
-        if answer in set(['y']):
+        if answer in set(["y"]):
             store_username_in_config(username)
         return username
     else:
         log.error("No JIRA_USERNAME exported and no username found in config.yml")
         sys.exit(os.EX_NOUSER)
 
 
 def get_password():
     """
     Get the password either from the environment variable or from the
     terminal.
     """
     try:
-        password = os.environ['JIRA_PASSWORD']
+        password = os.environ["JIRA_PASSWORD"]
         return password
     except KeyError:
         log.debug("Forgot to export JIRA_PASSWORD?")
 
     password = getpass.getpass()
     if len(password) == 0:
         log.error("JIRA_PASSWORD not exported or empty password provided")
@@ -92,32 +93,40 @@
     """
     Makes a connection to the Jira server and returns the Jira instance to the
     caller.
     """
     username = get_username()
 
     server = cfg.get_server(use_test_server)
-    url = server.get('url')
-    token = server.get('token')
+    url = server.get("url")
+    token = server.get("token")
 
     # password based authentication
     if not token:
         password = get_password()
 
     try:
         if token:
-            log.debug("Accessing %s with %s using token based authentication" % (url, username))
+            log.debug(
+                "Accessing %s with %s using token based authentication"
+                % (url, username)
+            )
             j = JIRA(url, basic_auth=(username, token)), username
         else:
-            log.debug("Accessing %s with %s using password based authentication" % (url, username))
+            log.debug(
+                "Accessing %s with %s using password based authentication"
+                % (url, username)
+            )
             j = JIRA(url, basic_auth=(username, password)), username
     except JIRAError as e:
-        if e.text.find('CAPTCHA_CHALLENGE') != -1:
-            log.error('Captcha verification has been triggered by '\
-                   'JIRA - please go to JIRA using your web '\
-                   'browser, log out of JIRA, log back in '\
-                   'entering the captcha; after that is done, '\
-                   'please re-run the script')
+        if e.text.find("CAPTCHA_CHALLENGE") != -1:
+            log.error(
+                "Captcha verification has been triggered by "
+                "JIRA - please go to JIRA using your web "
+                "browser, log out of JIRA, log back in "
+                "entering the captcha; after that is done, "
+                "please re-run the script"
+            )
             sys.exit(os.EX_NOPERM)
         else:
             raise
     return j
```

### Comparing `jipdate-2.0.1/pyproject.toml` & `jipdate-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jipdate-2.0.1/PKG-INFO` & `jipdate-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jipdate
-Version: 2.0.1
+Version: 2.0.2
 Summary: Command line tool for Jira
 Author-email: Joakim Bech <joakim.bech@linaro.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: jinja2
 Requires-Dist: jira
```

