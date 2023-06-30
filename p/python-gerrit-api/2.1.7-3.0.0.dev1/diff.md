# Comparing `tmp/python-gerrit-api-2.1.7.tar.gz` & `tmp/python-gerrit-api-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-2.1.7.tar", last modified: Wed Jun 14 04:48:27 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.0.dev1.tar", last modified: Fri Jun 30 15:46:47 2023, max compression
```

## Comparing `python-gerrit-api-2.1.7.tar` & `python-gerrit-api-3.0.0.dev1.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.718738 python-gerrit-api-2.1.7/gerrit/
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.718738 python-gerrit-api-2.1.7/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/accounts/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/reviewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/changes/revision/
--rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/changes/revision/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/gitiles/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/gitiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.722738 python-gerrit-api-2.1.7/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.726739 python-gerrit-api-2.1.7/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.726739 python-gerrit-api-2.1.7/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 04:48:27.000000 python-gerrit-api-2.1.7/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:48:27.730738 python-gerrit-api-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-14 04:48:17.000000 python-gerrit-api-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.353120 python-gerrit-api-3.0.0.dev1/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27452 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.357120 python-gerrit-api-3.0.0.dev1/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.361120 python-gerrit-api-3.0.0.dev1/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/gitiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.365120 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 15:46:47.000000 python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:46:47.369120 python-gerrit-api-3.0.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-30 15:46:36.000000 python-gerrit-api-3.0.0.dev1/tests/test_revision.py
```

### Comparing `python-gerrit-api-2.1.7/LICENSE` & `python-gerrit-api-3.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-2.1.7/PKG-INFO` & `python-gerrit-api-3.0.0.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 2.1.7
+Version: 3.0.0.dev1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://img.shields.io/pypi/v/python-gerrit-api.svg
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
+    :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-2.1.7/README.rst` & `python-gerrit-api-3.0.0.dev1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://img.shields.io/pypi/v/python-gerrit-api.svg
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
+    :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-2.1.7/gerrit/__init__.py` & `python-gerrit-api-3.0.0.dev1/gerrit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-__version__ = "2.1.7"
+__version__ = "3.0.0.dev1"
 
-import json
 import netrc
 from gerrit.utils.requester import Requester
+from gerrit.utils.common import (
+    decode_response,
+    strip_trailing_slash
+)
 from gerrit.config.config import GerritConfig
 from gerrit.projects.projects import GerritProjects
 from gerrit.accounts.accounts import GerritAccounts
 from gerrit.groups.groups import GerritGroups
 from gerrit.plugins.plugins import GerritPlugins
 from gerrit.changes.changes import GerritChanges
-from gerrit.gitiles import GerritGitiles
 
 
-class GerritClient(object):
+class GerritClient:
     """
     Python wrapper for the Gerrit V3.x REST API.
 
     """
 
     default_headers = {"Content-Type": "application/json; charset=UTF-8"}
 
@@ -31,15 +33,15 @@
         use_netrc=False,
         ssl_verify=True,
         cert=None,
         timeout=60,
         max_retries=None,
         auth_suffix="/a"
     ):
-        self._base_url = self.strip_trailing_slash(base_url)
+        self._base_url = strip_trailing_slash(base_url)
 
         if use_netrc:
             password = self.get_password_from_netrc_file()
 
         self.requester = Requester(
             base_url=base_url,
             username=username,
@@ -62,60 +64,22 @@
 
         netrc_client = netrc.netrc()
         auth_tokens = netrc_client.authenticators(self._base_url)
         if not auth_tokens:
             raise ValueError(f"The '{self._base_url}' host name is not found in netrc file.")
         return auth_tokens[2]
 
-    @classmethod
-    def strip_trailing_slash(cls, url):
-        """
-        remove url's trailing slash
-        :param url: url
-        :return:
-        """
-        while url.endswith("/"):
-            url = url[:-1]
-        return url
-
     def get_endpoint_url(self, endpoint):
         """
         Return the complete url including host and port for a given endpoint.
         :param endpoint: service endpoint as str
         :return: complete url (including host and port) as str
         """
         return f"{self._base_url}{self.auth_suffix}{endpoint}"
 
-    @staticmethod
-    def decode_response(response):
-        """Strip off Gerrit's magic prefix and decode a response.
-        :returns:
-            Decoded JSON content as a dict, or raw text if content could not be
-            decoded as JSON.
-        :raises:
-            requests.HTTPError if the response contains an HTTP error status code.
-        """
-        magic_json_prefix = ")]}'\n"
-        content_type = response.headers.get("content-type", "")
-
-        content = response.content.strip()
-        if response.encoding:
-            content = content.decode(response.encoding)
-        if not content:
-            return content
-        if content_type.split(";")[0] != "application/json":
-            return content
-        if content.startswith(magic_json_prefix):
-            index = len(magic_json_prefix)
-            content = content[index:]
-        try:
-            return json.loads(content)
-        except ValueError:
-            raise ValueError(f"Invalid json content: {content}")
-
     @property
     def config(self):
         """
         Config related REST APIs
 
         :return:
         """
@@ -179,50 +143,45 @@
         """
         get the information about the Gerrit server configuration.
 
         :return:
         """
         return self.config.get_server_info()
 
-    @property
-    def gitiles(self):
-        """gitiles plugin rest api"""
-        return GerritGitiles(gerrit=self)
-
     def get(self, endpoint, **kwargs):
         """
         Send HTTP GET to the endpoint.
 
         :param endpoint: The endpoint to send to.
         :return:
         """
         response = self.requester.get(self.get_endpoint_url(endpoint), **kwargs)
-        result = self.decode_response(response)
+        result = decode_response(response)
         return result
 
     def post(self, endpoint, **kwargs):
         """
         Send HTTP POST to the endpoint.
 
         :param endpoint: The endpoint to send to.
         :return:
         """
         response = self.requester.post(self.get_endpoint_url(endpoint), **kwargs)
-        result = self.decode_response(response)
+        result = decode_response(response)
         return result
 
     def put(self, endpoint, **kwargs):
         """
         Send HTTP PUT to the endpoint.
 
         :param endpoint: The endpoint to send to.
         :return:
         """
         response = self.requester.put(self.get_endpoint_url(endpoint), **kwargs)
-        result = self.decode_response(response)
+        result = decode_response(response)
         return result
 
     def delete(self, endpoint):
         """
         Send HTTP DELETE to the endpoint.
 
         :param endpoint: The endpoint to send to.
```

### Comparing `python-gerrit-api-2.1.7/gerrit/accounts/account.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
+from gerrit.utils.gerritbase import GerritBase
 from gerrit.accounts.emails import GerritAccountEmails
 from gerrit.accounts.ssh_keys import GerritAccountSSHKeys
 from gerrit.accounts.gpg_keys import GerritAccountGPGKeys
 
 
-class GerritAccount(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "username"
-        self.endpoint = f"/accounts/{self.username}"
+class GerritAccount(GerritBase):
+    def __init__(self, account, gerrit):
+        self.account = account
+        self.gerrit = gerrit
+        self.endpoint = f"/accounts/{self.account}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return str(self.account)
+
+    def get_detail(self):
+        """
+        fetch account info in more details, such as: registered_on
+
+        :return:
+        """
+        result = self.gerrit.get(self.endpoint + "/detail")
+        return result
 
     def get_name(self):
         """
         Retrieves the full name of an account.
 
         :return:
         """
@@ -187,23 +200,23 @@
 
         :return:
         """
         return self.gerrit.get(self.endpoint + "/oauthtoken")
 
     @property
     def emails(self):
-        return GerritAccountEmails(username=self.username, gerrit=self.gerrit)
+        return GerritAccountEmails(account=self.account, gerrit=self.gerrit)
 
     @property
     def ssh_keys(self):
-        return GerritAccountSSHKeys(username=self.username, gerrit=self.gerrit)
+        return GerritAccountSSHKeys(account=self.account, gerrit=self.gerrit)
 
     @property
     def gpg_keys(self):
-        return GerritAccountGPGKeys(username=self.username, gerrit=self.gerrit)
+        return GerritAccountGPGKeys(account=self.account, gerrit=self.gerrit)
 
     def list_capabilities(self):
         """
         Returns the global capabilities that are enabled for the specified user.
 
         :return:
         """
@@ -476,15 +489,14 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html
           #contributor-agreement-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/agreements",
                                json=input_, headers=self.gerrit.default_headers)
 
-
     def delete_draft_comments(self, input_):
         """
         Deletes some or all of a user’s draft comments.
 
         .. code-block:: python
 
             input_ = {
@@ -512,15 +524,15 @@
     def get_default_starred_changes(self):
         """
         Gets the changes that were starred with the default star by the identified user account.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/starred.changes")
-        return [self.gerrit.changes.get(item.get("id")) for item in result]
+        return result
 
     def put_default_star_on_change(self, id_):
         """
         Star a change with the default label.
 
         :param id_: change id
         :return:
@@ -539,15 +551,15 @@
     def get_starred_changes(self):
         """
         Gets the changes that were starred with any label by the identified user account.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/stars.changes")
-        return [self.gerrit.changes.get(item.get("id")) for item in result]
+        return result
 
     def get_star_labels_from_change(self, id_):
         """
         Get star labels from a change.
 
         :param id_: change id
         :return:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+import logging
+import requests
 from gerrit.accounts.account import GerritAccount
+from gerrit.utils.exceptions import (
+    AccountNotFoundError,
+    AccountAlreadyExistsError,
+    GerritAPIException
+)
 
 
-class GerritAccounts(object):
+logger = logging.getLogger(__name__)
+
+
+class GerritAccounts:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/accounts"
 
     def search(
         self,
-        query,
-        limit=None,
-        skip=None,
-        detailed=False,
-        suggested=False,
-        all_emails=False,
+        query: str,
+        limit: int = 25,
+        skip: int = 0,
+        detailed: bool = False,
+        suggested: bool = False,
+        all_emails: bool = False,
     ):
         """
         Queries accounts visible to the caller.
 
         :param query: Query string
         :param limit: Int value that allows to limit the number of accounts
                       to be included in the output results
@@ -36,40 +46,45 @@
                            for each account will be added to the output result
         :return:
         """
         option = filter(
             None,
             ["DETAILS" if detailed else None, "ALL_EMAILS" if all_emails else None],
         )
-        option = None if not option else option
+        # option = None if not option else option
         params = {
             k: v for k, v in (("n", limit), ("S", skip), ("o", option)) if v is not None
         }
 
         endpoint = self.endpoint + "/?"
         if suggested:
             endpoint += "suggest&"
         endpoint += f"q={query}"
 
         return self.gerrit.get(endpoint, params=params)
 
-    def get(self, username, detailed=False):
+    def get(self, account):
         """
         Returns an account
 
