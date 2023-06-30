# Comparing `tmp/inuits_policy_based_auth-3.0.1.tar.gz` & `tmp/inuits_policy_based_auth-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-3.0.1.tar", last modified: Tue Jun 20 08:25:32 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-4.0.0.tar", last modified: Fri Jun 30 10:44:53 2023, max compression
```

## Comparing `inuits_policy_based_auth-3.0.1.tar` & `inuits_policy_based_auth-4.0.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/
--rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/LICENSE
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7133 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/README.md
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1881 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)    11621 2023-06-20 08:23:35.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2744 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      571 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/
--rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1435 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2942 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1591 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)    10620 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-06-20 08:25:32.000000 inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/top_level.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/setup.cfg
--rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-06-20 08:23:35.000000 inuits_policy_based_auth-3.0.1/setup.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.953282 inuits_policy_based_auth-3.0.1/tests/
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1947 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/custom_token.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1508 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/flask_process.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/integration/test_api/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1793 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/app.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2593 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3480 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1040 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:25:32.956616 inuits_policy_based_auth-3.0.1/tests/unit/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)    11998 2023-06-20 08:03:51.000000 inuits_policy_based_auth-3.0.1/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/LICENSE
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7133 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/README.md
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1881 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     8649 2023-06-30 10:22:16.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2744 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      571 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1435 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2942 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1591 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    10620 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     7595 2023-06-30 10:44:53.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-06-30 10:44:53.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-06-30 10:44:53.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-06-30 10:44:53.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-06-30 10:44:53.000000 inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/top_level.txt
+-rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/setup.cfg
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-06-30 10:33:23.000000 inuits_policy_based_auth-4.0.0/setup.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/tests/
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/tests/integration/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.227095 inuits_policy_based_auth-4.0.0/tests/integration/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/integration/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authorization/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1947 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/custom_token.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1508 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/flask_process.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/integration/test_api/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/test_api/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1793 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/test_api/app.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2593 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3480 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/unit/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/unit/authentication/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authentication/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/unit/authorization/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     1040 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-06-30 10:44:53.230428 inuits_policy_based_auth-4.0.0/tests/unit/helpers/
+-rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/helpers/__init__.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 gverm     (1000) gverm     (1001)    11998 2023-06-27 10:44:19.000000 inuits_policy_based_auth-4.0.0/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-3.0.1/LICENSE` & `inuits_policy_based_auth-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/PKG-INFO` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: inuits_policy_based_auth
-Version: 3.0.1
+Name: inuits-policy-based-auth
+Version: 4.0.0
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-3.0.1/README.md` & `inuits_policy_based_auth-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/request_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/contexts/user_context.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth/policy_factory.py` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth/policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/PKG-INFO` & `inuits_policy_based_auth-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: inuits-policy-based-auth
-Version: 3.0.1
+Name: inuits_policy_based_auth
+Version: 4.0.0
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inuits_policy_based_auth-3.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt` & `inuits_policy_based_auth-4.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/setup.py` & `inuits_policy_based_auth-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     ],
     license="GPLv2",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     name="inuits_policy_based_auth",
     packages=find_packages(exclude=["tests"]),
     provides=["inuits_policy_based_auth"],
-    version="3.0.1",
+    version="4.0.0",
 )
```

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-4.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-4.0.0/tests/integration/authorization/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/custom_token.py` & `inuits_policy_based_auth-4.0.0/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/flask_process.py` & `inuits_policy_based_auth-4.0.0/tests/integration/flask_process.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/test_api/app.py` & `inuits_policy_based_auth-4.0.0/tests/integration/test_api/app.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-4.0.0/tests/integration/test_api/policy_loader.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-4.0.0/tests/integration/test_policy_factory.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-4.0.0/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-4.0.0/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-4.0.0/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-4.0.0/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-3.0.1/tests/unit/test_policy_factory.py` & `inuits_policy_based_auth-4.0.0/tests/unit/test_policy_factory.py`

 * *Files identical despite different names*