-        :param username: username or _account_id
-        :param detailed: boolean type, If True then fetch info in more details, such as:
-            registered_on
+        :param account: username or email or _account_id or 'self'
         :return:
         """
-        endpoint = self.endpoint + f"/{username}/"
-        if detailed:
-            endpoint += "detail"
-        result = self.gerrit.get(endpoint)
-        return GerritAccount(json=result, gerrit=self.gerrit)
+        try:
+            endpoint = self.endpoint + f"/{account}/"
+            result = self.gerrit.get(endpoint)
+
+            account_ = result.get("_account_id")
+            return GerritAccount(account=account_, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Account {account} does not exist"
+                logger.error(message)
+                raise AccountNotFoundError(message)
+            raise GerritAPIException from error
 
     def create(self, username, input_):
         """
         Creates a new account.
 
         .. code-block:: python
 
@@ -85,10 +100,16 @@
             new_account = client.accounts.create('john.doe', input_)
 
         :param username: account username
         :param input_: the AccountInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#account-input
         :return:
         """
-        result = self.gerrit.put(
-            self.endpoint + f"/{username}", json=input_, headers=self.gerrit.default_headers)
-        return GerritAccount(json=result, gerrit=self.gerrit)
+        try:
+            self.get(username)
+            message = f"Account {username} already exists"
+            logger.error(message)
+            raise AccountAlreadyExistsError(message)
+        except AccountNotFoundError:
+            self.gerrit.put(
+                self.endpoint + f"/{username}", json=input_, headers=self.gerrit.default_headers)
+            return self.get(username)
```

### Comparing `python-gerrit-api-2.1.7/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/emails.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
-
+import logging
+import requests
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.utils.exceptions import (
+    AccountEmailNotFoundError,
+    AccountEmailAlreadyExistsError,
+    GerritAPIException
+)
+
+
+logger = logging.getLogger(__name__)
+
+
+class GerritAccountEmail(GerritBase):
+    def __init__(self, email, account, gerrit):
+        self.email = email
+        self.account = account
+        self.gerrit = gerrit
+        self.endpoint = f"/accounts/{self.account}/emails/{self.email}"
+        GerritBase.__init__(self)
 
-class GerritAccountEmail(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "email"
-        self.endpoint = f"/accounts/{self.username}/emails/{self.email}"
+    def __str__(self):
+        return self.email
 
     def delete(self):
         """
         Deletes an email address of an account.
 
         :return:
         """
@@ -23,56 +38,74 @@
         Sets an email address as preferred email address for an account.
 
         :return:
         """
         self.gerrit.put(self.endpoint + "/preferred")
 
 
-class GerritAccountEmails(object):
-    def __init__(self, username, gerrit):
-        self.username = username
+class GerritAccountEmails:
+    def __init__(self, account, gerrit):
+        self.account = account
         self.gerrit = gerrit
-        self.endpoint = f"/accounts/{self.username}/emails"
+        self.endpoint = f"/accounts/{self.account}/emails"
 
     def list(self):
         """
         Returns the email addresses that are configured for the specified user.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint)
-        return GerritAccountEmail.parse_list(result, username=self.username, gerrit=self.gerrit)
+        return result
 
     def create(self, email):
         """
         Registers a new email address for the user.
 
         :return:
         """
-        return self.gerrit.put(self.endpoint + f"/{email}")
+        try:
+            self.get(email)
+            message = f"Account Email {email} already register"
+            logger.error(message)
+            raise AccountEmailAlreadyExistsError(message)
+        except AccountEmailNotFoundError:
+            self.gerrit.put(self.endpoint + f"/{email}")
+            return self.get(email)
 
     def get(self, email):
         """
         Retrieves an email address of a user.
 
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{email}")
-        return GerritAccountEmail(json=result, username=self.username, gerrit=self.gerrit)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{email}")
+
+            email_ = result.get("email")
+            return GerritAccountEmail(email=email_, account=self.account, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Account Email {email} does not exist"
+                logger.error(message)
+                raise AccountEmailNotFoundError(message)
+            raise GerritAPIException from error
 
     def set_preferred(self, email):
         """
         Sets an email address as preferred email address for an account.
 
         :param email: account email
         :return:
         """
+        self.get(email)
         self.gerrit.put(self.endpoint + f"/{email}/preferred")
 
     def delete(self, email):
         """
         Deletes an email address of an account.
 
         :param email: account email
         :return:
         """
+        self.get(email)
         self.gerrit.delete(self.endpoint + f"/{email}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/gpg_keys.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,80 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
+import logging
+import requests
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.utils.exceptions import (
+    GPGKeyNotFoundError,
+    GerritAPIException
+)
+
+logger = logging.getLogger(__name__)
 
 
-class GerritAccountGPGKey(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.endpoint = f"/accounts/{self.username}/gpgkeys"
+class GerritAccountGPGKey(GerritBase):
+    def __init__(self, id, account, gerrit):
+        self.id = id
+        self.account = account
+        self.gerrit = gerrit
+        self.endpoint = f"/accounts/{self.account}/gpgkeys/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def delete(self):
         """
         Deletes a GPG key of a user.
 
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{self.id}")
+        self.gerrit.delete(self.endpoint)
 
 
-class GerritAccountGPGKeys(object):
-    def __init__(self, username, gerrit):
-        self.username = username
+class GerritAccountGPGKeys:
+    def __init__(self, account, gerrit):
+        self.account = account
         self.gerrit = gerrit
-        self.endpoint = f"/accounts/{self.username}/gpgkeys"
+        self.endpoint = f"/accounts/{self.account}/gpgkeys"
 
     def list(self):
         """
         Returns the GPG keys of an account.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint)
         keys = []
         for key, value in result.items():
             gpg_key = value
             gpg_key.update({"id": key})
             keys.append(gpg_key)
 
-        return GerritAccountGPGKey.parse_list(
-            keys, username=self.username, gerrit=self.gerrit
-        )
+        return keys
 
     def get(self, id_):
         """
         Retrieves a GPG key of a user.
 
         :param id_: GPG key id
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{id_}")
-        return GerritAccountGPGKey(json=result, username=self.username, gerrit=self.gerrit)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{id_}")
+
+            id = result.get("id")
+            return GerritAccountGPGKey(id=id, account=self.account, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"GPG key {id_} does not exist"
+                logger.error(message)
+                raise GPGKeyNotFoundError(message)
+            raise GerritAPIException from error
 
     def modify(self, input_):
         """
         Add or delete one or more GPG keys for a user.
 
         .. code-block:: python
 
@@ -96,17 +117,18 @@
             account = client.accounts.get('kevin.shi')
             result = account.gpg_keys.modify(input_)
 
         :param input_: the GpgKeysInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-accounts.html#gpg-keys-input
         :return:
         """
-        return self.gerrit.post(self.endpoint , json=input_, headers=self.gerrit.default_headers)
+        return self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
 
     def delete(self, id_):
         """
         Deletes a GPG key of a user.
 
         :param id_: GPG key id
         :return:
         """
+        self.get(id_)
         self.gerrit.delete(self.endpoint + f"/{id_}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/webhooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
+from gerrit.utils.gerritbase import GerritBase
 
 
-class GerritAccountSSHKey(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "seq"
-        self.endpoint = f"/accounts/{self.username}/sshkeys"
+class GerritProjectWebHook(GerritBase):
+    def __init__(self, name: str, project: str, gerrit):
+        self.name = name
+        self.project = project
+        self.gerrit = gerrit
+        self.endpoint = f"/config/server/webhooks~projects/{self.project}/remotes/{self.name}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.name
 
     def delete(self):
         """
-        Deletes an SSH key of a user.
+        Delete a webhook for a project.
 
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{str(self.seq)}")
+        self.gerrit.delete(self.endpoint)
 
 
-class GerritAccountSSHKeys(object):
-    def __init__(self, username, gerrit):
-        self.username = username
+class GerritProjectWebHooks:
+    def __init__(self, project, gerrit):
+        self.project = project
         self.gerrit = gerrit
-        self.endpoint = f"/accounts/{self.username}/sshkeys"
+        self.endpoint = f"/config/server/webhooks~projects/{self.project}/remotes"
 
     def list(self):
         """
-        Returns the SSH keys of an account.
+        List existing webhooks for a project.
 
         :return:
         """
-        result = self.gerrit.get(self.endpoint)
-        return GerritAccountSSHKey.parse_list(result, username=self.username, gerrit=self.gerrit)
+        result = self.gerrit.get(self.endpoint + "/")
+
+        return result
 
-    def get(self, seq):
+    def create(self, name, input_):
         """
-        Retrieves an SSH key of a user.
+        Create or update a webhook for a project.
+
+        .. code-block:: python
+
+            input_ = {
+                "url": "https://foo.org/gerrit-events",
+                "maxTries": "3",
+                "sslVerify": "true"
+            }
+
+            project = client.projects.get('myproject')
+            new_webhook = project.webhooks.create('test', input_)
 
-        :param seq: SSH key id
+        :param name: the webhook name
+        :param input_: the RemoteInfo entity
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{str(seq)}")
-        return GerritAccountSSHKey(json=result, username=self.username, gerrit=self.gerrit)
+        result = self.gerrit.put(
+            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+        return result
 
-    def add(self, ssh_key):
+    def get(self, name):
         """
-        Adds an SSH key for a user.
-        The SSH public key must be provided as raw content in the request body.
+        Get information about one webhook.
 
-        :param ssh_key: SSH key raw content
+        :param name: the webhook name
         :return:
         """
-        result = self.gerrit.post(self.endpoint,
-                                  data=ssh_key, headers={"Content-Type": "plain/text"})
-        return GerritAccountSSHKey(json=result, username=self.username, gerrit=self.gerrit)
+        result = self.gerrit.get(self.endpoint + f"/{name}")
+        name = result.get("name")
+        return GerritProjectWebHook(name=name, project=self.project, gerrit=self.gerrit)
 
-    def delete(self, seq):
+    def delete(self, name):
         """
-        Deletes an SSH key of a user.
+        Delete a webhook for a project.
 
-        :param seq: SSH key id
+        :param name: the webhook name
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{str(seq)}")
+        self.gerrit.delete(self.endpoint + f"/{name}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/change.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/change.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from typing import Dict
+from gerrit.utils.gerritbase import GerritBase
 from gerrit.changes.reviewers import GerritChangeReviewers
 from gerrit.changes.revision import GerritChangeRevision
 from gerrit.changes.edit import GerritChangeEdit
 from gerrit.changes.messages import GerritChangeMessages
-from gerrit.utils.models import BaseModel
 
 
-class GerritChange(BaseModel):
-    def __init__(self, **kwargs):
-        self.revisions = {}
-        self.current_revision_number = 0
-        super().__init__(**kwargs)
+class GerritChange(GerritBase):
+    def __init__(self, id: str, gerrit):
+        self.id = id
+        self.gerrit = gerrit
         self.endpoint = f"/changes/{self.id}"
+        GerritBase.__init__(self)
+
+        self.revisions: Dict[str, str] = {}
+        self.current_revision_number = 0
+
+    def __str__(self):
+        return self.id
+
+    def get_detail(self, options=None):
+        """
+        retrieve a change with labels, detailed labels, detailed accounts, reviewer updates, and messages.
+
+        :param options: List of options to fetch additional data about a change
+        :return:
+        """
+        if options:
+            params = {"o": options}
+        else:
+            params = None
+        return self.gerrit.get(self.endpoint + "/detail", params=params)
 
     def get_meta_diff(self, old=None, meta=None):
         """
         Retrieves the difference between two historical states of a change by
         specifying the and the parameters. old=SHA-1,meta=SHA-1.
         If the parameter is not provided, the parent of the SHA-1 is used.
         If the parameter is not provided, the current state of the change is used.
@@ -114,15 +134,15 @@
         :param account:
         :param label:
         :param input_: the DeleteVoteInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
           #delete-vote-input
         :return:
         """
-        endpoint = f"/changes/{self.change}/reviewers/{account}/votes/{label}"
+        endpoint = f"{self.endpoint}/reviewers/{account}/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             endpoint += "/delete"
             self.gerrit.post(endpoint, json=input_, headers=self.gerrit.default_headers)
 
     def get_topic(self):
@@ -131,15 +151,15 @@
 
         :getter: Retrieves the topic of a change.
         :setter: Sets the topic of a change.
         :deleter: Deletes the topic of a change.
 
         :return:
         """
-        return self.gerrit.get(f"/changes/{self.id}/topic")
+        return self.gerrit.get(f"{self.endpoint}/topic")
 
     def set_topic(self, topic):
         """
         Sets the topic of a change.
 
         :param topic: The new topic
         :return:
@@ -150,26 +170,23 @@
 
     def delete_topic(self):
         """
         Deletes the topic of a change.
 
         :return:
         """
-        self.gerrit.delete(f"/changes/{self.id}/topic")
+        self.gerrit.delete(f"{self.endpoint}/topic")
 
     def get_assignee(self):
         """
         Retrieves the account of the user assigned to a change.
 
         :return:
         """
-        result = self.gerrit.get(self.endpoint + "/assignee")
-        if result:
-            username = result.get("username")
-            return self.gerrit.accounts.get(username)
+        return self.gerrit.get(self.endpoint + "/assignee")
 
     def set_assignee(self, input_):
         """
         Sets the assignee of a change.
 
         .. code-block:: python
 
@@ -182,47 +199,33 @@
 
         :param input_: the AssigneeInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#assignee-input
         :return:
         """
         result = self.gerrit.put(self.endpoint + "/assignee",
                                  json=input_, headers=self.gerrit.default_headers)
-        if result:
-            username = result.get("username")
-            return self.gerrit.accounts.get(username)
+        return result
 
     def get_past_assignees(self):
         """
         Returns a list of every user ever assigned to a change, in the order in which they were
         first assigned.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/past_assignees")
-        assignees = []
-        if result:
-            for item in result:
-                username = item.get("username")
-                assignee = self.gerrit.accounts.get(username)
-                assignees.append(assignee)
-
-        return assignees
+        return result
 
     def delete_assignee(self):
         """
         Deletes the assignee of a change.
 
         :return:
         """
-        response = self.gerrit.delete(self.endpoint + "/assignee")
-        result = self.gerrit.decode_response(response)
-
-        if result:
-            username = result.get("username")
-            return self.gerrit.accounts.get(username)
+        self.gerrit.delete(self.endpoint + "/assignee")
 
     def get_pure_revert(self, commit):
         """
         Check if the given change is a pure revert of the change it references in revertOf.
 
         :param commit: commit id
         :return:
@@ -368,15 +371,15 @@
         :return:
         """
         endpoint = self.endpoint + "/submit"
         if input_ is None:
             result = self.gerrit.post(endpoint)
         else:
             result = self.gerrit.post(endpoint,
-                                    json=input_, headers=self.gerrit.default_headers)
+                                      json=input_, headers=self.gerrit.default_headers)
         return result
 
     def list_submitted_together_changes(self):
         """
         Computes list of all changes which are submitted when Submit is called for this change,
         including the current change itself.
 
@@ -632,15 +635,14 @@
         :param input_: the HashtagsInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#hashtags-input
         :return:
         """
         return self.gerrit.post(self.endpoint + "/hashtags",
                                 json=input_, headers=self.gerrit.default_headers)
 
-
     @property
     def messages(self):
         return GerritChangeMessages(change=self.id, gerrit=self.gerrit)
 
     def check_submit_requirement(self, input_):
         """
         Tests a submit requirement.
@@ -656,36 +658,37 @@
         """
         Retrieves a change edit details.
         As response an EditInfo entity is returned that describes the change edit,
         or 204 No Content when change edit doesn't exist for this change.
 
         :return:
         """
-        result = self.gerrit.get(self.endpoint + "/edit")
-        return GerritChangeEdit(json=result, change=self.id, gerrit=self.gerrit)
+        return GerritChangeEdit(change=self.id, gerrit=self.gerrit)
 
     def create_empty_edit(self):
         """
         Creates empty change edit
 
         :return:
         """
         self.gerrit.post(self.endpoint + "/edit")
 
     @property
     def reviewers(self):
         return GerritChangeReviewers(change=self.id, gerrit=self.gerrit)
 
     def __get_revisions(self):
-        endpoint = f"/changes/?q={self.number}&o=ALL_REVISIONS"
+        number = self.to_dict().get("_number")
+
+        endpoint = f"/changes/?q={number}&o=ALL_REVISIONS"
         results = self.gerrit.get(endpoint)
 
         result = {}
         for item in results:
-            if item.get("_number") == self.number:
+            if item.get("_number") == number:
                 result = item
                 break
 
         revisions = result.get("revisions")
 
         if revisions is not None:
             for revision_sha, revision in revisions.items():
@@ -708,37 +711,36 @@
                             current (latest) revision.
                             Zero means current revision.
                             -N means the current revision number X minus N, so if the current
                             revision is 50, and -1 is given, the revision 49 will be retrieved.
         :return:
         """
         if isinstance(revision_id, int):
-            if len(self.revisions) == 0:
+            if len(self.revisions.keys()) == 0:
                 self.__get_revisions()
             if revision_id <= 0:
                 revision_id = self.current_revision_number + revision_id
             revision_id = self.__revision_number_to_sha(revision_id)
             if revision_id is None:
                 return None
 
         return GerritChangeRevision(
             gerrit=self.gerrit,
-            project=self.project,
             change=self.id,
             revision=revision_id
         )
 
     def get_attention_set(self):
         """
         Returns all users that are currently in the attention set.
         support this method since v3.3.0
 
         :return:
         """
-        return self.gerrit.get(f"/changes/{self.id}/attention")
+        return self.gerrit.get(f"{self.endpoint}/attention")
 
     def add_to_attention_set(self, input_):
         """
         Adds a single user to the attention set of a change.
         support this method since v3.3.0
 
         A user can only be added if they are not in the attention set.
@@ -787,8 +789,8 @@
         :return:
         """
         endpoint = self.endpoint + f"/attention/{id_}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             endpoint += "/delete"
-            return self.gerrit.post(endpoint, json=input_, headers=self.gerrit.default_headers)
+            self.gerrit.post(endpoint, json=input_, headers=self.gerrit.default_headers)
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/changes.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/changes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+import logging
+import requests
 from gerrit.changes.change import GerritChange
+from gerrit.utils.exceptions import (
+    ChangeNotFoundError,
+    GerritAPIException
+)
 
 
-class GerritChanges(object):
+logger = logging.getLogger(__name__)
+
+
+class GerritChanges:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/changes"
 
-    def search(self, query, options=None, limit=None, skip=None):
+    def search(self, query: str, options=None, limit: int = 25, skip: int = 0):
         """
         Queries changes visible to the caller.
 
         .. code-block:: python
 
             query = "is:open+owner:self+is:mergeable"
             result = client.changes.search(query=query, options=["LABELS"])
@@ -31,32 +40,39 @@
             k: v
             for k, v in (("o", options), ("n", limit), ("S", skip))
             if v is not None
         }
 
         return self.gerrit.get(self.endpoint + f"/?q={query}", params=params)
 
-    def get(self, id_, detailed=False, options=None):
+    def get(self, id_):
         """
         Retrieves a change.
 
         :param id_: change id
-        :param detailed: boolean value, if True then retrieve a change with
-                         labels, detailed labels, detailed accounts,
-                         reviewer updates, and messages.
-        :param options: List of options to fetch additional data about a change
         :return:
         """
-
-        endpoint = self.endpoint + f"/{id_}/"
-        if detailed:
-            endpoint += "detail"
-
-        result = self.gerrit.get(endpoint, params={"o": options})
-        return GerritChange(json=result, gerrit=self.gerrit)
+        try:
+            endpoint = self.endpoint + f"/{id_}/"
+            result = self.gerrit.get(endpoint)
+
+            id = result.get("id")
+            return GerritChange(id=id, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Change {id_} does not exist"
+                if id_.startswith("I"):
+                    res = self.search(query=f"change: {id_}")
+                    if len(res) > 0:
+                        change_ids = [item.get("id") for item in res]
+                        message = f"Change {id_} query multiple changes: {', '.join(change_ids)}, which one do you want?"
+
+                logger.error(message)
+                raise ChangeNotFoundError(message)
+            raise GerritAPIException from error
 
     def create(self, input_):
         """
         create a change
 
         .. code-block:: python
 
@@ -69,18 +85,24 @@
             }
             result = client.changes.create(input_)
 
         :param input_: the ChangeInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-input
         :return:
         """
+        project_name = input_.get("project")
+        branch_name = input_.get("branch")
+        project = self.gerrit.projects.get(project_name)
+        project.branches.get(branch_name)
+
         result = self.gerrit.post(self.endpoint + '/', json=input_, headers=self.gerrit.default_headers)
-        return GerritChange(json=result, gerrit=self.gerrit)
+        return result
 
     def delete(self, id_):
         """
         Deletes a change.
 
         :param id_: change id
         :return:
         """
+        self.get(id_)
         self.gerrit.delete(self.endpoint + f"/{id_}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/edit.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/edit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
-
-from gerrit.utils.models import BaseModel
+from urllib.parse import quote_plus
 
 
-class GerritChangeEdit(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "ref"
+class GerritChangeEdit:
+    def __init__(self, change: str, gerrit):
+        self.change = change
+        self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/edit"
 
     def get_change_file_content(self, file):
         """
         Retrieves content of a file from a change edit.
         The content of the file is returned as text encoded inside base64.
 
@@ -101,15 +96,15 @@
     def get_commit_message(self):
         """
         Retrieves commit message from change edit.
         The commit message is returned as base64 encoded string.
 
         :return:
         """
-        return self.gerrit.get(self.endpoint + f":message")
+        return self.gerrit.get(self.endpoint + ":message")
 
     def publish(self, input_):
         """
         Promotes change edit to a regular patch set.
 
         .. code-block:: python
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/messages.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from gerrit.utils.gerritbase import GerritBase
 
-from gerrit.utils.models import BaseModel
 
-
-class GerritChangeMessage(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class GerritChangeMessage(GerritBase):
+    def __init__(self, id: str, change: str, gerrit):
+        self.id = id
+        self.change = change
+        self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/messages/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def delete(self, input_=None):
         """
         Deletes a change message.
         Note that only users with the Administrate Server global capability are permitted to
         delete a change message.
 
@@ -31,37 +36,36 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
           #delete-change-message-input
         :return:
         """
         if input_ is None:
             self.gerrit.delete(self.endpoint)
         else:
-            result = self.gerrit.post(self.endpoint + "/delete",
-                                      json=input_, headers=self.gerrit.default_headers)
-            change = self.gerrit.changes.get(self.change)
-            return change.messages.get(result.get("id"))
+            self.gerrit.post(self.endpoint + "/delete",
+                             json=input_, headers=self.gerrit.default_headers)
 
 
-class GerritChangeMessages(object):
+class GerritChangeMessages:
     def __init__(self, change, gerrit):
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/messages"
 
     def list(self):
         """
         Lists all the messages of a change including detailed account information.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint)
-        return GerritChangeMessage.parse_list(result, change=self.change, gerrit=self.gerrit)
+        return result
 
     def get(self, id_):
         """
         Retrieves a change message including detailed account information.
 
         :param id_: change message id
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}")
-        return GerritChangeMessage(json=result, change=self.change, gerrit=self.gerrit)
+        id_ = result.get("id")
+        return GerritChangeMessage(id=id_, change=self.change, gerrit=self.gerrit)
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/reviewers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+import logging
+import requests
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.utils.exceptions import (
+    ReviewerNotFoundError,
+    ReviewerAlreadyExistsError,
+    GerritAPIException
+)
+
+logger = logging.getLogger(__name__)
 
-from gerrit.utils.models import BaseModel
 
+class GerritChangeReviewer(GerritBase):
+    def __init__(self, account: str, change: str, gerrit):
+        self.account = account
+        self.change = change
+        self.gerrit = gerrit
+        self.endpoint = f"/changes/{self.change}/reviewers/{self.account}"
+        GerritBase.__init__(self)
 
-class GerritChangeReviewer(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "username"
-        self.endpoint = f"/changes/{self.change}/reviewers/{self.username}"
+    def __str__(self):
+        return str(self.account)
 
     def delete(self, input_=None):
         """
         Deletes a reviewer from a change.
         Deleting a reviewer also removes that user from the attention set.
 
         .. code-block:: python
@@ -74,39 +87,47 @@
         endpoint = self.endpoint + f"/votes/{label}"
         if input_ is None:
             self.gerrit.delete(endpoint)
         else:
             self.gerrit.post(endpoint + "/delete", json=input_, headers=self.gerrit.default_headers)
 
 
-class GerritChangeReviewers(object):
+class GerritChangeReviewers:
     def __init__(self, change, gerrit):
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/reviewers"
 
     def list(self):
         """
         Lists the reviewers of a change.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/")
-        return GerritChangeReviewer.parse_list(result, change=self.change, gerrit=self.gerrit)
+        return result
 
     def get(self, account):
         """
         Retrieves a reviewer of a change.
 
         :param account: _account_id, name, username or email
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{account}")
-        if result:
-            return GerritChangeReviewer(json=result[0], change=self.change, gerrit=self.gerrit)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{account}")
+
+            account = result[0].get("_account_id")
+            return GerritChangeReviewer(account=account, change=self.change, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Reviewer {account} does not exist"
+                logger.error(message)
+                raise ReviewerNotFoundError(message)
+            raise GerritAPIException from error
 
     def add(self, input_):
         """
         Adds one user or all members of one group as reviewer to the change.
 
         Users can be moved from reviewer to CC and vice versa. This means if a user is added as
         CC that is already a reviewer on the change, the reviewer state of that user is updated
@@ -125,8 +146,16 @@
             change = client.changes.get('Project~stable~I10394472cbd17dd12454f229e4f6de00b143a444')
             new_reviewer = change.reviewers.add(input_)
 
         :param input_: the ReviewerInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#reviewer-input
         :return:
         """
-        return self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+        reviewer = input_.get("reviewer")
+        try:
+            self.get(reviewer)
+            message = f"Reviewer {reviewer} already exists"
+            logger.error(message)
+            raise ReviewerAlreadyExistsError(message)
+        except ReviewerNotFoundError:
+            self.gerrit.post(self.endpoint, json=input_, headers=self.gerrit.default_headers)
+            return self.get(reviewer)
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/revision/__init__.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
-
 from base64 import b64decode
+from urllib.parse import quote_plus
 from gerrit.changes.revision.drafts import GerritChangeRevisionDrafts
 from gerrit.changes.revision.comments import GerritChangeRevisionComments
 from gerrit.changes.revision.files import GerritChangeRevisionFiles
 
 
-class GerritChangeRevision(object):
-    def __init__(self, gerrit, project, change, revision="current"):
-        self.project = project
+class GerritChangeRevision:
+    def __init__(self, gerrit, change, revision="current"):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}"
 
+    def __repr__(self):
+        return f"<{self.__class__.__module__}.{self.__class__.__name__} {str(self)}>"
+
+    def __str__(self):
+        return str(self.revision)
+
     def get_commit(self):
         """
         Retrieves a parsed commit of a revision.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/commit")
-        commit = result.get("commit")
-        if commit:
-            project = self.gerrit.projects.get(self.project)
-            if project:
-                return project.get_commit(commit)
+        return result
 
     def get_description(self):
         """
         Retrieves the description of a patch set.
         If the patch set does not have a description an empty string is returned.
 
         :return:
@@ -69,18 +66,15 @@
         Returns the list of commits that are being integrated into a target branch by a merge
         commit. By default, the first parent is assumed to be uninteresting. By using the parent
         option another parent can be set as uninteresting (parents are 1-based).
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/mergelist")
-        return [
-            self.gerrit.projects.get(self.project).get_commit(item.get("commit"))
-            for item in result
-        ]
+        return result
 
     def get_revision_actions(self):
         """
         Retrieves revision actions of the revision of a change.
 
         :return:
         """
@@ -187,19 +181,19 @@
         return self.gerrit.post(self.endpoint + "/submit")
 
     def get_patch(self, zip_=False, download=False, path=None, decode=False):
         """
         Gets the formatted patch for one revision.
         The formatted patch is returned as text encoded inside base64 if decode is False.
 
-        Adding query parameter zip (for example /changes/…​/patch?zip) returns the patch as a
+        Adding query parameter zip (for example /changes/.../patch?zip) returns the patch as a
         single file inside of a ZIP archive. Clients can expand the ZIP to obtain the plain text
         patch, avoiding the need for a base64 decoding step. This option implies download.
 
-        Query parameter download (e.g. /changes/…​/patch?download) will suggest the browser
+        Query parameter download (e.g. /changes/.../patch?download) will suggest the browser
         save the patch as commitsha1.diff.base64, for later processing by command line tools.
 
         If the path parameter is set, the returned content is a diff of the single file that
         the path refers to.
 
         :param zip_:
         :param download:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/revision/comments.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/comments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from gerrit.utils.gerritbase import GerritBase
 
-from gerrit.utils.models import BaseModel
 
-
-class GerritChangeRevisionComment(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class GerritChangeRevisionComment(GerritBase):
+    def __init__(self, id: str, change: str, revision: str, gerrit):
+        self.id = id
+        self.change = change
+        self.revision = revision
+        self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/comments/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def delete(self, input_=None):
         """
         Deletes a published comment of a revision. Instead of deleting the whole comment,
         this endpoint just replaces the comment’s message with a new message, which contains
         the name of the user who deletes the comment and the reason why it’s deleted.
 
@@ -37,15 +43,15 @@
         if input_ is None:
             return self.gerrit.delete(self.endpoint)
         else:
             return self.gerrit.post(self.endpoint + "/delete",
                                     json=input_, headers=self.gerrit.default_headers)
 
 
-class GerritChangeRevisionComments(object):
+class GerritChangeRevisionComments:
     def __init__(self, change, revision, gerrit):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/comments"
 
     def list(self):
@@ -57,22 +63,22 @@
         result = self.gerrit.get(self.endpoint)
         comments = []
         for key, value in result.items():
             for item in value:
                 comment = item
                 comment.update({"path": key})
                 comments.append(comment)
-        return GerritChangeRevisionComment.parse_list(
-            comments, change=self.change, revision=self.revision, gerrit=self.gerrit
-        )
+        return comments
 
     def get(self, id_):
         """
         Retrieves a published comment of a revision.
 
         :param id_:
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}")
+
+        id = result.get("id")
         return GerritChangeRevisionComment(
-            json=result, change=self.change, revision=self.revision, gerrit=self.gerrit
+            id=id, change=self.change, revision=self.revision, gerrit=self.gerrit
         )
```

### Comparing `python-gerrit-api-2.1.7/gerrit/changes/revision/drafts.py` & `python-gerrit-api-3.0.0.dev1/gerrit/changes/revision/drafts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from gerrit.utils.gerritbase import GerritBase
 
-from gerrit.utils.models import BaseModel
 
-
-class GerritChangeRevisionDraft(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class GerritChangeRevisionDraft(GerritBase):
+    def __init__(self, id: str, change: str, revision: str, gerrit):
+        self.id = id
+        self.change = change
+        self.revision = revision
+        self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/drafts/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def update(self, input_):
         """
         Updates a draft comment on a revision.
 
         .. code-block:: python
 
@@ -26,29 +32,26 @@
             draft = revision.drafts.get('89f04e8c_9b7fd51d')
             result = draft.update(input_)
 
         :param input_: the CommentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#comment-input
         :return:
         """
-        result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
-        return GerritChangeRevisionDraft(
-            json=result, change=self.change, revision=self.revision, gerrit=self.gerrit
-        )
+        return self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
 
     def delete(self):
         """
         Deletes a draft comment from a revision.
 
         :return:
         """
         self.gerrit.delete(self.endpoint)
 
 
-class GerritChangeRevisionDrafts(object):
+class GerritChangeRevisionDrafts:
     def __init__(self, change, revision, gerrit):
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self.endpoint = self.gerrit.get(f"/changes/{self.change}/revisions/{self.revision}/drafts")
 
     def list(self):
@@ -60,28 +63,29 @@
         result = self.gerrit.get(f"/changes/{self.change}/revisions/{self.revision}/drafts")
         drafts = []
         for key, value in result.items():
             for item in value:
                 draft = item
                 draft.update({"path": key})
                 drafts.append(draft)
-        return GerritChangeRevisionDraft.parse_list(
-            drafts, change=self.change, revision=self.revision, gerrit=self.gerrit
-        )
+
+        return drafts
 
     def get(self, id_):
         """
         Retrieves a draft comment of a revision that belongs to the calling user.
 
         :param id_: the draft comment id
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}")
+
+        id = result.get("id")
         return GerritChangeRevisionDraft(
-            json=result, change=self.change, revision=self.revision, gerrit=self.gerrit
+            id=id, change=self.change, revision=self.revision, gerrit=self.gerrit
         )
 
     def create(self, input_):
         """
         Creates a draft comment on a revision.
 
         .. code-block:: python
@@ -96,17 +100,15 @@
             new_draft = revision.drafts.create(input_)
 
         :param input_: the CommentInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#comment-input
         :return:
         """
         result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
-        return GerritChangeRevisionDraft(
-            json=result, change=self.change, revision=self.revision, gerrit=self.gerrit
-        )
+        return result
 
     def delete(self, id_):
         """
         Deletes a draft comment from a revision.
 
         :param id_: the draft comment id
         :return:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/config/caches.py` & `python-gerrit-api-3.0.0.dev1/gerrit/config/caches.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
-
-
-class Cache(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "name"
-        self.endpoint = "/config/server/caches"
+class Cache:
+    def __init__(self, name: str, gerrit):
+        self.name = name
+        self.gerrit = gerrit
+        self.endpoint = f"/config/server/caches/{self.name}"
 
     def flush(self):
         """
         Flushes a cache.
 
         :return:
         """
-        self.gerrit.post(self.endpoint + f"/{self.name}/flush")
+        self.gerrit.post(self.endpoint + "/flush")
 
 
-class Caches(object):
+class Caches:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/config/server/caches"
 
     def list(self):
         """
         Lists the caches of the server. Caches defined by plugins are included.
@@ -33,25 +30,27 @@
         result = self.gerrit.get(self.endpoint)
         caches = []
         for key, value in result.items():
             cache = value
             cache.update({"name": key})
             caches.append(cache)
 
-        return Cache.parse_list(caches, gerrit=self.gerrit)
+        return caches
 
     def get(self, name):
         """
         Retrieves information about a cache.
 
         :param name: cache name
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{name}")
-        return Cache(json=result, gerrit=self.gerrit)
+
+        name = result.get("name")
+        return Cache(name=name, gerrit=self.gerrit)
 
     def flush(self, name):
         """
         Flushes a cache.
 
         :param name: cache name
         :return:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/config/config.py` & `python-gerrit-api-3.0.0.dev1/gerrit/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from gerrit.config.caches import Caches
 from gerrit.config.tasks import Tasks
 
 
-class GerritConfig(object):
+class GerritConfig:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/config/server"
 
     def get_version(self):
         """
         get the version of the Gerrit server.
```

### Comparing `python-gerrit-api-2.1.7/gerrit/config/tasks.py` & `python-gerrit-api-3.0.0.dev1/gerrit/accounts/ssh_keys.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,89 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
+import logging
+import requests
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.utils.exceptions import (
+    SSHKeyNotFoundError,
+    GerritAPIException
+)
+
+logger = logging.getLogger(__name__)
 
 
-class Task(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.endpoint = "/config/server/tasks"
+class GerritAccountSSHKey(GerritBase):
+    def __init__(self, seq, account, gerrit):
+        self.seq = seq
+        self.account = account
+        self.gerrit = gerrit
+        self.endpoint = f"/accounts/{self.account}/sshkeys"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return str(self.seq)
 
     def delete(self):
         """
-        Kills a task from the background work queue that the Gerrit daemon is currently performing,
-        or will perform in the near future.
+        Deletes an SSH key of a user.
 
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{self.id}")
+        self.gerrit.delete(self.endpoint + f"/{str(self.seq)}")
 
 
-class Tasks(object):
-    def __init__(self, gerrit):
+class GerritAccountSSHKeys:
+    def __init__(self, account, gerrit):
+        self.account = account
         self.gerrit = gerrit
-        self.endpoint = "/config/server/tasks"
+        self.endpoint = f"/accounts/{self.account}/sshkeys"
 
     def list(self):
         """
-        Lists the tasks from the background work queues that the Gerrit daemon is currently
-        performing, or will perform in the near future.
+        Returns the SSH keys of an account.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint)
-        return Task.parse_list(result, gerrit=self.gerrit)
+        return result
 
-    def get(self, id_):
+    def get(self, seq):
         """
-        Retrieves a task from the background work queue that the Gerrit daemon is currently
-        performing, or will perform in the near future.
+        Retrieves an SSH key of a user.
 
-        :param id_: task id
+        :param seq: SSH key id
         :return:
         """
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{str(seq)}")
 
-        result = self.gerrit.get(self.endpoint + f"/{id_}")
-        return Task(json=result, gerrit=self.gerrit)
+            seq = result.get("seq")
+            return GerritAccountSSHKey(seq=seq, account=self.account, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"SSH key {seq} does not exist"
+                logger.error(message)
+                raise SSHKeyNotFoundError(message)
+            raise GerritAPIException from error
+
+    def add(self, ssh_key):
+        """
+        Adds an SSH key for a user.
+        The SSH public key must be provided as raw content in the request body.
+
+        :param ssh_key: SSH key raw content
+        :return:
+        """
+        result = self.gerrit.post(self.endpoint,
+                                  data=ssh_key, headers={"Content-Type": "plain/text"})
+        return result
 
-    def delete(self, id_):
+    def delete(self, seq):
         """
-        Kills a task from the background work queue that the Gerrit daemon is currently performing,
-        or will perform in the near future.
+        Deletes an SSH key of a user.
 
-        :param id_: task id
+        :param seq: SSH key id
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{id_}")
+        self.get(seq)
+        self.gerrit.delete(self.endpoint + f"/{str(seq)}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/groups/group.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
+from gerrit.utils.gerritbase import GerritBase
 from gerrit.groups.members import GerritGroupMembers
 from gerrit.groups.subgroups import GerritGroupSubGroups
 
 
-class GerritGroup(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "name"
+class GerritGroup(GerritBase):
+    def __init__(self, group_id: int, gerrit):
+        self.id = group_id
+        self.gerrit = gerrit
         self.endpoint = f"/groups/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def get_name(self):
         """
         Retrieves the name of a group.
 
         :return:
         """
         return self.gerrit.get(self.endpoint + "/name")
 
+    def get_detail(self):
+        """
+        Retrieves a group with the direct members and the directly included groups.
+
+        :return:
+        """
+        return self.gerrit.get(self.endpoint + "/detail")
+
     def set_name(self, input_):
         """
         Renames a Gerrit internal group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
         .. code-block:: python
```

### Comparing `python-gerrit-api-2.1.7/gerrit/groups/groups.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+import logging
+import requests
 from gerrit.groups.group import GerritGroup
 from gerrit.utils.common import params_creator
-from packaging.version import parse
+from gerrit.utils.exceptions import (
+    GroupNotFoundError,
+    GroupAlreadyExistsError,
+    GerritAPIException
+)
 
+logger = logging.getLogger(__name__)
 
-class GerritGroups(object):
+
+class GerritGroups:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/groups"
 
-    def list(self, pattern_dispatcher=None, options=None, limit=None, skip=None):
+    def list(self, pattern_dispatcher=None, options=None, limit: int = 25, skip: int = 0):
         """
         Lists the groups accessible by the caller.
 
         :param pattern_dispatcher: Dict of pattern type with respective
                      pattern value: {('match'|'regex') : value}
         :param options: Additional fields can be obtained by adding o parameters,
                         each option requires more lookups and slows down the query response time to
@@ -29,15 +37,15 @@
         :return:
         """
         params = params_creator((("o", options), ("n", limit), ("S", skip)),
                                 {"match": "m", "regex": "r"}, pattern_dispatcher)
 
         return self.gerrit.get(self.endpoint, params=params)
 
-    def search(self, query, options=None, limit=None, skip=None):
+    def search(self, query, options=None, limit: int = 25, skip: int = 0):
         """
         Query Groups
 
         :param query:
         :param options: Additional fields can be obtained by adding o parameters,
                         each option requires more lookups and slows down the query response time to
                         the client so they are generally disabled by default. Optional fields are:
@@ -45,40 +53,44 @@
                           MEMBERS: include list of direct group members.
         :param limit: Int value that allows to limit the number of groups
                       to be included in the output results
         :param skip: Int value that allows to skip the given
                      number of groups from the beginning of the list
         :return:
         """
-        version = self.gerrit.version
-        if parse(version) < parse("3.2.0"):
-            endpoint = self.endpoint + f"/?query2={query}"
-        else:
-            endpoint = self.endpoint + f"/?query={query}"
+        endpoint = self.endpoint + f"/?query={query}"
 
         params = {
             k: v
             for k, v in (("o", options), ("limit", limit), ("start", skip))
             if v is not None
         }
 
         return self.gerrit.get(endpoint, params=params)
 
-    def get(self, id_, detailed=False):
+    def get(self, id_):
         """
         Retrieves a group.
 
         :param id_: group id, or group_id, or group name
         :param detailed:
         :return:
         """
-        endpoint = self.endpoint + f"/{id_}/"
-        if detailed:
-            endpoint += "detail"
-        return GerritGroup(json=self.gerrit.get(endpoint), gerrit=self.gerrit)
+        try:
+            endpoint = self.endpoint + f"/{id_}/"
+            res = self.gerrit.get(endpoint)
+
+            group_id = res.get("id")
+            return GerritGroup(group_id=group_id, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Group {id_} does not exist"
+                logger.error(message)
+                raise GroupNotFoundError(message)
+            raise GerritAPIException from error
 
     def create(self, name, input_):
         """
         Creates a new Gerrit internal group.
 
         .. code-block:: python
 
@@ -91,10 +103,16 @@
             new_group = client.groups.create('My-Project2-Committers', input_)
 
         :param name: group name
         :param input_: the GroupInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-groups.html#group-input
         :return:
         """
-        result = self.gerrit.put(
-            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
-        return GerritGroup(json=result, gerrit=self.gerrit)
+        try:
+            self.get(name)
+            message = f"Group {name} already exists"
+            logger.error(message)
+            raise GroupAlreadyExistsError(message)
+        except GroupNotFoundError:
+            self.gerrit.put(
+                self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+            return self.get(name)
```

### Comparing `python-gerrit-api-2.1.7/gerrit/groups/members.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/subgroups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 
 
-class GerritGroupMembers(object):
+class GerritGroupSubGroups:
     def __init__(self, group_id, gerrit):
-        self.group_id = group_id
+        self.id = group_id
         self.gerrit = gerrit
-        self.endpoint = f"/groups/{self.group_id}/members"
+        self.endpoint = f"/groups/{self.id}/groups/"
 
     def list(self):
         """
-        Lists the direct members of a Gerrit internal group.
+        Lists the direct subgroups of a group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint)
-
-        accounts = []
+        subgroups = []
         for item in result:
-            username = item.get("username")
-            accounts.append(self.gerrit.accounts.get(username))
+            group_id = item.get("id")
+            subgroups.append(self.gerrit.groups.get(group_id))
 
-        return accounts
+        return subgroups
 
-    def get(self, username):
+    def get(self, subgroup):
         """
-        Retrieves a group member.
+        Retrieves a subgroup.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        :param username: account username
+        :param subgroup: subgroup id or name
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{username}")
-        if result:
-            username = result.get("username")
-            return self.gerrit.accounts.get(username)
+        result = self.gerrit.get(self.endpoint + f"/{subgroup}")
+
+        subgroup_id = result.get("id")
+        return self.gerrit.groups.get(subgroup_id)
 
-    def add(self, username):
+    def add(self, subgroup):
         """
-        Adds a user as member to a Gerrit internal group.
+        Adds an internal or external group as subgroup to a Gerrit internal group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        :param username: account username
+        :param subgroup: subgroup id or name
         :return:
         """
-        result = self.gerrit.put(self.endpoint + f"/{username}")
-        if result:
-            username = result.get("username")
-            return self.gerrit.accounts.get(username)
+        result = self.gerrit.put(self.endpoint + f"/{subgroup}")
+
+        subgroup_id = result.get("id")
+        return self.gerrit.groups.get(subgroup_id)
 
-    def remove(self, username):
+    def remove(self, subgroup):
         """
-        Removes a user from a Gerrit internal group.
+        Removes a subgroup from a Gerrit internal group.
         This endpoint is only allowed for Gerrit internal groups;
         attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        :param username: account username
+        :param subgroup: subgroup id or name
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{username}")
+        self.gerrit.delete(self.endpoint + f"/{subgroup}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.0.dev1/gerrit/plugins/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.models import BaseModel
 from gerrit.utils.common import params_creator
 
 
-class GerritPlugin(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.endpoint = f"/plugins/{self.id}"
+class GerritPlugin:
+    def __init__(self, id_: str, gerrit):
+        self.id_ = id_
+        self.gerrit = gerrit
+        self.endpoint = f"/plugins/{self.id_}"
 
     def enable(self):
         """
         Enables a plugin on the Gerrit server.
 
         :return:
         """
         result = self.gerrit.post(self.endpoint + "/gerrit~enable")
-        return self.gerrit.plugins.get(result.get("id"))
+        return result
 
     def disable(self):
         """
         Disables a plugin on the Gerrit server.
 
         :return:
         """
         result = self.gerrit.post(self.endpoint + "/gerrit~disable")
-        return self.gerrit.plugins.get(result.get("id"))
+        return result
 
     def reload(self):
         """
         Reloads a plugin on the Gerrit server.
 
         :return:
         """
         result = self.gerrit.post(self.endpoint + "/gerrit~reload")
-        return self.gerrit.plugins.get(result.get("id"))
+        return result
 
 
-class GerritPlugins(object):
+class GerritPlugins:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/plugins"
 
-    def list(self, is_all=False, limit=None, skip=None, pattern_dispatcher=None):
+    def list(
+        self,
+        is_all: bool = False,
+        limit: int = 25,
+        skip: int = 0,
+        pattern_dispatcher=None
+    ):
         """
         Lists the plugins installed on the Gerrit server.
 
         :param is_all: boolean value, if True then all plugins (including
                        hidden ones) will be added to the results
         :param limit: Int value that allows to limit the number of plugins
                       to be included in the output results
@@ -66,15 +72,17 @@
     def get(self, id_):
         """
 
         :param id_: plugin id
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}/gerrit~status")
-        return GerritPlugin(json=result, gerrit=self.gerrit)
+
+        plugin_id = result.get("id")
+        return GerritPlugin(id_=plugin_id, gerrit=self.gerrit)
 
     def install(self, id_, input_):
         """
         Installs a new plugin on the Gerrit server.
 
         .. code-block:: python
 
@@ -88,8 +96,8 @@
         :param input_: the PluginInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-plugins.html#plugin-input
         :return:
         """
         result = self.gerrit.put(
             self.endpoint + f"/{id_}.jar", json=input_, headers=self.gerrit.default_headers
         )
-        return GerritPlugin(json=result, gerrit=self.gerrit)
+        return result
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/branches.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/tags.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,119 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
-
-from gerrit.utils.models import BaseModel
+import logging
+from urllib.parse import quote_plus
+import requests
 from gerrit.utils.common import params_creator
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.utils.exceptions import (
+    TagNotFoundError,
+    TagAlreadyExistsError,
+    GerritAPIException
+)
 
 
-class GerritProjectBranch(BaseModel):
-    branch_prefix = "refs/heads/"
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "ref"
-        self.endpoint = f"/projects/{self.project}/branches/{self.name}"
-
-    @property
-    def name(self):
-        return self.ref.replace(self.branch_prefix, "")
-
-    def get_file_content(self, file):
-        """
-        Gets the content of a file from the HEAD revision of a certain branch.
-        The content is returned as base64 encoded string.
-
-        :param file: the file path
-        :return:
-        """
-        return self.gerrit.get(self.endpoint + f"/files/{quote_plus(file)}/content")
-
-    def is_mergeable(self, input_):
-        """
-        Gets whether the source is mergeable with the target branch.
+logger = logging.getLogger(__name__)
 
-        .. code-block:: python
-
-            input_ = {
-                'source': 'testbranch',
-                'strategy': 'recursive'
-            }
-            result = stable.is_mergeable(input_)
 
-        :param input_: the MergeInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#merge-input
-        :return:
-        """
-        return self.gerrit.get(self.endpoint + "/mergeable", params=input_)
+class GerritProjectTag(GerritBase):
+    def __init__(self, name: str, project: str, gerrit):
+        self.name = name
+        self.project = project
+        self.gerrit = gerrit
+        self.endpoint = f"/projects/{self.project}/tags/{self.name}"
+        GerritBase.__init__(self)
 
-    def get_reflog(self):
-        """
-        Gets the reflog of a certain branch.
-
-        :return:
-        """
-        return self.gerrit.get(self.endpoint + "/reflog")
+    def __str__(self):
+        return self.name
 
     def delete(self):
         """
-        Delete a branch.
+        Delete a tag.
 
         :return:
         """
         self.gerrit.delete(self.endpoint)
 
 
-class GerritProjectBranches(object):
-    branch_prefix = "refs/heads/"
+class GerritProjectTags:
+    tag_prefix = "refs/tags/"
 
     def __init__(self, project, gerrit):
         self.project = project
         self.gerrit = gerrit
-        self.endpoint = f"/projects/{self.project}/branches"
+        self.endpoint = f"/projects/{self.project}/tags"
 
-    def list(self, pattern_dispatcher=None, limit=None, skip=None):
+    def list(self, pattern_dispatcher=None, limit: int = 25, skip: int = 0):
         """
-        List the branches of a project.
+        List the tags of a project.
 
         :param pattern_dispatcher: Dict of pattern type with respective
                pattern value: {('match'|'regex') : value}
-        :param limit: Limit the number of branches to be included in the results.
-        :param skip: Skip the given number of branches from the beginning of the list.
+        :param limit: Limit the number of tags to be included in the results.
+        :param skip: Skip the given number of tags from the beginning of the list.
         :return:
         """
         params = params_creator((("n", limit), ("s", skip)),
                                 {"match": "m", "regex": "r"}, pattern_dispatcher)
-
         return self.gerrit.get(self.endpoint + "/", params=params)
 
     def get(self, name):
         """
-        get a branch by ref
+        get a tag by ref
 
-        :param name: branch ref name
+        :param name: the tag ref
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
-        return GerritProjectBranch(json=result, project=self.project, gerrit=self.gerrit)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
+
+            ref = result.get("ref")
+            name = ref.replace(self.tag_prefix, "")
+            return GerritProjectTag(name=name, project=self.project, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Tag {name} does not exist"
+                logger.error(message)
+                raise TagNotFoundError(message)
+            raise GerritAPIException from error
 
     def create(self, name, input_):
         """
-        Creates a new branch.
+        Creates a new tag on the project.
 
         .. code-block:: python
 
             input_ = {
-                'revision': '76016386a0d8ecc7b6be212424978bb45959d668'
+                "message": "annotation",
+                'revision': 'c83117624b5b5d8a7f86093824e2f9c1ed309d63'
             }
+
             project = client.projects.get('myproject')
-            new_branch = project.branches.create('stable', input_)
+            new_tag = project.tags.create('1.1.8', input_)
 
+        :param name: the tag name
+        :param input_: the TagInput entity,
+          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#tag-input
+        :return:
+        """
+        try:
+            self.get(name)
+            message = f"Tag {name} already exists"
+            logger.error(message)
+            raise TagAlreadyExistsError(message)
+        except TagNotFoundError:
+            self.gerrit.put(
+                self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
 
-        :param name: the branch name
-        :param input_: the BranchInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#branch-info
-        :return:
-        """
-        return self.gerrit.put(
-            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+            return self.get(name)
 
     def delete(self, name):
         """
-        Delete a branch.
+        Delete a tag.
 
-        :param name: branch ref name
+        :param name: the tag ref
         :return:
         """
+        self.get(name)
         self.gerrit.delete(self.endpoint + f"/{quote_plus(name)}")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/commit.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/commit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
-
-from gerrit.utils.models import BaseModel
+from base64 import b64decode
+from urllib.parse import quote_plus
+from gerrit.utils.gerritbase import GerritBase
 
 
-class GerritProjectCommit(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "commit"
+class GerritProjectCommit(GerritBase):
+    def __init__(self, commit: str, project: str, gerrit):
+        self.commit = commit
+        self.project = project
+        self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/commits/{self.commit}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.commit
 
     def get_include_in(self):
         """
         Retrieves the branches and tags in which a change is included.
 
         :return:
         """
         return self.gerrit.get(self.endpoint + "/in")
 
-    def get_file_content(self, file):
+    def get_file_content(self, file, decode=False):
         """
         Gets the content of a file from a certain commit.
 
         :param file: the file path
+        :param decode: Decode bas64 to plain text.
         :return:
         """
-        return self.gerrit.get(self.endpoint + f"/files/{quote_plus(file)}/content")
+        result = self.gerrit.get(self.endpoint + f"/files/{quote_plus(file)}/content")
+        if decode:
+            return b64decode(result).decode("utf-8")
+        return result
 
     def cherry_pick(self, input_):
         """
         Cherry-picks a commit of a project to a destination branch.
 
         .. code-block:: python
 
@@ -47,15 +53,15 @@
         :param input_: the CherryPickInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html
           #cherrypick-input
         :return:  the resulting cherry-picked change
         """
         result = self.gerrit.post(
             self.endpoint + "/cherrypick", json=input_, headers=self.gerrit.default_headers)
-        return self.gerrit.changes.get(result.get("id"))
+        return result
 
     def list_change_files(self):
         """
         Lists the files that were modified, added or deleted in a commit.
 
         :return:
         """
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/dashboards.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from gerrit.utils.gerritbase import GerritBase
 
-from gerrit.utils.models import BaseModel
 
+class GerritProjectDashboard(GerritBase):
+    def __init__(self, id: str, project: str, gerrit):
+        self.id = id
+        self.project = project
+        self.gerrit = gerrit
+        self.endpoint = f"/projects/{self.project}/dashboards/{self.id}"
+        GerritBase.__init__(self)
 
-class GerritProjectDashboard(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __str__(self):
+        return str(self.id)
 
     def delete(self):
         """
         Deletes a project dashboard.
 
         :return:
         """
-        self.gerrit.delete(f"/projects/{self.project}/dashboards/{self.id}")
+        self.gerrit.delete(self.endpoint)
 
 
-class GerritProjectDashboards(object):
+class GerritProjectDashboards:
     def __init__(self, project, gerrit):
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/dashboards"
 
     def list(self):
         """
         List custom dashboards for a project.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/")
-        return GerritProjectDashboard.parse_list(result, project=self.project, gerrit=self.gerrit)
+        return result
 
     def create(self, id_, input_):
         """
         Creates a project dashboard, if a project dashboard with the given dashboard ID doesn't
         exist yet.
 
         .. code-block:: python
@@ -51,26 +57,28 @@
         :param input_: the DashboardInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
           #dashboard-input
         :return:
         """
         result = self.gerrit.put(
             self.endpoint + f"/{id_}", json=input_, headers=self.gerrit.default_headers)
-        return GerritProjectDashboard(json=result, project=self.project, gerrit=self.gerrit)
+        return result
 
     def get(self, id_):
         """
         Retrieves a project dashboard. The dashboard can be defined on that project or be inherited
         from a parent project.
 
         :param id_: the dashboard id
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{id_}")
-        return GerritProjectDashboard(json=result, project=self.project, gerrit=self.gerrit)
+
+        dashboard_id = result.get("id")
+        return GerritProjectDashboard(id=dashboard_id, project=self.project, gerrit=self.gerrit)
 
     def delete(self, id_):
         """
         Deletes a project dashboard.
 
         :param id_: the dashboard id
         :return:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/labels.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
+from gerrit.utils.gerritbase import GerritBase
 
-from gerrit.utils.models import BaseModel
 
-
-class GerritProjectLabel(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "name"
+class GerritProjectLabel(GerritBase):
+    def __init__(self, name: str, project: str, gerrit):
+        self.name = name
+        self.project = project
+        self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/labels/{self.name}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.name
 
     def set(self, input_):
         """
         Updates the definition of a label that is defined in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
         Properties which are not set in the input entity are not modified.
 
@@ -30,51 +34,53 @@
 
         :param input_: the LabelDefinitionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
           #label-definition-input
         :return:
         """
         result = self.gerrit.put(self.endpoint, json=input_, headers=self.gerrit.default_headers)
-        return self.gerrit.projects.get(self.project).labels.get(result.get("name"))
+        return result
 
     def delete(self):
         """
         Deletes the definition of a label that is defined in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
 
         :return:
         """
         self.gerrit.delete(self.endpoint)
 
 
-class GerritProjectLabels(object):
+class GerritProjectLabels:
     def __init__(self, project, gerrit):
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/labels"
 
     def list(self):
         """
         Lists the labels that are defined in this project.
 
         :return:
         """
         result = self.gerrit.get(self.endpoint + "/")
-        return GerritProjectLabel.parse_list(result, gerrit=self.gerrit)
+        return result
 
     def get(self, name):
         """
         Retrieves the definition of a label that is defined in this project.
         The calling user must have read access to the refs/meta/config branch of the project.
 
         :param name: label name
         :return:
         """
         result = self.gerrit.get(self.endpoint + f"/{name}")
-        return GerritProjectLabel(json=result, gerrit=self.gerrit)
+
+        name = result.get("name")
+        return GerritProjectLabel(name=name, project=self.project, gerrit=self.gerrit)
 
     def create(self, name, input_):
         """
         Creates a new label definition in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
         If a label with this name is already defined in this project, this label definition is
         updated (see Set Label).
@@ -97,15 +103,15 @@
         :param input_: the LabelDefinitionInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
           #label-definition-input
         :return:
         """
         result = self.gerrit.put(
             self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
-        return GerritProjectLabel(json=result, gerrit=self.gerrit)
+        return result
 
     def delete(self, name):
         """
         Deletes the definition of a label that is defined in this project.
         The calling user must have write access to the refs/meta/config branch of the project.
 
         :param name: label name
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/project.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from packaging.version import parse
+import logging
+import requests
+from gerrit.utils.gerritbase import GerritBase
+from gerrit.projects.commit import GerritProjectCommit
 from gerrit.projects.branches import GerritProjectBranches
 from gerrit.projects.tags import GerritProjectTags
-from gerrit.projects.commit import GerritProjectCommit
 from gerrit.projects.dashboards import GerritProjectDashboards
 from gerrit.projects.labels import GerritProjectLabels
 from gerrit.projects.webhooks import GerritProjectWebHooks
-from gerrit.changes.change import GerritChange
-from gerrit.utils.models import BaseModel
+from gerrit.utils.exceptions import (
+    CommitNotFoundError,
+    GerritAPIException
+)
+
+logger = logging.getLogger(__name__)
 
 
-class GerritProject(BaseModel):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+class GerritProject(GerritBase):
+    def __init__(self, project_id: str, gerrit):
+        self.id = project_id
+        self.gerrit = gerrit
         self.endpoint = f"/projects/{self.id}"
+        GerritBase.__init__(self)
+
+    def __str__(self):
+        return self.id
 
     def get_description(self):
         """
         Retrieves the description of a project.
 
         :return:
         """
@@ -88,23 +99,23 @@
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
           #project-parent-input
         :return:
         """
         return self.gerrit.put(self.endpoint + "/parent",
                                json=input_, headers=self.gerrit.default_headers)
 
-    def get_HEAD(self):
+    def get_head(self):
         """
         Retrieves for a project the name of the branch to which HEAD points.
 
         :return:
         """
         return self.gerrit.get(self.endpoint + "/HEAD")
 
-    def set_HEAD(self, input_):
+    def set_head(self, input_):
         """
         Sets HEAD for a project.
 
         .. code-block:: python
 
             input_ = {
                 "ref": "refs/heads/stable"
@@ -251,15 +262,15 @@
             result = project.create_change(input_)
 
         :param input_:
         :return:
         """
         result = self.gerrit.post(self.endpoint + "/create.change",
                                   json=input_, headers=self.gerrit.default_headers)
-        return GerritChange(json=result, gerrit=self.gerrit)
+        return result
 
     def create_access_rights_change(self, input_):
         """
         Sets access rights for the project using the diff schema provided by ProjectAccessInput
         This takes the same input as Update Access Rights, but creates a pending change for review.
         Like Create Change, it returns a ChangeInfo entity describing the resulting change.
         https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
@@ -268,15 +279,15 @@
         :param input_: the ProjectAccessInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html
           #project-access-input
         :return:
         """
         result = self.gerrit.put(self.endpoint + "/access:review",
                                  json=input_, headers=self.gerrit.default_headers)
-        return GerritChange(json=result, gerrit=self.gerrit)
+        return result
 
     def check_access(self, options):
         """
         runs access checks for other users.
 
         :param options:
           Check Access Options
@@ -377,38 +388,43 @@
 
     def get_commit(self, commit):
         """
         Retrieves a commit of a project.
 
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/commits/{commit}")
-        return GerritProjectCommit(json=result, project=self.id, gerrit=self.gerrit)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/commits/{commit}")
+
+            commit = result.get("commit")
+            return GerritProjectCommit(commit=commit, project=self.id, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Commit {commit} does not exist"
+                logger.error(message)
+                raise CommitNotFoundError(message)
+            raise GerritAPIException from error
 
     @property
     def dashboards(self):
         """
         gerrit dashboards operations
 
         :return:
         """
         return GerritProjectDashboards(project=self.id, gerrit=self.gerrit)
 
-    def get_labels(self):
+    @property
+    def labels(self):
         """
         gerrit labels or gerrit labels operations
 
         :return:
         """
-        version = self.gerrit.version
-        if parse(version) < parse("3.2.0"):
-            result = self.gerrit.get(self.endpoint)
-            return result.get("labels")
-        else:
-            return GerritProjectLabels(project=self.id, gerrit=self.gerrit)
+        return GerritProjectLabels(project=self.id, gerrit=self.gerrit)
 
     @property
     def webhooks(self):
         """
         gerrit webhooks operations, requires webhooks plugin
 
         :return:
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/projects.py` & `python-gerrit-api-3.0.0.dev1/gerrit/projects/projects.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
+import logging
+from typing import Any, Union, Dict, List, Optional
+from urllib.parse import quote_plus
+import requests
 from gerrit.projects.project import GerritProject
 from gerrit.utils.common import params_creator
+from gerrit.utils.exceptions import (
+    ProjectNotFoundError,
+    ProjectAlreadyExistsError,
+    GerritAPIException
+)
 
 
-class GerritProjects(object):
+logger = logging.getLogger(__name__)
+
+
+class GerritProjects:
     def __init__(self, gerrit):
         self.gerrit = gerrit
         self.endpoint = "/projects"
 
     def list(
         self,
-        is_all=False,
-        limit=None,
-        skip=None,
-        pattern_dispatcher=None,
-        project_type=None,
-        description=False,
-        branch=None,
-        state=None,
-    ):
+        is_all: bool = False,
+        limit: int = 25,
+        skip: int = 0,
+        pattern_dispatcher: Union[Dict, None] = None,
+        project_type: Optional[str] = None,
+        description: bool = False,
+        branch: Optional[str] = None,
+        state: Optional[str] = None,
+    ) -> List:
         """
         Get list of all available projects accessible by the caller.
 
         :param is_all: boolean value, if True then all projects (including
                        hidden ones) will be added to the results.
                        May not be used together with the state option.
         :param limit: Int value that allows to limit the number of projects
@@ -46,24 +54,27 @@
         :param state: Get all projects with the given state. May not be used together with the all
         option.
 
         :return:
         """
         if is_all and state:
             raise ValueError("is_all can not be used together with the state option.")
-        
+
         pattern_types = {"prefix": "p", "match": "m", "regex": "r"}
-        tuples = (("n", limit),("S", skip),("type", project_type),("b", branch),("state", state))
+        tuples = (("n", limit), ("S", skip), ("type", project_type), ("b", branch), ("state", state))
         params = params_creator(tuples, pattern_types, pattern_dispatcher)
-        params["all"] = int(is_all)
+        if is_all:
+            params.clear()
+            params["all"] = int(is_all)
         params["d"] = int(description)
+        print(params)
 
         return self.gerrit.get(self.endpoint + "/", params=params)
 
-    def search(self, query, limit=None, skip=None):
+    def search(self, query: str, limit: int = 25, skip: int = 0) -> List:
         """
         Queries projects visible to the caller. The query string must be provided by the
         query parameter.
         The start and limit parameters can be used to skip/limit results.
 
         query parameter
           * name:'NAME' Matches projects that have exactly the name 'NAME'.
@@ -81,25 +92,33 @@
                      number of accounts from the beginning of the list
         :return:
         """
         params = {k: v for k, v in (("limit", limit), ("start", skip)) if v is not None}
 
         return self.gerrit.get(self.endpoint + f"/?query={query}", params=params)
 
-    def get(self, name):
+    def get(self, name: str):
         """
         Retrieves a project.
 
         :param name: the name of the project
         :return:
         """
-        result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
-        return GerritProject(json=result, gerrit=self.gerrit)
+        try:
+            res = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
+            project_id = res.get("id")
+            return GerritProject(project_id=project_id, gerrit=self.gerrit)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Project {name} does not exist"
+                logger.error(message)
+                raise ProjectNotFoundError(message)
+            raise GerritAPIException from error
 
-    def create(self, project_name, input_):
+    def create(self, project_name: str, input_: Dict[str, Any]):
         """
         Creates a new project.
 
         .. code-block:: python
 
             input_ = {
                 "description": "This is a demo project.",
@@ -112,20 +131,26 @@
 
         :param project_name: the name of the project
         :param input_: the ProjectInput entity,
           https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#project-input
 
         :return:
         """
-        result = self.gerrit.put(
-            self.endpoint + f"/{quote_plus(project_name)}",
-            json=input_, headers=self.gerrit.default_headers)
-        return GerritProject(json=result, gerrit=self.gerrit)
+        try:
+            self.get(project_name)
+            message = f"Project {project_name} already exists"
+            logger.error(message)
+            raise ProjectAlreadyExistsError(message)
+        except ProjectNotFoundError:
+            self.gerrit.put(self.endpoint + f"/{quote_plus(project_name)}",
+                            json=input_, headers=self.gerrit.default_headers)
+            return self.get(project_name)
 
-    def delete(self, project_name):
+    def delete(self, project_name: str):
         """
         Delete the project, requires delete-project plugin
 
         :param project_name: project name
         :return:
         """
+        self.get(project_name)
         self.gerrit.post(self.endpoint + f"/{quote_plus(project_name)}/delete-project~delete")
```

### Comparing `python-gerrit-api-2.1.7/gerrit/projects/tags.py` & `python-gerrit-api-3.0.0.dev1/gerrit/groups/members.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,87 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
-from gerrit.utils.common import params_creator
-try:
-    from urllib.parse import quote_plus
-except ImportError:
-    from urllib import quote_plus
+import logging
+import requests
 
-from gerrit.utils.models import BaseModel
+from gerrit.utils.exceptions import (
+    GroupMemberNotFoundError,
+    GroupMemberAlreadyExistsError,
+    GerritAPIException
+)
 
+logger = logging.getLogger(__name__)
 
-class GerritProjectTag(BaseModel):
-    tag_prefix = "refs/tags/"
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.entity_name = "ref"
-        self.endpoint = f"/projects/{self.project}/tags"
-
-    @property
-    def name(self):
-        return self.ref.replace(self.tag_prefix, "")
-
-    def delete(self):
-        """
-        Delete a tag.
-
-        :return:
-        """
-        self.gerrit.delete(self.endpoint + f"/{self.name}")
-
-
-class GerritProjectTags(object):
-    tag_prefix = "refs/tags/"
-
-    def __init__(self, project, gerrit):
-        self.project = project
+class GerritGroupMembers:
+    def __init__(self, group_id, gerrit):
+        self.id = group_id
         self.gerrit = gerrit
-        self.endpoint = f"/projects/{self.project}/tags"
+        self.endpoint = f"/groups/{self.id}/members"
 
-    def list(self, pattern_dispatcher=None, limit=None, skip=None):
+    def list(self):
         """
-        List the tags of a project.
+        Lists the direct members of a Gerrit internal group.
+        This endpoint is only allowed for Gerrit internal groups;
+        attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        :param pattern_dispatcher: Dict of pattern type with respective
-               pattern value: {('match'|'regex') : value}
-        :param limit: Limit the number of tags to be included in the results.
-        :param skip: Skip the given number of tags from the beginning of the list.
         :return:
         """
-        params = params_creator((("n", limit), ("s", skip)),
-                                {"match": "m", "regex": "r"}, pattern_dispatcher)
-        return self.gerrit.get(self.endpoint + "/", params=params)
+        result = self.gerrit.get(self.endpoint)
 
-    def get(self, name):
-        """
-        get a tag by ref
+        accounts = []
+        for item in result:
+            account_id = item.get("_account_id")
+            accounts.append(self.gerrit.accounts.get(account_id))
 
-        :param name: the tag ref
-        :return:
-        """
-        result = self.gerrit.get(self.endpoint + f"/{quote_plus(name)}")
-        return GerritProjectTag(json=result, project=self.project, gerrit=self.gerrit)
+        return accounts
 
-    def create(self, name, input_):
+    def get(self, account):
         """
-        Creates a new tag on the project.
+        Retrieves a group member.
+        This endpoint is only allowed for Gerrit internal groups;
+        attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        .. code-block:: python
-
-            input_ = {
-                "message": "annotation",
-                'revision': 'c83117624b5b5d8a7f86093824e2f9c1ed309d63'
-            }
-
-            project = client.projects.get('myproject')
-            new_tag = project.tags.create('1.1.8', input_)
-
-        :param name: the tag name
-        :param input_: the TagInput entity,
-          https://gerrit-review.googlesource.com/Documentation/rest-api-projects.html#tag-input
+        :param account: account username or id
         :return:
         """
-        return self.gerrit.put(
-            self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+        try:
+            result = self.gerrit.get(self.endpoint + f"/{account}")
+            account_id = result.get("_account_id")
+            return self.gerrit.accounts.get(account_id)
+        except requests.exceptions.HTTPError as error:
+            if error.response.status_code in (404, 400):
+                message = f"Group member {account} does not exist"
+                logger.error(message)
+                raise GroupMemberNotFoundError(message)
+            raise GerritAPIException from error
+
+    def add(self, account):
+        """
+        Adds a user as member to a Gerrit internal group.
+        This endpoint is only allowed for Gerrit internal groups;
+        attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-    def delete(self, name):
+        :param account: account username or id
+        :return:
         """
-        Delete a tag.
+        try:
+            self.get(account)
+            message = f"Group member {account} already exists"
+            logger.error(message)
+            raise GroupMemberAlreadyExistsError(message)
+        except GroupMemberNotFoundError:
+            self.gerrit.put(self.endpoint + f"/{account}")
+            return self.get(account)
+
+    def remove(self, account):
+        """
+        Removes a user from a Gerrit internal group.
+        This endpoint is only allowed for Gerrit internal groups;
+        attempting to call on a non-internal group will return 405 Method Not Allowed.
 
-        :param name: the tag ref
+        :param account: account username or id
         :return:
         """
-        self.gerrit.delete(self.endpoint + f"/{quote_plus(name)}")
+        self.get(account)
+        self.gerrit.delete(self.endpoint + f"/{account}")
```

### Comparing `python-gerrit-api-2.1.7/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 2.1.7
+Version: 3.0.0.dev1
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,14 +28,16 @@
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://img.shields.io/pypi/v/python-gerrit-api.svg
     :target: https://pypi.python.org/pypi/python-gerrit-api
 .. image:: https://pepy.tech/badge/python-gerrit-api
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
+.. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
+    :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-2.1.7/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.0.dev1/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 gerrit/changes/revision/comments.py
 gerrit/changes/revision/drafts.py
 gerrit/changes/revision/files.py
 gerrit/config/__init__.py
 gerrit/config/caches.py
 gerrit/config/config.py
 gerrit/config/tasks.py
-gerrit/gitiles/__init__.py
 gerrit/groups/__init__.py
 gerrit/groups/group.py
 gerrit/groups/groups.py
 gerrit/groups/members.py
 gerrit/groups/subgroups.py
 gerrit/plugins/__init__.py
 gerrit/plugins/plugins.py
@@ -39,16 +38,22 @@
 gerrit/projects/labels.py
 gerrit/projects/project.py
 gerrit/projects/projects.py
 gerrit/projects/tags.py
 gerrit/projects/webhooks.py
 gerrit/utils/__init__.py
 gerrit/utils/common.py
-gerrit/utils/entity.py
 gerrit/utils/exceptions.py
-gerrit/utils/models.py
+gerrit/utils/gerritbase.py
 gerrit/utils/requester.py
+gitiles/__init__.py
 python_gerrit_api.egg-info/PKG-INFO
 python_gerrit_api.egg-info/SOURCES.txt
 python_gerrit_api.egg-info/dependency_links.txt
 python_gerrit_api.egg-info/requires.txt
-python_gerrit_api.egg-info/top_level.txt
+python_gerrit_api.egg-info/top_level.txt
+tests/test_accounts.py
+tests/test_changes.py
+tests/test_gitiles.py
+tests/test_groups.py
+tests/test_projects.py
+tests/test_revision.py
```

### Comparing `python-gerrit-api-2.1.7/setup.py` & `python-gerrit-api-3.0.0.dev1/setup.py`

 * *Files identical despite different names*

