# Comparing `tmp/finbourne-identity-sdk-0.0.2469.tar.gz` & `tmp/finbourne-identity-sdk-0.0.840.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finbourne-identity-sdk-0.0.2469.tar", last modified: Fri Jun 30 12:49:41 2023, max compression
+gzip compressed data, was "dist/finbourne-identity-sdk-0.0.840.tar", last modified: Wed Jul 15 09:47:57 2020, max compression
```

## Comparing `finbourne-identity-sdk-0.0.2469.tar` & `finbourne-identity-sdk-0.0.840.tar`

### file list

```diff
@@ -1,82 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11814 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/
--rw-r--r--   0 root         (0) root         (0)     4624 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    35285 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/applications_api.py
--rw-r--r--   0 root         (0) root         (0)    32946 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/identity_provider_api.py
--rw-r--r--   0 root         (0) root         (0)    13657 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/me_api.py
--rw-r--r--   0 root         (0) root         (0)    21035 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/personal_authentication_tokens_api.py
--rw-r--r--   0 root         (0) root         (0)    60534 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/roles_api.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/tokens_api.py
--rw-r--r--   0 root         (0) root         (0)    93888 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api/users_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/
--rw-r--r--   0 root         (0) root         (0)     3061 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7258 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9021 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7235 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     4679 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/add_scim_response.py
--rw-r--r--   0 root         (0) root         (0)     8995 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/api_key.py
--rw-r--r--   0 root         (0) root         (0)     9895 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/authentication_information.py
--rw-r--r--   0 root         (0) root         (0)     6328 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_api_key.py
--rw-r--r--   0 root         (0) root         (0)    11713 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_application_request.py
--rw-r--r--   0 root         (0) root         (0)     6825 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_role_request.py
--rw-r--r--   0 root         (0) root         (0)    15542 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10268 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/created_api_key.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/current_user_response.py
--rw-r--r--   0 root         (0) root         (0)     5447 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/error_detail.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6429 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6679 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/list_users_response.py
--rw-r--r--   0 root         (0) root         (0)     9543 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10708 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/o_auth_application.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     5747 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/role_id.py
--rw-r--r--   0 root         (0) root         (0)     8752 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/role_response.py
--rw-r--r--   0 root         (0) root         (0)     4647 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/set_password.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/set_password_response.py
--rw-r--r--   0 root         (0) root         (0)     4336 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_expiry.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_expiry_with_role.py
--rw-r--r--   0 root         (0) root         (0)     8410 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_request.py
--rw-r--r--   0 root         (0) root         (0)    16351 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_response.py
--rw-r--r--   0 root         (0) root         (0)     6488 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_role.py
--rw-r--r--   0 root         (0) root         (0)     4198 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_roles_response.py
--rw-r--r--   0 root         (0) root         (0)     4537 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/temporary_password.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/update_role_request.py
--rw-r--r--   0 root         (0) root         (0)    12896 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/update_user_request.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/user_response.py
--rw-r--r--   0 root         (0) root         (0)     9366 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/models/user_summary.py
--rw-r--r--   0 root         (0) root         (0)    13567 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/tcp/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4970 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/tcp/tcp_keep_alive_probes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/
--rw-r--r--   0 root         (0) root         (0)      622 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_client_builder.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_client_factory.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_configuration.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_configuration_loader.py
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      298 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/config_keys.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/finbourne_identity_retry.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/proxy_config.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/refreshing_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      364 2023-06-30 12:49:40.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3251 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 12:49:40.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-30 12:49:40.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-30 12:49:40.000000 finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 12:49:41.000000 finbourne-identity-sdk-0.0.2469/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2252 2023-06-30 12:49:01.000000 finbourne-identity-sdk-0.0.2469/setup.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)       53 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/MANIFEST.in
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      363 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/PKG-INFO
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     4278 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/__init__.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)       24 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/__version__.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      634 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/__init__.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    10333 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/application_metadata_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    20908 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/applications_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    21667 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/authentication_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    27279 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/domains_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    16845 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/personal_authentication_tokens_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    42154 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/roles_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5426 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/tokens_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    28886 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api/users_api.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    25372 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/api_client.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    10427 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/configuration.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3841 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/exceptions.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     2782 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/__init__.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6079 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/access_controlled_action.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     7817 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/access_controlled_resource.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5937 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/action_id.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5281 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/agreement_response.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6542 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/api_key.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6277 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/authentication_information.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5153 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_api_key.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6286 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_application_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    11248 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_domain_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     4490 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_role_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    10707 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_user_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     7498 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/created_api_key.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3619 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/domain_id.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     9224 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/domain_response.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5658 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/id_selector_definition.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     7686 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/identifier_part_schema.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5574 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/link.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     9315 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/lusid_problem_details.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    10503 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/lusid_validation_problem_details.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     7380 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/o_auth_application.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6723 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/problem_details.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5190 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5387 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/role.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     4554 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/role_id.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     6299 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/role_response.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3634 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_expiry.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     5555 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    12907 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_response.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3516 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/update_role_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     8518 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/update_user_request.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3635 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/user_id.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    11147 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/models/user_response.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)    12638 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/rest.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/tcp/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      106 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/tcp/__init__.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     4970 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/tcp/tcp_keep_alive_probes.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      549 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/__init__.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     7231 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_client_builder.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     4930 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_client_factory.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     2839 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_configuration.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     3535 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_configuration_loader.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      940 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/config_keys.json
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      882 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/finbourne_identity_retry.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     1725 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/proxy_config.py
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     2970 2020-07-15 09:41:04.000000 finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/refreshing_token.py
+drwxr-xr-x   0 rizwansaeed   (501) staff       (20)        0 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)      363 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     2926 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)        1 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)       84 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/requires.txt
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)       19 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/top_level.txt
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)       38 2020-07-15 09:47:57.000000 finbourne-identity-sdk-0.0.840/setup.cfg
+-rw-r--r--   0 rizwansaeed   (501) staff       (20)     2209 2020-07-15 09:47:53.000000 finbourne-identity-sdk-0.0.840/setup.py
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/__init__.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.0.2469"
+__version__ = "0.0.840"
 
 # import apis into sdk package
 from finbourne_identity.api.application_metadata_api import ApplicationMetadataApi
 from finbourne_identity.api.applications_api import ApplicationsApi
 from finbourne_identity.api.authentication_api import AuthenticationApi
-from finbourne_identity.api.identity_provider_api import IdentityProviderApi
-from finbourne_identity.api.me_api import MeApi
+from finbourne_identity.api.domains_api import DomainsApi
 from finbourne_identity.api.personal_authentication_tokens_api import PersonalAuthenticationTokensApi
 from finbourne_identity.api.roles_api import RolesApi
 from finbourne_identity.api.tokens_api import TokensApi
 from finbourne_identity.api.users_api import UsersApi
 
 # import ApiClient
 from finbourne_identity.api_client import ApiClient
@@ -36,49 +35,45 @@
 from finbourne_identity.exceptions import ApiValueError
 from finbourne_identity.exceptions import ApiKeyError
 from finbourne_identity.exceptions import ApiException
 # import models into sdk package
 from finbourne_identity.models.access_controlled_action import AccessControlledAction
 from finbourne_identity.models.access_controlled_resource import AccessControlledResource
 from finbourne_identity.models.action_id import ActionId
-from finbourne_identity.models.add_scim_response import AddScimResponse
+from finbourne_identity.models.agreement_response import AgreementResponse
 from finbourne_identity.models.api_key import ApiKey
 from finbourne_identity.models.authentication_information import AuthenticationInformation
 from finbourne_identity.models.create_api_key import CreateApiKey
 from finbourne_identity.models.create_application_request import CreateApplicationRequest
+from finbourne_identity.models.create_domain_request import CreateDomainRequest
 from finbourne_identity.models.create_role_request import CreateRoleRequest
 from finbourne_identity.models.create_user_request import CreateUserRequest
 from finbourne_identity.models.created_api_key import CreatedApiKey
-from finbourne_identity.models.current_user_response import CurrentUserResponse
-from finbourne_identity.models.error_detail import ErrorDetail
+from finbourne_identity.models.domain_id import DomainId
+from finbourne_identity.models.domain_response import DomainResponse
 from finbourne_identity.models.id_selector_definition import IdSelectorDefinition
 from finbourne_identity.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_identity.models.link import Link
-from finbourne_identity.models.list_users_response import ListUsersResponse
 from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
 from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from finbourne_identity.models.o_auth_application import OAuthApplication
+from finbourne_identity.models.problem_details import ProblemDetails
 from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
+from finbourne_identity.models.role import Role
 from finbourne_identity.models.role_id import RoleId
 from finbourne_identity.models.role_response import RoleResponse
-from finbourne_identity.models.set_password import SetPassword
-from finbourne_identity.models.set_password_response import SetPasswordResponse
 from finbourne_identity.models.support_access_expiry import SupportAccessExpiry
-from finbourne_identity.models.support_access_expiry_with_role import SupportAccessExpiryWithRole
 from finbourne_identity.models.support_access_request import SupportAccessRequest
 from finbourne_identity.models.support_access_response import SupportAccessResponse
-from finbourne_identity.models.support_role import SupportRole
-from finbourne_identity.models.support_roles_response import SupportRolesResponse
-from finbourne_identity.models.temporary_password import TemporaryPassword
 from finbourne_identity.models.update_role_request import UpdateRoleRequest
 from finbourne_identity.models.update_user_request import UpdateUserRequest
+from finbourne_identity.models.user_id import UserId
 from finbourne_identity.models.user_response import UserResponse
-from finbourne_identity.models.user_summary import UserSummary
 
 # import utilities into sdk package
 from finbourne_identity.utilities.api_client_builder import ApiClientBuilder
 from finbourne_identity.utilities.api_configuration import ApiConfiguration
 from finbourne_identity.utilities.api_configuration_loader import ApiConfigurationLoader
 from finbourne_identity.utilities.refreshing_token import RefreshingToken
 
 # import tcp utilities
-from finbourne_identity.tcp.tcp_keep_alive_probes import TCPKeepAlivePoolManager, TCPKeepAliveProxyManager
+from finbourne_identity.tcp.tcp_keep_alive_probes import TCPKeepAlivePoolManager, TCPKeepAliveProxyManager
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/__init__.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-from __future__ import absolute_import
-
-# flake8: noqa
-
-# import apis into api package
-from finbourne_identity.api.application_metadata_api import ApplicationMetadataApi
-from finbourne_identity.api.applications_api import ApplicationsApi
-from finbourne_identity.api.authentication_api import AuthenticationApi
-from finbourne_identity.api.identity_provider_api import IdentityProviderApi
-from finbourne_identity.api.me_api import MeApi
-from finbourne_identity.api.personal_authentication_tokens_api import PersonalAuthenticationTokensApi
-from finbourne_identity.api.roles_api import RolesApi
-from finbourne_identity.api.tokens_api import TokensApi
-from finbourne_identity.api.users_api import UsersApi
+from finbourne_identity.utilities.api_client_builder import ApiClientBuilder
+from finbourne_identity.utilities.api_configuration_loader import ApiConfigurationLoader
+from finbourne_identity.utilities.refreshing_token import RefreshingToken
+from finbourne_identity.utilities.api_client_factory import ApiClientFactory
+from finbourne_identity.utilities.finbourne_identity_retry import finbourne_identityretry
+from finbourne_identity.utilities.proxy_config import ProxyConfig
+from finbourne_identity.utilities.api_configuration import ApiConfiguration
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/application_metadata_api.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api/application_metadata_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,123 +1,206 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from finbourne_identity.api_client import ApiClient
-from finbourne_identity.exceptions import (  # noqa: F401
+from finbourne_identity.exceptions import (
     ApiTypeError,
     ApiValueError
 )
-from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
-from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 
 
 class ApplicationMetadataApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def get_registration_availability(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Check Registration availability  # noqa: E501
+
+        Identify whether there registrations service is available  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_registration_availability(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: str
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_registration_availability_with_http_info(**kwargs)  # noqa: E501
+
+    def get_registration_availability_with_http_info(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Check Registration availability  # noqa: E501
+
+        Identify whether there registrations service is available  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_registration_availability_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(str, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_registration_availability" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
+
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
+
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
+
+        return self.api_client.call_api(
+            '/api/metadata/eap', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='str',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def list_access_controlled_resources(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """[EARLY ACCESS] Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.list_access_controlled_resources(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: ResourceListOfAccessControlledResource
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ResourceListOfAccessControlledResource
         """
         kwargs['_return_http_data_only'] = True
         return self.list_access_controlled_resources_with_http_info(**kwargs)  # noqa: E501
 
     def list_access_controlled_resources_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """[EARLY ACCESS] Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.list_access_controlled_resources_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(ResourceListOfAccessControlledResource, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (ResourceListOfAccessControlledResource, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method list_access_controlled_resources" % key
                 )
@@ -126,47 +209,40 @@
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "ResourceListOfAccessControlledResource",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
             '/api/metadata/access/resources', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='ResourceListOfAccessControlledResource',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/applications_api.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api/roles_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,778 +1,960 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from finbourne_identity.api_client import ApiClient
-from finbourne_identity.exceptions import (  # noqa: F401
+from finbourne_identity.exceptions import (
     ApiTypeError,
     ApiValueError
 )
-from finbourne_identity.models.create_application_request import CreateApplicationRequest
-from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
-from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from finbourne_identity.models.o_auth_application import OAuthApplication
 
 
-class ApplicationsApi(object):
+class RolesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_application(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] CreateApplication: Create Application  # noqa: E501
+    def add_user_to_role(self, id, user_id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Add User to Role  # noqa: E501
 
-        Create a new Application  # noqa: E501
+        Adds the User to the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_application(async_req=True)
+        >>> thread = api.add_user_to_role(id, user_id, async_req=True)
         >>> result = thread.get()
 
-        :param create_application_request: Details of the application to be created
-        :type create_application_request: CreateApplicationRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param str user_id: The unique identifier for the User (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: OAuthApplication
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_application_with_http_info(**kwargs)  # noqa: E501
+        return self.add_user_to_role_with_http_info(id, user_id, **kwargs)  # noqa: E501
 
-    def create_application_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] CreateApplication: Create Application  # noqa: E501
+    def add_user_to_role_with_http_info(self, id, user_id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Add User to Role  # noqa: E501
 
-        Create a new Application  # noqa: E501
+        Adds the User to the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_application_with_http_info(async_req=True)
+        >>> thread = api.add_user_to_role_with_http_info(id, user_id, async_req=True)
         >>> result = thread.get()
 
-        :param create_application_request: Details of the application to be created
-        :type create_application_request: CreateApplicationRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param str user_id: The unique identifier for the User (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (OAuthApplication, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'create_application_request'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id', 'user_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_application" % key
+                    " to method add_user_to_role" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `add_user_to_role`")  # noqa: E501
+        # verify the required parameter 'user_id' is set
+        if ('user_id' not in local_var_params or
+                local_var_params['user_id'] is None):
+            raise ApiValueError("Missing the required parameter `user_id` when calling `add_user_to_role`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'user_id' in local_var_params:
+            path_params['userId'] = local_var_params['user_id']  # noqa: E501
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'create_application_request' in local_var_params:
-            body_params = local_var_params['create_application_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
 
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
+
+        return self.api_client.call_api(
+            '/api/roles/{id}/users/{userId}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def create_role(self, create_role_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Create Role  # noqa: E501
+
+        Creates a new Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_role(create_role_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param CreateRoleRequest create_role_request: Details of the role to be created (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: RoleResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_role_with_http_info(create_role_request, **kwargs)  # noqa: E501
+
+    def create_role_with_http_info(self, create_role_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Create Role  # noqa: E501
+
+        Creates a new Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_role_with_http_info(create_role_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param CreateRoleRequest create_role_request: Details of the role to be created (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(RoleResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['create_role_request']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_role" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'create_role_request' is set
+        if ('create_role_request' not in local_var_params or
+                local_var_params['create_role_request'] is None):
+            raise ApiValueError("Missing the required parameter `create_role_request` when calling `create_role`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'create_role_request' in local_var_params:
+            body_params = local_var_params['create_role_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "OAuthApplication",
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/applications', 'POST',
+            '/api/roles', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='RoleResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def delete_application(self, id, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] DeleteApplication: Delete Application  # noqa: E501
+    def delete_role(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Delete Role  # noqa: E501
 
-        Delete the specified application  # noqa: E501
+        Delete the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_application(id, async_req=True)
+        >>> thread = api.delete_role(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_application_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_role_with_http_info(id, **kwargs)  # noqa: E501
 
-    def delete_application_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] DeleteApplication: Delete Application  # noqa: E501
+    def delete_role_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Delete Role  # noqa: E501
 
-        Delete the specified application  # noqa: E501
+        Delete the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_application_with_http_info(id, async_req=True)
+        >>> thread = api.delete_role_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_application" % key
+                    " to method delete_role" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `delete_application`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_application`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_application`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `delete_application`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_role`")  # noqa: E501
+
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {}
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/applications/{id}', 'DELETE',
+            '/api/roles/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def get_application(self, id, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetApplication: Get Application  # noqa: E501
+    def get_role(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get Role  # noqa: E501
 
-        get the specified application, and optionally the OIDC secret  # noqa: E501
+        Get the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_application(id, async_req=True)
+        >>> thread = api.get_role(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param include_secret: Optional. If set to true, the application secrets will be returned in plain text
-        :type include_secret: bool
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: RoleResponse
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: OAuthApplication
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_application_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_role_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_application_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetApplication: Get Application  # noqa: E501
+    def get_role_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get Role  # noqa: E501
 
-        get the specified application, and optionally the OIDC secret  # noqa: E501
+        Get the specified role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_application_with_http_info(id, async_req=True)
+        >>> thread = api.get_role_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param include_secret: Optional. If set to true, the application secrets will be returned in plain text
-        :type include_secret: bool
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(RoleResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (OAuthApplication, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'id',
-            'include_secret'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_application" % key
+                    " to method get_role" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_application`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_application`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_application`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `get_application`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `get_role`")  # noqa: E501
+
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'include_secret' in local_var_params and local_var_params['include_secret'] is not None:  # noqa: E501
-            query_params.append(('includeSecret', local_var_params['include_secret']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "OAuthApplication",
-            404: None,
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/applications/{id}', 'GET',
+            '/api/roles/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='RoleResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def list_applications(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] ListApplications: List Applications  # noqa: E501
+    def list_roles(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] List Roles  # noqa: E501
 
-        List the available applications  # noqa: E501
+        List the available Roles  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_applications(async_req=True)
+        >>> thread = api.list_roles(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: list[RoleResponse]
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[OAuthApplication]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_applications_with_http_info(**kwargs)  # noqa: E501
+        return self.list_roles_with_http_info(**kwargs)  # noqa: E501
 
-    def list_applications_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] ListApplications: List Applications  # noqa: E501
+    def list_roles_with_http_info(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] List Roles  # noqa: E501
 
-        List the available applications  # noqa: E501
+        List the available Roles  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_applications_with_http_info(async_req=True)
+        >>> thread = api.list_roles_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(list[RoleResponse], status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (list[OAuthApplication], int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_applications" % key
+                    " to method list_roles" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
 
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
+
+        return self.api_client.call_api(
+            '/api/roles', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[RoleResponse]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def list_users_in_role(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get the users in the specified role.  # noqa: E501
+
+        List all Users in the specified Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_users_in_role(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: list[UserResponse]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.list_users_in_role_with_http_info(id, **kwargs)  # noqa: E501
+
+    def list_users_in_role_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get the users in the specified role.  # noqa: E501
+
+        List all Users in the specified Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.list_users_in_role_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(list[UserResponse], status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_users_in_role" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `list_users_in_role`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "list[OAuthApplication]",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/applications', 'GET',
+            '/api/roles/{id}/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='list[UserResponse]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def rotate_application_secrets(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
+    def remove_user_from_role(self, id, user_id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Remove User from Role  # noqa: E501
 
-        Rotate the secrets for the specified application  # noqa: E501
+        Removes the User from the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.rotate_application_secrets(id, async_req=True)
+        >>> thread = api.remove_user_from_role(id, user_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param str user_id: The unique identifier for the User (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: OAuthApplication
         """
         kwargs['_return_http_data_only'] = True
-        return self.rotate_application_secrets_with_http_info(id, **kwargs)  # noqa: E501
+        return self.remove_user_from_role_with_http_info(id, user_id, **kwargs)  # noqa: E501
 
-    def rotate_application_secrets_with_http_info(self, id, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets  # noqa: E501
+    def remove_user_from_role_with_http_info(self, id, user_id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Remove User from Role  # noqa: E501
 
-        Rotate the secrets for the specified application  # noqa: E501
+        Removes the User from the specified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.rotate_application_secrets_with_http_info(id, async_req=True)
+        >>> thread = api.remove_user_from_role_with_http_info(id, user_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: The unique identifier for the application (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the Role (required)
+        :param str user_id: The unique identifier for the User (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (OAuthApplication, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id', 'user_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method rotate_application_secrets" % key
+                    " to method remove_user_from_role" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `rotate_application_secrets`")  # noqa: E501
-
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) > 64):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `rotate_application_secrets`, length must be less than or equal to `64`")  # noqa: E501
-        if self.api_client.client_side_validation and ('id' in local_var_params and  # noqa: E501
-                                                        len(local_var_params['id']) < 1):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `rotate_application_secrets`, length must be greater than or equal to `1`")  # noqa: E501
-        if self.api_client.client_side_validation and 'id' in local_var_params and not re.search(r'^[a-zA-Z0-9\-_]+$', local_var_params['id']):  # noqa: E501
-            raise ApiValueError("Invalid value for parameter `id` when calling `rotate_application_secrets`, must conform to the pattern `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `remove_user_from_role`")  # noqa: E501
+        # verify the required parameter 'user_id' is set
+        if ('user_id' not in local_var_params or
+                local_var_params['user_id'] is None):
+            raise ApiValueError("Missing the required parameter `user_id` when calling `remove_user_from_role`")  # noqa: E501
+
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'user_id' in local_var_params:
+            path_params['userId'] = local_var_params['user_id']  # noqa: E501
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
 
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
+
+        return self.api_client.call_api(
+            '/api/roles/{id}/users/{userId}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_role(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Update Role  # noqa: E501
+
+        Update the specified Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_role(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role to be updated (required)
+        :param UpdateRoleRequest update_role_request: The new definition of the role
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: RoleResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.update_role_with_http_info(id, **kwargs)  # noqa: E501
+
+    def update_role_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Update Role  # noqa: E501
+
+        Update the specified Role  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_role_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the role to be updated (required)
+        :param UpdateRoleRequest update_role_request: The new definition of the role
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(RoleResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['id', 'update_role_request']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_role" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `update_role`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'update_role_request' in local_var_params:
+            body_params = local_var_params['update_role_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "OAuthApplication",
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/applications/{id}/lifecycle/$newsecret', 'POST',
+            '/api/roles/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='RoleResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/authentication_api.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api/users_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,734 +1,629 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from finbourne_identity.api_client import ApiClient
-from finbourne_identity.exceptions import (  # noqa: F401
+from finbourne_identity.exceptions import (
     ApiTypeError,
     ApiValueError
 )
-from finbourne_identity.models.authentication_information import AuthenticationInformation
-from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
-from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
-from finbourne_identity.models.support_access_request import SupportAccessRequest
-from finbourne_identity.models.support_access_response import SupportAccessResponse
-from finbourne_identity.models.support_roles_response import SupportRolesResponse
 
 
-class AuthenticationApi(object):
+class UsersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_authentication_information(self, **kwargs):  # noqa: E501
-        """GetAuthenticationInformation: Gets AuthenticationInformation  # noqa: E501
+    def create_user(self, create_user_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Create User  # noqa: E501
 
-        Get the AuthenticationInformation associated with the current domain. This includes all the  necessary information to login to this domain.  # noqa: E501
+        Create a new User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_authentication_information(async_req=True)
+        >>> thread = api.create_user(create_user_request, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param CreateUserRequest create_user_request: Details of the User to be created (required)
+        :param bool wait_for_reindex: Should the request wait until the newly created User is indexed (available in List) before returning
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: UserResponse
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AuthenticationInformation
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_authentication_information_with_http_info(**kwargs)  # noqa: E501
+        return self.create_user_with_http_info(create_user_request, **kwargs)  # noqa: E501
 
-    def get_authentication_information_with_http_info(self, **kwargs):  # noqa: E501
-        """GetAuthenticationInformation: Gets AuthenticationInformation  # noqa: E501
+    def create_user_with_http_info(self, create_user_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Create User  # noqa: E501
 
-        Get the AuthenticationInformation associated with the current domain. This includes all the  necessary information to login to this domain.  # noqa: E501
+        Create a new User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_authentication_information_with_http_info(async_req=True)
+        >>> thread = api.create_user_with_http_info(create_user_request, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param CreateUserRequest create_user_request: Details of the User to be created (required)
+        :param bool wait_for_reindex: Should the request wait until the newly created User is indexed (available in List) before returning
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(UserResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (AuthenticationInformation, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['create_user_request', 'wait_for_reindex']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_authentication_information" % key
+                    " to method create_user" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'create_user_request' is set
+        if ('create_user_request' not in local_var_params or
+                local_var_params['create_user_request'] is None):
+            raise ApiValueError("Missing the required parameter `create_user_request` when calling `create_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'wait_for_reindex' in local_var_params:
+            query_params.append(('waitForReindex', local_var_params['wait_for_reindex']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'create_user_request' in local_var_params:
+            body_params = local_var_params['create_user_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "AuthenticationInformation",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/authentication/information', 'GET',
+            '/api/users', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='UserResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def get_support_access_history(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
+    def delete_user(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Delete User  # noqa: E501
 
-        The active and inactive support requests will be returned, inactive support requests will have information pertaining to their termination  including obfuscated userIds of those who created and terminated the request  # noqa: E501
+        By default the user will be de-provisioned and inactive, however their record will remain in the identity  provider for audit purposes. If this is not desirable and removal of all trace of the user is required,  the purge parameter can be specified to indicate the details should be purged completely.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_support_access_history(async_req=True)
+        >>> thread = api.delete_user(id, async_req=True)
         >>> result = thread.get()
 
-        :param start: The start expiry date to query support access requests from
-        :type start: datetime
-        :param end: The end expiry date to query support access requests to
-        :type end: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the user (required)
+        :param bool purge: Whether to purge any trace of the user from the identity provider (will affect audit)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[SupportAccessResponse]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_support_access_history_with_http_info(**kwargs)  # noqa: E501
+        return self.delete_user_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_support_access_history_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination  # noqa: E501
+    def delete_user_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Delete User  # noqa: E501
 
-        The active and inactive support requests will be returned, inactive support requests will have information pertaining to their termination  including obfuscated userIds of those who created and terminated the request  # noqa: E501
+        By default the user will be de-provisioned and inactive, however their record will remain in the identity  provider for audit purposes. If this is not desirable and removal of all trace of the user is required,  the purge parameter can be specified to indicate the details should be purged completely.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_support_access_history_with_http_info(async_req=True)
+        >>> thread = api.delete_user_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param start: The start expiry date to query support access requests from
-        :type start: datetime
-        :param end: The end expiry date to query support access requests to
-        :type end: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the user (required)
+        :param bool purge: Whether to purge any trace of the user from the identity provider (will affect audit)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (list[SupportAccessResponse], int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'start',
-            'end'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id', 'purge']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_support_access_history" % key
+                    " to method delete_user" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
-        if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
-            query_params.append(('start', local_var_params['start']))  # noqa: E501
-        if 'end' in local_var_params and local_var_params['end'] is not None:  # noqa: E501
-            query_params.append(('end', local_var_params['end']))  # noqa: E501
+        if 'purge' in local_var_params:
+            query_params.append(('purge', local_var_params['purge']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "list[SupportAccessResponse]",
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/authentication/support', 'GET',
+            '/api/users/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def get_support_roles(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+    def get_user(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get User  # noqa: E501
 
-        Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+        Get the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_support_roles(async_req=True)
+        >>> thread = api.get_user(id, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the User (required)
+        :param bool include_roles: Flag indicating that the users roles should be included in the response
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: UserResponse
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: SupportRolesResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_support_roles_with_http_info(**kwargs)  # noqa: E501
+        return self.get_user_with_http_info(id, **kwargs)  # noqa: E501
 
-    def get_support_roles_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+    def get_user_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Get User  # noqa: E501
 
-        Get mapping of support roles, the internal representation to a human friendly representation  # noqa: E501
+        Get the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_support_roles_with_http_info(async_req=True)
+        >>> thread = api.get_user_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the User (required)
+        :param bool include_roles: Flag indicating that the users roles should be included in the response
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(UserResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (SupportRolesResponse, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id', 'include_roles']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_support_roles" % key
+                    " to method get_user" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `get_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
+        if 'include_roles' in local_var_params:
+            query_params.append(('includeRoles', local_var_params['include_roles']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "SupportRolesResponse",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/authentication/support-roles', 'GET',
+            '/api/users/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='UserResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def grant_support_access(self, support_access_request, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
+    def list_users(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] List Users  # noqa: E501
 
-        Granting support access will allow FINBOURNE employees full access to your data with the express intent to investigate support issues  You can revoke this (and all) access at any time using the InvalidateSupportAccess endpoint.  # noqa: E501
+        List the available Users  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.grant_support_access(support_access_request, async_req=True)
+        >>> thread = api.list_users(async_req=True)
         >>> result = thread.get()
 
-        :param support_access_request: Request detailing the duration and reasons for supplying support access (required)
-        :type support_access_request: SupportAccessRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param bool include_roles: Flag indicating that the users roles should be included in the response
+        :param bool include_deactivated: Include previously deleted (not purged) users
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: list[UserResponse]
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: SupportAccessResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.grant_support_access_with_http_info(support_access_request, **kwargs)  # noqa: E501
+        return self.list_users_with_http_info(**kwargs)  # noqa: E501
 
-    def grant_support_access_with_http_info(self, support_access_request, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account  # noqa: E501
+    def list_users_with_http_info(self, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] List Users  # noqa: E501
 
-        Granting support access will allow FINBOURNE employees full access to your data with the express intent to investigate support issues  You can revoke this (and all) access at any time using the InvalidateSupportAccess endpoint.  # noqa: E501
+        List the available Users  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.grant_support_access_with_http_info(support_access_request, async_req=True)
+        >>> thread = api.list_users_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param support_access_request: Request detailing the duration and reasons for supplying support access (required)
-        :type support_access_request: SupportAccessRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param bool include_roles: Flag indicating that the users roles should be included in the response
+        :param bool include_deactivated: Include previously deleted (not purged) users
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(list[UserResponse], status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (SupportAccessResponse, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'support_access_request'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['include_roles', 'include_deactivated']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method grant_support_access" % key
+                    " to method list_users" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'support_access_request' is set
-        if self.api_client.client_side_validation and ('support_access_request' not in local_var_params or  # noqa: E501
-                                                        local_var_params['support_access_request'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `support_access_request` when calling `grant_support_access`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'include_roles' in local_var_params:
+            query_params.append(('includeRoles', local_var_params['include_roles']))  # noqa: E501
+        if 'include_deactivated' in local_var_params:
+            query_params.append(('includeDeactivated', local_var_params['include_deactivated']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'support_access_request' in local_var_params:
-            body_params = local_var_params['support_access_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            201: "SupportAccessResponse",
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/authentication/support', 'POST',
+            '/api/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='list[UserResponse]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def invalidate_support_access(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
+    def update_user(self, id, update_user_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Update User  # noqa: E501
 
-        This will result in a loss of access to your data for all FINBOURNE support agents  # noqa: E501
+        Updates the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.invalidate_support_access(async_req=True)
+        >>> thread = api.update_user(id, update_user_request, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the User to be updated (required)
+        :param UpdateUserRequest update_user_request: The new definition of the User (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: UserResponse
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[SupportAccessResponse]
         """
         kwargs['_return_http_data_only'] = True
-        return self.invalidate_support_access_with_http_info(**kwargs)  # noqa: E501
+        return self.update_user_with_http_info(id, update_user_request, **kwargs)  # noqa: E501
 
-    def invalidate_support_access_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account  # noqa: E501
+    def update_user_with_http_info(self, id, update_user_request, **kwargs):  # noqa: E501
+        """[EARLY ACCESS] Update User  # noqa: E501
 
-        This will result in a loss of access to your data for all FINBOURNE support agents  # noqa: E501
+        Updates the specified User  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.invalidate_support_access_with_http_info(async_req=True)
+        >>> thread = api.update_user_with_http_info(id, update_user_request, async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param str id: The unique identifier for the User to be updated (required)
+        :param UpdateUserRequest update_user_request: The new definition of the User (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(UserResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (list[SupportAccessResponse], int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['id', 'update_user_request']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method invalidate_support_access" % key
+                    " to method update_user" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `update_user`")  # noqa: E501
+        # verify the required parameter 'update_user_request' is set
+        if ('update_user_request' not in local_var_params or
+                local_var_params['update_user_request'] is None):
+            raise ApiValueError("Missing the required parameter `update_user_request` when calling `update_user`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'update_user_request' in local_var_params:
+            body_params = local_var_params['update_user_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "list[SupportAccessResponse]",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/authentication/support', 'DELETE',
+            '/api/users/{id}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='UserResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/identity_provider_api.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api/personal_authentication_tokens_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,318 +1,378 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from finbourne_identity.api_client import ApiClient
-from finbourne_identity.exceptions import (  # noqa: F401
+from finbourne_identity.exceptions import (
     ApiTypeError,
     ApiValueError
 )
-from finbourne_identity.models.add_scim_response import AddScimResponse
-from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
-from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
 
 
-class IdentityProviderApi(object):
+class PersonalAuthenticationTokensApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def add_scim(self, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] AddScim: Add SCIM  # noqa: E501
+    def create_api_key(self, create_api_key, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Create a Personal Access Token  # noqa: E501
 
-        Generates an API token to be used for SCIM  # noqa: E501
+        Generates a Personal Access Token and returns the new key and its associated metadata.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.add_scim(async_req=True)
+        >>> thread = api.create_api_key(create_api_key, async_req=True)
         >>> result = thread.get()
 
-        :param api_token_action: The action to take. For the API token. Defaults to \"ensure\"
-        :type api_token_action: str
-        :param old_api_token_deactivation: Optional deactivation date for the old API token. Only used if apiTokenAction is \"regenerate\"
-        :type old_api_token_deactivation: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param CreateApiKey create_api_key: The request to create a new Personal Access Token (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: CreatedApiKey
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AddScimResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.add_scim_with_http_info(**kwargs)  # noqa: E501
+        return self.create_api_key_with_http_info(create_api_key, **kwargs)  # noqa: E501
 
-    def add_scim_with_http_info(self, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] AddScim: Add SCIM  # noqa: E501
+    def create_api_key_with_http_info(self, create_api_key, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Create a Personal Access Token  # noqa: E501
 
-        Generates an API token to be used for SCIM  # noqa: E501
+        Generates a Personal Access Token and returns the new key and its associated metadata.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.add_scim_with_http_info(async_req=True)
+        >>> thread = api.create_api_key_with_http_info(create_api_key, async_req=True)
         >>> result = thread.get()
 
-        :param api_token_action: The action to take. For the API token. Defaults to \"ensure\"
-        :type api_token_action: str
-        :param old_api_token_deactivation: Optional deactivation date for the old API token. Only used if apiTokenAction is \"regenerate\"
-        :type old_api_token_deactivation: datetime
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
+        :param CreateApiKey create_api_key: The request to create a new Personal Access Token (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(CreatedApiKey, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: (AddScimResponse, int, HTTPHeaderDict)
         """
 
         local_var_params = locals()
 
-        all_params = [
-            'api_token_action',
-            'old_api_token_deactivation'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = ['create_api_key']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method add_scim" % key
+                    " to method create_api_key" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'create_api_key' is set
+        if ('create_api_key' not in local_var_params or
+                local_var_params['create_api_key'] is None):
+            raise ApiValueError("Missing the required parameter `create_api_key` when calling `create_api_key`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'api_token_action' in local_var_params and local_var_params['api_token_action'] is not None:  # noqa: E501
-            query_params.append(('apiTokenAction', local_var_params['api_token_action']))  # noqa: E501
-        if 'old_api_token_deactivation' in local_var_params and local_var_params['old_api_token_deactivation'] is not None:  # noqa: E501
-            query_params.append(('oldApiTokenDeactivation', local_var_params['old_api_token_deactivation']))  # noqa: E501
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'create_api_key' in local_var_params:
+            body_params = local_var_params['create_api_key']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
+        # Authentication setting
+        auth_settings = ['oauth2']  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
+
+        return self.api_client.call_api(
+            '/api/keys', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='CreatedApiKey',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_api_key(self, id, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Invalidate a Personal Access Token  # noqa: E501
+
+        Immediately invalidates the specified Personal Access Token  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_api_key(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The id of the Personal Access Token to delete (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ApiKey
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_api_key_with_http_info(id, **kwargs)  # noqa: E501
+
+    def delete_api_key_with_http_info(self, id, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Invalidate a Personal Access Token  # noqa: E501
+
+        Immediately invalidates the specified Personal Access Token  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_api_key_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The id of the Personal Access Token to delete (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ApiKey, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_api_key" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in local_var_params or
+                local_var_params['id'] is None):
+            raise ApiValueError("Missing the required parameter `id` when calling `delete_api_key`")  # noqa: E501
+
+        if ('id' in local_var_params and
+                len(local_var_params['id']) > 128):
+            raise ApiValueError("Invalid value for parameter `id` when calling `delete_api_key`, length must be less than or equal to `128`")  # noqa: E501
+        if ('id' in local_var_params and
+                len(local_var_params['id']) < 0):
+            raise ApiValueError("Invalid value for parameter `id` when calling `delete_api_key`, length must be greater than or equal to `0`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {
-            200: "AddScimResponse",
-            400: "LusidValidationProblemDetails",
-        }
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/identityprovider/scim', 'PUT',
+            '/api/keys/{id}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='ApiKey',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
 
-    def remove_scim(self, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] RemoveScim: Remove SCIM  # noqa: E501
+    def list_own_api_keys(self, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
 
-        Deactivates any existing SCIM API token  # noqa: E501
+        Gets the meta data for all of the user's Personal Access Tokens that have not been deleted. They may be  invalid due to the deactivation date having passed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.remove_scim(async_req=True)
+        >>> thread = api.list_own_api_keys(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: list[ApiKey]
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.remove_scim_with_http_info(**kwargs)  # noqa: E501
+        return self.list_own_api_keys_with_http_info(**kwargs)  # noqa: E501
 
-    def remove_scim_with_http_info(self, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] RemoveScim: Remove SCIM  # noqa: E501
+    def list_own_api_keys_with_http_info(self, **kwargs):  # noqa: E501
+        """[EXPERIMENTAL] Gets the meta data for all of the user's existing Personal Access Tokens.  # noqa: E501
 
-        Deactivates any existing SCIM API token  # noqa: E501
+        Gets the meta data for all of the user's Personal Access Tokens that have not been deleted. They may be  invalid due to the deactivation date having passed.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.remove_scim_with_http_info(async_req=True)
+        >>> thread = api.list_own_api_keys_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: tuple(list[ApiKey], status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method remove_scim" % key
+                    " to method list_own_api_keys" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {}
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
-            '/api/identityprovider/scim', 'DELETE',
+            '/api/keys', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type='list[ApiKey]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api/tokens_api.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api/tokens_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
 from finbourne_identity.api_client import ApiClient
-from finbourne_identity.exceptions import (  # noqa: F401
+from finbourne_identity.exceptions import (
     ApiTypeError,
     ApiValueError
 )
-from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
 
 
 class TokensApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -35,88 +34,68 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def invalidate_token(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
+        """[EXPERIMENTAL] Invalidate current JWT token (sign out)  # noqa: E501
 
         Log the current user out of all Finbourne platforms by invalidating the current token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.invalidate_token(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: Returns the result object.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
         return self.invalidate_token_with_http_info(**kwargs)  # noqa: E501
 
     def invalidate_token_with_http_info(self, **kwargs):  # noqa: E501
-        """[EARLY ACCESS] InvalidateToken: Invalidate current JWT token (sign out)  # noqa: E501
+        """[EXPERIMENTAL] Invalidate current JWT token (sign out)  # noqa: E501
 
         Log the current user out of all Finbourne platforms by invalidating the current token  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.invalidate_token_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
+        :param async_req bool: execute request asynchronously
         :param _return_http_data_only: response data without head status code
                                        and headers
-        :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
-        :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object, the HTTP status code, and the headers.
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
         """
 
         local_var_params = locals()
 
-        all_params = [
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_headers'
-            ]
-        )
+        all_params = []  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method invalidate_token" % key
                 )
@@ -125,45 +104,40 @@
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
-        header_params = dict(local_var_params.get('_headers', {}))
+        header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        header_params['Accept-Encoding'] = "gzip, deflate, br"
-
-
-        # set the LUSID header
-        header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.2469'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
-        response_types_map = {}
+        # set the LUSID header
+        header_params['X-LUSID-SDK-Language'] = 'Python'
+        header_params['X-LUSID-SDK-Version'] = '0.0.840'
 
         return self.api_client.call_api(
             '/api/tokens', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_types_map=response_types_map,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
+            collection_formats=collection_formats)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/api_client.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # coding: utf-8
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
-import atexit
 import datetime
-from dateutil.parser import parse
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
 from finbourne_identity.configuration import Configuration
 import finbourne_identity.models
 from finbourne_identity import rest
-from finbourne_identity.exceptions import ApiValueError, ApiException
+from finbourne_identity.exceptions import ApiValueError
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -65,48 +63,38 @@
         'object': object,
     }
     _pool = None
 
     def __init__(self, configuration=None, header_name=None, header_value=None,
                  cookie=None, pool_threads=1):
         if configuration is None:
-            configuration = Configuration.get_default_copy()
+            configuration = Configuration()
         self.configuration = configuration
         self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.2469/python'
-        self.client_side_validation = configuration.client_side_validation
+        self.user_agent = 'OpenAPI-Generator/0.0.840/python'
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.close()
-
-    def close(self):
+    def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
-            if hasattr(atexit, 'unregister'):
-                atexit.unregister(self.close)
 
     @property
     def pool(self):
         """Create thread pool on first request
          avoids instantiating unused threadpool for blocking clients.
         """
         if self._pool is None:
-            atexit.register(self.close)
             self._pool = ThreadPool(self.pool_threads)
         return self._pool
 
     @property
     def user_agent(self):
         """User agent for this API client"""
         return self.default_headers['User-Agent']
@@ -117,18 +105,17 @@
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
-            files=None, response_types_map=None, auth_settings=None,
+            files=None, response_type=None, auth_settings=None,
             _return_http_data_only=None, collection_formats=None,
-            _preload_content=True, _request_timeout=None, _host=None,
-            _request_auth=None):
+            _preload_content=True, _request_timeout=None, _host=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
@@ -161,63 +148,43 @@
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(post_params,
                                                     collection_formats)
             post_params.extend(self.files_parameters(files))
 
         # auth setting
-        self.update_params_for_auth(
-            header_params, query_params, auth_settings,
-            request_auth=_request_auth)
+        self.update_params_for_auth(header_params, query_params, auth_settings)
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
         else:
             # use server/host defined in path or operation instead
             url = _host + resource_path
 
-        try:
-            # perform request and return response
-            response_data = self.request(
-                method, url, query_params=query_params, headers=header_params,
-                post_params=post_params, body=body,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout)
-        except ApiException as e:
-            e.body = e.body.decode('utf-8') if six.PY3 else e.body
-            raise e
+        # perform request and return response
+        response_data = self.request(
+            method, url, query_params=query_params, headers=header_params,
+            post_params=post_params, body=body,
+            _preload_content=_preload_content,
+            _request_timeout=_request_timeout)
 
         self.last_response = response_data
 
         return_data = response_data
-
-        if not _preload_content:
-            return return_data
-        
-        response_type = response_types_map.get(response_data.status, None)
-
-        if six.PY3 and response_type not in ["file", "bytes"]:
-            match = None
-            content_type = response_data.getheader('content-type')
-            if content_type is not None:
-                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
-            encoding = match.group(1) if match else "utf-8"
-            response_data.data = response_data.data.decode(encoding)
-
-        # deserialize response data
-        
-        if response_type:
-            return_data = self.deserialize(response_data, response_type)
-        else:
-            return_data = None
+        if _preload_content:
+            # deserialize response data
+            if response_type:
+                return_data = self.deserialize(response_data, response_type)
+            else:
+                return_data = None
 
         if _return_http_data_only:
             return (return_data)
         else:
             return (return_data, response_data.status,
                     response_data.getheaders())
 
@@ -316,25 +283,24 @@
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
-            return self.__deserialize_datetime(data)
+            return self.__deserialize_datatime(data)
         else:
             return self.__deserialize_model(data, klass)
 
     def call_api(self, resource_path, method,
                  path_params=None, query_params=None, header_params=None,
                  body=None, post_params=None, files=None,
-                 response_types_map=None, auth_settings=None,
-                 async_req=None, _return_http_data_only=None,
-                 collection_formats=None,_preload_content=True,
-                  _request_timeout=None, _host=None, _request_auth=None):
+                 response_type=None, auth_settings=None, async_req=None,
+                 _return_http_data_only=None, collection_formats=None,
+                 _preload_content=True, _request_timeout=None, _host=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -356,46 +322,40 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_token: dict, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
-                                   response_types_map, auth_settings,
+                                   response_type, auth_settings,
                                    _return_http_data_only, collection_formats,
-                                   _preload_content, _request_timeout, _host,
-                                   _request_auth)
-
-        return self.pool.apply_async(self.__call_api, (resource_path,
-                                                       method, path_params,
-                                                       query_params,
-                                                       header_params, body,
-                                                       post_params, files,
-                                                       response_types_map,
-                                                       auth_settings,
-                                                       _return_http_data_only,
-                                                       collection_formats,
-                                                       _preload_content,
-                                                       _request_timeout,
-                                                       _host, _request_auth))
+                                   _preload_content, _request_timeout, _host)
+        else:
+            thread = self.pool.apply_async(self.__call_api, (resource_path,
+                                           method, path_params, query_params,
+                                           header_params, body,
+                                           post_params, files,
+                                           response_type, auth_settings,
+                                           _return_http_data_only,
+                                           collection_formats,
+                                           _preload_content,
+                                           _request_timeout,
+                                           _host))
+        return thread
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
                 _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return self.rest_client.GET(url,
@@ -409,16 +369,18 @@
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
                                          headers=headers)
         elif method == "OPTIONS":
             return self.rest_client.OPTIONS(url,
                                             query_params=query_params,
                                             headers=headers,
+                                            post_params=post_params,
                                             _preload_content=_preload_content,
-                                            _request_timeout=_request_timeout)
+                                            _request_timeout=_request_timeout,
+                                            body=body)
         elif method == "POST":
             return self.rest_client.POST(url,
                                          query_params=query_params,
                                          headers=headers,
                                          post_params=post_params,
                                          _preload_content=_preload_content,
                                          _request_timeout=_request_timeout,
@@ -534,53 +496,39 @@
         content_types = [x.lower() for x in content_types]
 
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, querys, auth_settings,
-                               request_auth=None):
+    def update_params_for_auth(self, headers, querys, auth_settings):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param querys: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
-        :param request_auth: if set, the provided settings will
-                             override the token in the configuration.
         """
         if not auth_settings:
             return
 
-        if request_auth:
-            self._apply_auth_params(headers, querys, request_auth)
-            return
-
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                self._apply_auth_params(headers, querys, auth_setting)
-
-    def _apply_auth_params(self, headers, querys, auth_setting):
-        """Updates the request parameters based on a single auth_setting
-
-        :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
-        :param auth_setting: auth settings for the endpoint
-        """
-        if auth_setting['in'] == 'cookie':
-            headers['Cookie'] = auth_setting['value']
-        elif auth_setting['in'] == 'header':
-            headers[auth_setting['key']] = auth_setting['value']
-        elif auth_setting['in'] == 'query':
-            querys.append((auth_setting['key'], auth_setting['value']))
-        else:
-            raise ApiValueError(
-                'Authentication token must be in `query` or `header`'
-            )
+                if not auth_setting['value']:
+                    continue
+                elif auth_setting['in'] == 'cookie':
+                    headers['Cookie'] = auth_setting['value']
+                elif auth_setting['in'] == 'header':
+                    headers[auth_setting['key']] = auth_setting['value']
+                elif auth_setting['in'] == 'query':
+                    querys.append((auth_setting['key'], auth_setting['value']))
+                else:
+                    raise ApiValueError(
+                        'Authentication token must be in `query` or `header`'
+                    )
 
     def __deserialize_file(self, response):
         """Deserializes body to file
 
         Saves response body into a file in a temporary folder,
         using the filename from the `Content-Disposition` header if provided.
 
@@ -627,32 +575,34 @@
     def __deserialize_date(self, string):
         """Deserializes string to date.
 
         :param string: str.
         :return: date.
         """
         try:
+            from dateutil.parser import parse
             return parse(string).date()
         except ImportError:
             return string
         except ValueError:
             raise rest.ApiException(
                 status=0,
                 reason="Failed to parse `{0}` as date object".format(string)
             )
 
-    def __deserialize_datetime(self, string):
+    def __deserialize_datatime(self, string):
         """Deserializes string to datetime.
 
         The string should be in iso8601 datetime format.
 
         :param string: str.
         :return: datetime.
         """
         try:
+            from dateutil.parser import parse
             return parse(string)
         except ImportError:
             return string
         except ValueError:
             raise rest.ApiException(
                 status=0,
                 reason=(
@@ -664,31 +614,28 @@
     def __deserialize_model(self, data, klass):
         """Deserializes list or dict to model.
 
         :param data: dict, list.
         :param klass: class literal.
         :return: model object.
         """
-        has_discriminator = False
-        if (hasattr(klass, 'get_real_child_model')
-                and klass.discriminator_value_class_map):
-            has_discriminator = True
 
-        if not klass.openapi_types and has_discriminator is False:
+        if not klass.openapi_types and not hasattr(klass,
+                                                   'get_real_child_model'):
             return data
 
         kwargs = {}
-        if (data is not None and
-                klass.openapi_types is not None and
-                isinstance(data, (list, dict))):
+        if klass.openapi_types is not None:
             for attr, attr_type in six.iteritems(klass.openapi_types):
-                if klass.attribute_map[attr] in data:
+                if (data is not None and
+                        klass.attribute_map[attr] in data and
+                        isinstance(data, (list, dict))):
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
         instance = klass(**kwargs)
 
-        if has_discriminator:
+        if hasattr(instance, 'get_real_child_model'):
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/exceptions.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
 
@@ -61,33 +61,14 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
-class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Raised when an attribute reference or assignment fails.
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiAttributeError, self).__init__(full_msg)
-
-
 class ApiKeyError(OpenApiException, KeyError):
     def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -125,38 +106,14 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, six.integer_types):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/__init__.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from finbourne_identity.models.access_controlled_action import AccessControlledAction
 from finbourne_identity.models.access_controlled_resource import AccessControlledResource
 from finbourne_identity.models.action_id import ActionId
-from finbourne_identity.models.add_scim_response import AddScimResponse
+from finbourne_identity.models.agreement_response import AgreementResponse
 from finbourne_identity.models.api_key import ApiKey
 from finbourne_identity.models.authentication_information import AuthenticationInformation
 from finbourne_identity.models.create_api_key import CreateApiKey
 from finbourne_identity.models.create_application_request import CreateApplicationRequest
+from finbourne_identity.models.create_domain_request import CreateDomainRequest
 from finbourne_identity.models.create_role_request import CreateRoleRequest
 from finbourne_identity.models.create_user_request import CreateUserRequest
 from finbourne_identity.models.created_api_key import CreatedApiKey
-from finbourne_identity.models.current_user_response import CurrentUserResponse
-from finbourne_identity.models.error_detail import ErrorDetail
+from finbourne_identity.models.domain_id import DomainId
+from finbourne_identity.models.domain_response import DomainResponse
 from finbourne_identity.models.id_selector_definition import IdSelectorDefinition
 from finbourne_identity.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_identity.models.link import Link
-from finbourne_identity.models.list_users_response import ListUsersResponse
 from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
 from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from finbourne_identity.models.o_auth_application import OAuthApplication
+from finbourne_identity.models.problem_details import ProblemDetails
 from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
+from finbourne_identity.models.role import Role
 from finbourne_identity.models.role_id import RoleId
 from finbourne_identity.models.role_response import RoleResponse
-from finbourne_identity.models.set_password import SetPassword
-from finbourne_identity.models.set_password_response import SetPasswordResponse
 from finbourne_identity.models.support_access_expiry import SupportAccessExpiry
-from finbourne_identity.models.support_access_expiry_with_role import SupportAccessExpiryWithRole
 from finbourne_identity.models.support_access_request import SupportAccessRequest
 from finbourne_identity.models.support_access_response import SupportAccessResponse
-from finbourne_identity.models.support_role import SupportRole
-from finbourne_identity.models.support_roles_response import SupportRolesResponse
-from finbourne_identity.models.temporary_password import TemporaryPassword
 from finbourne_identity.models.update_role_request import UpdateRoleRequest
 from finbourne_identity.models.update_user_request import UpdateUserRequest
+from finbourne_identity.models.user_id import UserId
 from finbourne_identity.models.user_response import UserResponse
-from finbourne_identity.models.user_summary import UserSummary
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/access_controlled_action.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/access_controlled_action.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class AccessControlledAction(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -55,30 +49,28 @@
     required_map = {
         'description': 'required',
         'action': 'required',
         'limited_set': 'optional',
         'links': 'optional'
     }
 
-    def __init__(self, description=None, action=None, limited_set=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """AccessControlledAction - a model defined in OpenAPI"
-        
+    def __init__(self, description=None, action=None, limited_set=None, links=None):  # noqa: E501
+        """
+        AccessControlledAction - a model defined in OpenAPI
+
         :param description:  (required)
         :type description: str
         :param action:  (required)
         :type action: finbourne_identity.ActionId
         :param limited_set: 
         :type limited_set: list[finbourne_identity.IdSelectorDefinition]
         :param links: 
         :type links: list[finbourne_identity.Link]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._description = None
         self._action = None
         self._limited_set = None
         self._links = None
         self.discriminator = None
 
@@ -99,118 +91,107 @@
 
     @description.setter
     def description(self, description):
         """Sets the description of this AccessControlledAction.
 
 
         :param description: The description of this AccessControlledAction.  # noqa: E501
-        :type description: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
+        if description is None:
             raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 1):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._description = description
 
     @property
     def action(self):
         """Gets the action of this AccessControlledAction.  # noqa: E501
 
 
         :return: The action of this AccessControlledAction.  # noqa: E501
-        :rtype: finbourne_identity.ActionId
+        :rtype: ActionId
         """
         return self._action
 
     @action.setter
     def action(self, action):
         """Sets the action of this AccessControlledAction.
 
 
         :param action: The action of this AccessControlledAction.  # noqa: E501
-        :type action: finbourne_identity.ActionId
+        :type: ActionId
         """
-        if self.local_vars_configuration.client_side_validation and action is None:  # noqa: E501
+        if action is None:
             raise ValueError("Invalid value for `action`, must not be `None`")  # noqa: E501
 
         self._action = action
 
     @property
     def limited_set(self):
         """Gets the limited_set of this AccessControlledAction.  # noqa: E501
 
 
         :return: The limited_set of this AccessControlledAction.  # noqa: E501
-        :rtype: list[finbourne_identity.IdSelectorDefinition]
+        :rtype: list[IdSelectorDefinition]
         """
         return self._limited_set
 
     @limited_set.setter
     def limited_set(self, limited_set):
         """Sets the limited_set of this AccessControlledAction.
 
 
         :param limited_set: The limited_set of this AccessControlledAction.  # noqa: E501
-        :type limited_set: list[finbourne_identity.IdSelectorDefinition]
+        :type: list[IdSelectorDefinition]
         """
 
         self._limited_set = limited_set
 
     @property
     def links(self):
         """Gets the links of this AccessControlledAction.  # noqa: E501
 
 
         :return: The links of this AccessControlledAction.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :rtype: list[Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
         """Sets the links of this AccessControlledAction.
 
 
         :param links: The links of this AccessControlledAction.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :type: list[Link]
         """
 
         self._links = links
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -219,15 +200,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, AccessControlledAction):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AccessControlledAction):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/access_controlled_resource.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/access_controlled_resource.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class AccessControlledResource(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -61,34 +55,32 @@
         'name': 'optional',
         'description': 'required',
         'actions': 'required',
         'identifier_parts': 'optional',
         'links': 'optional'
     }
 
-    def __init__(self, application=None, name=None, description=None, actions=None, identifier_parts=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """AccessControlledResource - a model defined in OpenAPI"
-        
+    def __init__(self, application=None, name=None, description=None, actions=None, identifier_parts=None, links=None):  # noqa: E501
+        """
+        AccessControlledResource - a model defined in OpenAPI
+
         :param application: 
         :type application: str
         :param name: 
         :type name: str
         :param description:  (required)
         :type description: str
         :param actions:  (required)
         :type actions: list[finbourne_identity.AccessControlledAction]
         :param identifier_parts: 
         :type identifier_parts: list[finbourne_identity.IdentifierPartSchema]
         :param links: 
         :type links: list[finbourne_identity.Link]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._application = None
         self._name = None
         self._description = None
         self._actions = None
         self._identifier_parts = None
         self._links = None
@@ -113,15 +105,15 @@
 
     @application.setter
     def application(self, application):
         """Sets the application of this AccessControlledResource.
 
 
         :param application: The application of this AccessControlledResource.  # noqa: E501
-        :type application: str
+        :type: str
         """
 
         self._application = application
 
     @property
     def name(self):
         """Gets the name of this AccessControlledResource.  # noqa: E501
@@ -134,15 +126,15 @@
 
     @name.setter
     def name(self, name):
         """Sets the name of this AccessControlledResource.
 
 
         :param name: The name of this AccessControlledResource.  # noqa: E501
-        :type name: str
+        :type: str
         """
 
         self._name = name
 
     @property
     def description(self):
         """Gets the description of this AccessControlledResource.  # noqa: E501
@@ -155,118 +147,107 @@
 
     @description.setter
     def description(self, description):
         """Sets the description of this AccessControlledResource.
 
 
         :param description: The description of this AccessControlledResource.  # noqa: E501
-        :type description: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
+        if description is None:
             raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 1):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._description = description
 
     @property
     def actions(self):
         """Gets the actions of this AccessControlledResource.  # noqa: E501
 
 
         :return: The actions of this AccessControlledResource.  # noqa: E501
-        :rtype: list[finbourne_identity.AccessControlledAction]
+        :rtype: list[AccessControlledAction]
         """
         return self._actions
 
     @actions.setter
     def actions(self, actions):
         """Sets the actions of this AccessControlledResource.
 
 
         :param actions: The actions of this AccessControlledResource.  # noqa: E501
-        :type actions: list[finbourne_identity.AccessControlledAction]
+        :type: list[AccessControlledAction]
         """
-        if self.local_vars_configuration.client_side_validation and actions is None:  # noqa: E501
+        if actions is None:
             raise ValueError("Invalid value for `actions`, must not be `None`")  # noqa: E501
 
         self._actions = actions
 
     @property
     def identifier_parts(self):
         """Gets the identifier_parts of this AccessControlledResource.  # noqa: E501
 
 
         :return: The identifier_parts of this AccessControlledResource.  # noqa: E501
-        :rtype: list[finbourne_identity.IdentifierPartSchema]
+        :rtype: list[IdentifierPartSchema]
         """
         return self._identifier_parts
 
     @identifier_parts.setter
     def identifier_parts(self, identifier_parts):
         """Sets the identifier_parts of this AccessControlledResource.
 
 
         :param identifier_parts: The identifier_parts of this AccessControlledResource.  # noqa: E501
-        :type identifier_parts: list[finbourne_identity.IdentifierPartSchema]
+        :type: list[IdentifierPartSchema]
         """
 
         self._identifier_parts = identifier_parts
 
     @property
     def links(self):
         """Gets the links of this AccessControlledResource.  # noqa: E501
 
 
         :return: The links of this AccessControlledResource.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :rtype: list[Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
         """Sets the links of this AccessControlledResource.
 
 
         :param links: The links of this AccessControlledResource.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :type: list[Link]
         """
 
         self._links = links
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -275,15 +256,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, AccessControlledResource):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AccessControlledResource):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/action_id.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/action_id.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class ActionId(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -52,28 +46,26 @@
 
     required_map = {
         'scope': 'required',
         'activity': 'required',
         'entity': 'required'
     }
 
-    def __init__(self, scope=None, activity=None, entity=None, local_vars_configuration=None):  # noqa: E501
-        """ActionId - a model defined in OpenAPI"
-        
+    def __init__(self, scope=None, activity=None, entity=None):  # noqa: E501
+        """
+        ActionId - a model defined in OpenAPI
+
         :param scope:  (required)
         :type scope: str
         :param activity:  (required)
         :type activity: str
         :param entity:  (required)
         :type entity: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._scope = None
         self._activity = None
         self._entity = None
         self.discriminator = None
 
         self.scope = scope
@@ -92,23 +84,21 @@
 
     @scope.setter
     def scope(self, scope):
         """Sets the scope of this ActionId.
 
 
         :param scope: The scope of this ActionId.  # noqa: E501
-        :type scope: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and scope is None:  # noqa: E501
+        if scope is None:
             raise ValueError("Invalid value for `scope`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                scope is not None and len(scope) > 100):
+        if scope is not None and len(scope) > 100:
             raise ValueError("Invalid value for `scope`, length must be less than or equal to `100`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                scope is not None and len(scope) < 3):
+        if scope is not None and len(scope) < 3:
             raise ValueError("Invalid value for `scope`, length must be greater than or equal to `3`")  # noqa: E501
 
         self._scope = scope
 
     @property
     def activity(self):
         """Gets the activity of this ActionId.  # noqa: E501
@@ -121,23 +111,21 @@
 
     @activity.setter
     def activity(self, activity):
         """Sets the activity of this ActionId.
 
 
         :param activity: The activity of this ActionId.  # noqa: E501
-        :type activity: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and activity is None:  # noqa: E501
+        if activity is None:
             raise ValueError("Invalid value for `activity`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                activity is not None and len(activity) > 25):
+        if activity is not None and len(activity) > 25:
             raise ValueError("Invalid value for `activity`, length must be less than or equal to `25`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                activity is not None and len(activity) < 3):
+        if activity is not None and len(activity) < 3:
             raise ValueError("Invalid value for `activity`, length must be greater than or equal to `3`")  # noqa: E501
 
         self._activity = activity
 
     @property
     def entity(self):
         """Gets the entity of this ActionId.  # noqa: E501
@@ -150,56 +138,46 @@
 
     @entity.setter
     def entity(self, entity):
         """Sets the entity of this ActionId.
 
 
         :param entity: The entity of this ActionId.  # noqa: E501
-        :type entity: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and entity is None:  # noqa: E501
+        if entity is None:
             raise ValueError("Invalid value for `entity`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                entity is not None and len(entity) > 25):
+        if entity is not None and len(entity) > 25:
             raise ValueError("Invalid value for `entity`, length must be less than or equal to `25`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                entity is not None and len(entity) < 3):
+        if entity is not None and len(entity) < 3:
             raise ValueError("Invalid value for `entity`, length must be greater than or equal to `3`")  # noqa: E501
 
         self._entity = entity
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -208,15 +186,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, ActionId):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ActionId):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/add_scim_response.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/link.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class AddScimResponse(object):
+class Link(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,136 +29,185 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'base_url': 'str',
-        'api_token': 'str'
+        'relation': 'str',
+        'href': 'str',
+        'description': 'str',
+        'method': 'str'
     }
 
     attribute_map = {
-        'base_url': 'baseUrl',
-        'api_token': 'apiToken'
+        'relation': 'relation',
+        'href': 'href',
+        'description': 'description',
+        'method': 'method'
     }
 
     required_map = {
-        'base_url': 'optional',
-        'api_token': 'optional'
+        'relation': 'required',
+        'href': 'required',
+        'description': 'optional',
+        'method': 'required'
     }
 
-    def __init__(self, base_url=None, api_token=None, local_vars_configuration=None):  # noqa: E501
-        """AddScimResponse - a model defined in OpenAPI"
-        
-        :param base_url: 
-        :type base_url: str
-        :param api_token: 
-        :type api_token: str
+    def __init__(self, relation=None, href=None, description=None, method=None):  # noqa: E501
+        """
+        Link - a model defined in OpenAPI
+
+        :param relation:  (required)
+        :type relation: str
+        :param href:  (required)
+        :type href: str
+        :param description: 
+        :type description: str
+        :param method:  (required)
+        :type method: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
-        self._base_url = None
-        self._api_token = None
+        self._relation = None
+        self._href = None
+        self._description = None
+        self._method = None
         self.discriminator = None
 
-        self.base_url = base_url
-        self.api_token = api_token
+        self.relation = relation
+        self.href = href
+        self.description = description
+        self.method = method
+
+    @property
+    def relation(self):
+        """Gets the relation of this Link.  # noqa: E501
+
+
+        :return: The relation of this Link.  # noqa: E501
+        :rtype: str
+        """
+        return self._relation
+
+    @relation.setter
+    def relation(self, relation):
+        """Sets the relation of this Link.
+
+
+        :param relation: The relation of this Link.  # noqa: E501
+        :type: str
+        """
+        if relation is None:
+            raise ValueError("Invalid value for `relation`, must not be `None`")  # noqa: E501
+
+        self._relation = relation
 
     @property
-    def base_url(self):
-        """Gets the base_url of this AddScimResponse.  # noqa: E501
+    def href(self):
+        """Gets the href of this Link.  # noqa: E501
 
 
-        :return: The base_url of this AddScimResponse.  # noqa: E501
+        :return: The href of this Link.  # noqa: E501
         :rtype: str
         """
-        return self._base_url
+        return self._href
 
-    @base_url.setter
-    def base_url(self, base_url):
-        """Sets the base_url of this AddScimResponse.
+    @href.setter
+    def href(self, href):
+        """Sets the href of this Link.
 
 
-        :param base_url: The base_url of this AddScimResponse.  # noqa: E501
-        :type base_url: str
+        :param href: The href of this Link.  # noqa: E501
+        :type: str
         """
+        if href is None:
+            raise ValueError("Invalid value for `href`, must not be `None`")  # noqa: E501
 
-        self._base_url = base_url
+        self._href = href
 
     @property
-    def api_token(self):
-        """Gets the api_token of this AddScimResponse.  # noqa: E501
+    def description(self):
+        """Gets the description of this Link.  # noqa: E501
 
 
-        :return: The api_token of this AddScimResponse.  # noqa: E501
+        :return: The description of this Link.  # noqa: E501
         :rtype: str
         """
-        return self._api_token
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Link.
+
+
+        :param description: The description of this Link.  # noqa: E501
+        :type: str
+        """
+
+        self._description = description
 
-    @api_token.setter
-    def api_token(self, api_token):
-        """Sets the api_token of this AddScimResponse.
+    @property
+    def method(self):
+        """Gets the method of this Link.  # noqa: E501
 
 
-        :param api_token: The api_token of this AddScimResponse.  # noqa: E501
-        :type api_token: str
+        :return: The method of this Link.  # noqa: E501
+        :rtype: str
         """
+        return self._method
 
-        self._api_token = api_token
+    @method.setter
+    def method(self, method):
+        """Sets the method of this Link.
 
-    def to_dict(self, serialize=False):
+
+        :param method: The method of this Link.  # noqa: E501
+        :type: str
+        """
+        if method is None:
+            raise ValueError("Invalid value for `method`, must not be `None`")  # noqa: E501
+
+        self._method = method
+
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AddScimResponse):
+        if not isinstance(other, Link):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AddScimResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/api_key.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/created_api_key.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class ApiKey(object):
+class CreatedApiKey(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,224 +29,225 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'key': 'str',
         'id': 'str',
         'display_name': 'str',
         'created_date': 'datetime',
         'deactivation_date': 'datetime'
     }
 
     attribute_map = {
+        'key': 'key',
         'id': 'id',
         'display_name': 'displayName',
         'created_date': 'createdDate',
         'deactivation_date': 'deactivationDate'
     }
 
     required_map = {
+        'key': 'required',
         'id': 'required',
         'display_name': 'required',
         'created_date': 'required',
         'deactivation_date': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, created_date=None, deactivation_date=None, local_vars_configuration=None):  # noqa: E501
-        """ApiKey - a model defined in OpenAPI"
-        
+    def __init__(self, key=None, id=None, display_name=None, created_date=None, deactivation_date=None):  # noqa: E501
+        """
+        CreatedApiKey - a model defined in OpenAPI
+
+        :param key:  The API Key value (required)
+        :type key: str
         :param id:  The unique Id of the API key (required)
         :type id: str
         :param display_name:  The display name of the API key (required)
         :type display_name: str
         :param created_date:  The creation date of the API key (required)
         :type created_date: datetime
         :param deactivation_date:  The deactivation date of the API key
         :type deactivation_date: datetime
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
+        self._key = None
         self._id = None
         self._display_name = None
         self._created_date = None
         self._deactivation_date = None
         self.discriminator = None
 
+        self.key = key
         self.id = id
         self.display_name = display_name
         self.created_date = created_date
         self.deactivation_date = deactivation_date
 
     @property
+    def key(self):
+        """Gets the key of this CreatedApiKey.  # noqa: E501
+
+        The API Key value  # noqa: E501
+
+        :return: The key of this CreatedApiKey.  # noqa: E501
+        :rtype: str
+        """
+        return self._key
+
+    @key.setter
+    def key(self, key):
+        """Sets the key of this CreatedApiKey.
+
+        The API Key value  # noqa: E501
+
+        :param key: The key of this CreatedApiKey.  # noqa: E501
+        :type: str
+        """
+        if key is None:
+            raise ValueError("Invalid value for `key`, must not be `None`")  # noqa: E501
+
+        self._key = key
+
+    @property
     def id(self):
-        """Gets the id of this ApiKey.  # noqa: E501
+        """Gets the id of this CreatedApiKey.  # noqa: E501
 
         The unique Id of the API key  # noqa: E501
 
-        :return: The id of this ApiKey.  # noqa: E501
+        :return: The id of this CreatedApiKey.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this ApiKey.
+        """Sets the id of this CreatedApiKey.
 
         The unique Id of the API key  # noqa: E501
 
-        :param id: The id of this ApiKey.  # noqa: E501
-        :type id: str
+        :param id: The id of this CreatedApiKey.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+        if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) > 64):
-            raise ValueError("Invalid value for `id`, length must be less than or equal to `64`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) < 1):
-            raise ValueError("Invalid value for `id`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', id)):  # noqa: E501
-            raise ValueError(r"Invalid value for `id`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
 
         self._id = id
 
     @property
     def display_name(self):
-        """Gets the display_name of this ApiKey.  # noqa: E501
+        """Gets the display_name of this CreatedApiKey.  # noqa: E501
 
         The display name of the API key  # noqa: E501
 
-        :return: The display_name of this ApiKey.  # noqa: E501
+        :return: The display_name of this CreatedApiKey.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this ApiKey.
+        """Sets the display_name of this CreatedApiKey.
 
         The display name of the API key  # noqa: E501
 
-        :param display_name: The display_name of this ApiKey.  # noqa: E501
-        :type display_name: str
+        :param display_name: The display_name of this CreatedApiKey.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+        if display_name is None:
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) > 512):
-            raise ValueError("Invalid value for `display_name`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def created_date(self):
-        """Gets the created_date of this ApiKey.  # noqa: E501
+        """Gets the created_date of this CreatedApiKey.  # noqa: E501
 
         The creation date of the API key  # noqa: E501
 
-        :return: The created_date of this ApiKey.  # noqa: E501
+        :return: The created_date of this CreatedApiKey.  # noqa: E501
         :rtype: datetime
         """
         return self._created_date
 
     @created_date.setter
     def created_date(self, created_date):
-        """Sets the created_date of this ApiKey.
+        """Sets the created_date of this CreatedApiKey.
 
         The creation date of the API key  # noqa: E501
 
-        :param created_date: The created_date of this ApiKey.  # noqa: E501
-        :type created_date: datetime
+        :param created_date: The created_date of this CreatedApiKey.  # noqa: E501
+        :type: datetime
         """
-        if self.local_vars_configuration.client_side_validation and created_date is None:  # noqa: E501
+        if created_date is None:
             raise ValueError("Invalid value for `created_date`, must not be `None`")  # noqa: E501
 
         self._created_date = created_date
 
     @property
     def deactivation_date(self):
-        """Gets the deactivation_date of this ApiKey.  # noqa: E501
+        """Gets the deactivation_date of this CreatedApiKey.  # noqa: E501
 
         The deactivation date of the API key  # noqa: E501
 
-        :return: The deactivation_date of this ApiKey.  # noqa: E501
+        :return: The deactivation_date of this CreatedApiKey.  # noqa: E501
         :rtype: datetime
         """
         return self._deactivation_date
 
     @deactivation_date.setter
     def deactivation_date(self, deactivation_date):
-        """Sets the deactivation_date of this ApiKey.
+        """Sets the deactivation_date of this CreatedApiKey.
 
         The deactivation date of the API key  # noqa: E501
 
-        :param deactivation_date: The deactivation_date of this ApiKey.  # noqa: E501
-        :type deactivation_date: datetime
+        :param deactivation_date: The deactivation_date of this CreatedApiKey.  # noqa: E501
+        :type: datetime
         """
 
         self._deactivation_date = deactivation_date
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiKey):
+        if not isinstance(other, CreatedApiKey):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiKey):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/authentication_information.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/authentication_information.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class AuthenticationInformation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -36,74 +30,58 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'issuer_url': 'str',
-        'fallback_issuer_urls': 'list[str]',
         'saml_identity_provider_id': 'str',
         'support': 'SupportAccessExpiry',
-        'support_access_expiry_with_role': 'list[SupportAccessExpiryWithRole]',
         'links': 'list[Link]'
     }
 
     attribute_map = {
         'issuer_url': 'issuerUrl',
-        'fallback_issuer_urls': 'fallbackIssuerUrls',
         'saml_identity_provider_id': 'samlIdentityProviderId',
         'support': 'support',
-        'support_access_expiry_with_role': 'supportAccessExpiryWithRole',
         'links': 'links'
     }
 
     required_map = {
         'issuer_url': 'required',
-        'fallback_issuer_urls': 'optional',
         'saml_identity_provider_id': 'optional',
         'support': 'optional',
-        'support_access_expiry_with_role': 'optional',
         'links': 'optional'
     }
 
-    def __init__(self, issuer_url=None, fallback_issuer_urls=None, saml_identity_provider_id=None, support=None, support_access_expiry_with_role=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """AuthenticationInformation - a model defined in OpenAPI"
-        
+    def __init__(self, issuer_url=None, saml_identity_provider_id=None, support=None, links=None):  # noqa: E501
+        """
+        AuthenticationInformation - a model defined in OpenAPI
+
         :param issuer_url:  (required)
         :type issuer_url: str
-        :param fallback_issuer_urls: 
-        :type fallback_issuer_urls: list[str]
         :param saml_identity_provider_id: 
         :type saml_identity_provider_id: str
         :param support: 
         :type support: finbourne_identity.SupportAccessExpiry
-        :param support_access_expiry_with_role: 
-        :type support_access_expiry_with_role: list[finbourne_identity.SupportAccessExpiryWithRole]
         :param links: 
         :type links: list[finbourne_identity.Link]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._issuer_url = None
-        self._fallback_issuer_urls = None
         self._saml_identity_provider_id = None
         self._support = None
-        self._support_access_expiry_with_role = None
         self._links = None
         self.discriminator = None
 
         self.issuer_url = issuer_url
-        self.fallback_issuer_urls = fallback_issuer_urls
         self.saml_identity_provider_id = saml_identity_provider_id
         if support is not None:
             self.support = support
-        self.support_access_expiry_with_role = support_access_expiry_with_role
         self.links = links
 
     @property
     def issuer_url(self):
         """Gets the issuer_url of this AuthenticationInformation.  # noqa: E501
 
 
@@ -114,46 +92,22 @@
 
     @issuer_url.setter
     def issuer_url(self, issuer_url):
         """Sets the issuer_url of this AuthenticationInformation.
 
 
         :param issuer_url: The issuer_url of this AuthenticationInformation.  # noqa: E501
-        :type issuer_url: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and issuer_url is None:  # noqa: E501
+        if issuer_url is None:
             raise ValueError("Invalid value for `issuer_url`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                issuer_url is not None and len(issuer_url) < 1):
-            raise ValueError("Invalid value for `issuer_url`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._issuer_url = issuer_url
 
     @property
-    def fallback_issuer_urls(self):
-        """Gets the fallback_issuer_urls of this AuthenticationInformation.  # noqa: E501
-
-
-        :return: The fallback_issuer_urls of this AuthenticationInformation.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._fallback_issuer_urls
-
-    @fallback_issuer_urls.setter
-    def fallback_issuer_urls(self, fallback_issuer_urls):
-        """Sets the fallback_issuer_urls of this AuthenticationInformation.
-
-
-        :param fallback_issuer_urls: The fallback_issuer_urls of this AuthenticationInformation.  # noqa: E501
-        :type fallback_issuer_urls: list[str]
-        """
-
-        self._fallback_issuer_urls = fallback_issuer_urls
-
-    @property
     def saml_identity_provider_id(self):
         """Gets the saml_identity_provider_id of this AuthenticationInformation.  # noqa: E501
 
 
         :return: The saml_identity_provider_id of this AuthenticationInformation.  # noqa: E501
         :rtype: str
         """
@@ -161,111 +115,82 @@
 
     @saml_identity_provider_id.setter
     def saml_identity_provider_id(self, saml_identity_provider_id):
         """Sets the saml_identity_provider_id of this AuthenticationInformation.
 
 
         :param saml_identity_provider_id: The saml_identity_provider_id of this AuthenticationInformation.  # noqa: E501
-        :type saml_identity_provider_id: str
+        :type: str
         """
 
         self._saml_identity_provider_id = saml_identity_provider_id
 
     @property
     def support(self):
         """Gets the support of this AuthenticationInformation.  # noqa: E501
 
 
         :return: The support of this AuthenticationInformation.  # noqa: E501
-        :rtype: finbourne_identity.SupportAccessExpiry
+        :rtype: SupportAccessExpiry
         """
         return self._support
 
     @support.setter
     def support(self, support):
         """Sets the support of this AuthenticationInformation.
 
 
         :param support: The support of this AuthenticationInformation.  # noqa: E501
-        :type support: finbourne_identity.SupportAccessExpiry
+        :type: SupportAccessExpiry
         """
 
         self._support = support
 
     @property
-    def support_access_expiry_with_role(self):
-        """Gets the support_access_expiry_with_role of this AuthenticationInformation.  # noqa: E501
-
-
-        :return: The support_access_expiry_with_role of this AuthenticationInformation.  # noqa: E501
-        :rtype: list[finbourne_identity.SupportAccessExpiryWithRole]
-        """
-        return self._support_access_expiry_with_role
-
-    @support_access_expiry_with_role.setter
-    def support_access_expiry_with_role(self, support_access_expiry_with_role):
-        """Sets the support_access_expiry_with_role of this AuthenticationInformation.
-
-
-        :param support_access_expiry_with_role: The support_access_expiry_with_role of this AuthenticationInformation.  # noqa: E501
-        :type support_access_expiry_with_role: list[finbourne_identity.SupportAccessExpiryWithRole]
-        """
-
-        self._support_access_expiry_with_role = support_access_expiry_with_role
-
-    @property
     def links(self):
         """Gets the links of this AuthenticationInformation.  # noqa: E501
 
 
         :return: The links of this AuthenticationInformation.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :rtype: list[Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
         """Sets the links of this AuthenticationInformation.
 
 
         :param links: The links of this AuthenticationInformation.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :type: list[Link]
         """
 
         self._links = links
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -274,15 +199,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, AuthenticationInformation):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AuthenticationInformation):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_api_key.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_api_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class CreateApiKey(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -49,26 +43,24 @@
     }
 
     required_map = {
         'display_name': 'required',
         'deactivation_date': 'optional'
     }
 
-    def __init__(self, display_name=None, deactivation_date=None, local_vars_configuration=None):  # noqa: E501
-        """CreateApiKey - a model defined in OpenAPI"
-        
+    def __init__(self, display_name=None, deactivation_date=None):  # noqa: E501
+        """
+        CreateApiKey - a model defined in OpenAPI
+
         :param display_name:  The display name for the API key (required)
         :type display_name: str
         :param deactivation_date:  The optional date at which the key should deactivate
         :type deactivation_date: datetime
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._display_name = None
         self._deactivation_date = None
         self.discriminator = None
 
         self.display_name = display_name
         self.deactivation_date = deactivation_date
@@ -87,27 +79,22 @@
     @display_name.setter
     def display_name(self, display_name):
         """Sets the display_name of this CreateApiKey.
 
         The display name for the API key  # noqa: E501
 
         :param display_name: The display_name of this CreateApiKey.  # noqa: E501
-        :type display_name: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+        if display_name is None:
             raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) > 512):
-            raise ValueError("Invalid value for `display_name`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+        if display_name is not None and len(display_name) > 50:
+            raise ValueError("Invalid value for `display_name`, length must be less than or equal to `50`")  # noqa: E501
+        if display_name is not None and len(display_name) < 0:
+            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
     def deactivation_date(self):
         """Gets the deactivation_date of this CreateApiKey.  # noqa: E501
 
@@ -121,48 +108,40 @@
     @deactivation_date.setter
     def deactivation_date(self, deactivation_date):
         """Sets the deactivation_date of this CreateApiKey.
 
         The optional date at which the key should deactivate  # noqa: E501
 
         :param deactivation_date: The deactivation_date of this CreateApiKey.  # noqa: E501
-        :type deactivation_date: datetime
+        :type: datetime
         """
 
         self._deactivation_date = deactivation_date
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -171,15 +150,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, CreateApiKey):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateApiKey):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_role_request.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/role_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class CreateRoleRequest(object):
+class RoleResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,160 +29,193 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'id': 'str',
+        'role_id': 'RoleId',
         'name': 'str',
         'description': 'str'
     }
 
     attribute_map = {
+        'id': 'id',
+        'role_id': 'roleId',
         'name': 'name',
         'description': 'description'
     }
 
     required_map = {
+        'id': 'required',
+        'role_id': 'required',
         'name': 'required',
-        'description': 'optional'
+        'description': 'required'
     }
 
-    def __init__(self, name=None, description=None, local_vars_configuration=None):  # noqa: E501
-        """CreateRoleRequest - a model defined in OpenAPI"
-        
+    def __init__(self, id=None, role_id=None, name=None, description=None):  # noqa: E501
+        """
+        RoleResponse - a model defined in OpenAPI
+
+        :param id:  The role's system supplied unique identifier (required)
+        :type id: str
+        :param role_id:  (required)
+        :type role_id: finbourne_identity.RoleId
         :param name:  The role name, which must be unique within the system. (required)
         :type name: str
-        :param description:  The description for this role
+        :param description:  The description for this role (required)
         :type description: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
+        self._id = None
+        self._role_id = None
         self._name = None
         self._description = None
         self.discriminator = None
 
+        self.id = id
+        self.role_id = role_id
         self.name = name
         self.description = description
 
     @property
+    def id(self):
+        """Gets the id of this RoleResponse.  # noqa: E501
+
+        The role's system supplied unique identifier  # noqa: E501
+
+        :return: The id of this RoleResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this RoleResponse.
+
+        The role's system supplied unique identifier  # noqa: E501
+
+        :param id: The id of this RoleResponse.  # noqa: E501
+        :type: str
+        """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
+
+        self._id = id
+
+    @property
+    def role_id(self):
+        """Gets the role_id of this RoleResponse.  # noqa: E501
+
+
+        :return: The role_id of this RoleResponse.  # noqa: E501
+        :rtype: RoleId
+        """
+        return self._role_id
+
+    @role_id.setter
+    def role_id(self, role_id):
+        """Sets the role_id of this RoleResponse.
+
+
+        :param role_id: The role_id of this RoleResponse.  # noqa: E501
+        :type: RoleId
+        """
+        if role_id is None:
+            raise ValueError("Invalid value for `role_id`, must not be `None`")  # noqa: E501
+
+        self._role_id = role_id
+
+    @property
     def name(self):
-        """Gets the name of this CreateRoleRequest.  # noqa: E501
+        """Gets the name of this RoleResponse.  # noqa: E501
 
         The role name, which must be unique within the system.  # noqa: E501
 
-        :return: The name of this CreateRoleRequest.  # noqa: E501
+        :return: The name of this RoleResponse.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateRoleRequest.
+        """Sets the name of this RoleResponse.
 
         The role name, which must be unique within the system.  # noqa: E501
 
-        :param name: The name of this CreateRoleRequest.  # noqa: E501
-        :type name: str
+        :param name: The name of this RoleResponse.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+        if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 512):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and not re.search(r'^[a-zA-Z][a-zA-Z0-9-_ +]{2,100}$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[a-zA-Z][a-zA-Z0-9-_ +]{2,100}$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def description(self):
-        """Gets the description of this CreateRoleRequest.  # noqa: E501
+        """Gets the description of this RoleResponse.  # noqa: E501
 
         The description for this role  # noqa: E501
 
-        :return: The description of this CreateRoleRequest.  # noqa: E501
+        :return: The description of this RoleResponse.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateRoleRequest.
+        """Sets the description of this RoleResponse.
 
         The description for this role  # noqa: E501
 
-        :param description: The description of this CreateRoleRequest.  # noqa: E501
-        :type description: str
+        :param description: The description of this RoleResponse.  # noqa: E501
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 1024):
-            raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 0):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
-            raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+        if description is None:
+            raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
 
         self._description = description
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateRoleRequest):
+        if not isinstance(other, RoleResponse):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateRoleRequest):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/create_user_request.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_user_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class CreateUserRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -38,76 +32,67 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'first_name': 'str',
         'last_name': 'str',
         'email_address': 'str',
-        'second_email_address': 'str',
         'login': 'str',
         'roles': 'list[RoleId]',
         'type': 'str'
     }
 
     attribute_map = {
         'first_name': 'firstName',
         'last_name': 'lastName',
         'email_address': 'emailAddress',
-        'second_email_address': 'secondEmailAddress',
         'login': 'login',
         'roles': 'roles',
         'type': 'type'
     }
 
     required_map = {
         'first_name': 'required',
         'last_name': 'required',
         'email_address': 'required',
-        'second_email_address': 'optional',
         'login': 'required',
         'roles': 'optional',
         'type': 'required'
     }
 
-    def __init__(self, first_name=None, last_name=None, email_address=None, second_email_address=None, login=None, roles=None, type=None, local_vars_configuration=None):  # noqa: E501
-        """CreateUserRequest - a model defined in OpenAPI"
-        
+    def __init__(self, first_name=None, last_name=None, email_address=None, login=None, roles=None, type=None):  # noqa: E501
+        """
+        CreateUserRequest - a model defined in OpenAPI
+
         :param first_name:  The first name of the user (required)
         :type first_name: str
         :param last_name:  The last name of the user (required)
         :type last_name: str
         :param email_address:  The user's email address - to which the account validation email will be sent. For user accounts  this should exactly match the Login. (required)
         :type email_address: str
-        :param second_email_address:  The user's second email address. Only allowed for Service users
-        :type second_email_address: str
         :param login:  The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address. (required)
         :type login: str
         :param roles:  Optional. Any known roles the user should be created with.
         :type roles: list[finbourne_identity.RoleId]
         :param type:  The type of user (e.g. Personal or Service) (required)
         :type type: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._first_name = None
         self._last_name = None
         self._email_address = None
-        self._second_email_address = None
         self._login = None
         self._roles = None
         self._type = None
         self.discriminator = None
 
         self.first_name = first_name
         self.last_name = last_name
         self.email_address = email_address
-        self.second_email_address = second_email_address
         self.login = login
         self.roles = roles
         self.type = type
 
     @property
     def first_name(self):
         """Gets the first_name of this CreateUserRequest.  # noqa: E501
@@ -122,27 +107,22 @@
     @first_name.setter
     def first_name(self, first_name):
         """Sets the first_name of this CreateUserRequest.
 
         The first name of the user  # noqa: E501
 
         :param first_name: The first_name of this CreateUserRequest.  # noqa: E501
-        :type first_name: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and first_name is None:  # noqa: E501
+        if first_name is None:
             raise ValueError("Invalid value for `first_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                first_name is not None and len(first_name) > 50):
+        if first_name is not None and len(first_name) > 50:
             raise ValueError("Invalid value for `first_name`, length must be less than or equal to `50`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                first_name is not None and len(first_name) < 1):
+        if first_name is not None and len(first_name) < 1:
             raise ValueError("Invalid value for `first_name`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                first_name is not None and not re.search(r'^[\s\S]*$', first_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `first_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._first_name = first_name
 
     @property
     def last_name(self):
         """Gets the last_name of this CreateUserRequest.  # noqa: E501
 
@@ -156,27 +136,22 @@
     @last_name.setter
     def last_name(self, last_name):
         """Sets the last_name of this CreateUserRequest.
 
         The last name of the user  # noqa: E501
 
         :param last_name: The last_name of this CreateUserRequest.  # noqa: E501
-        :type last_name: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and last_name is None:  # noqa: E501
+        if last_name is None:
             raise ValueError("Invalid value for `last_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                last_name is not None and len(last_name) > 50):
+        if last_name is not None and len(last_name) > 50:
             raise ValueError("Invalid value for `last_name`, length must be less than or equal to `50`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                last_name is not None and len(last_name) < 2):
+        if last_name is not None and len(last_name) < 2:
             raise ValueError("Invalid value for `last_name`, length must be greater than or equal to `2`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                last_name is not None and not re.search(r'^[\s\S]*$', last_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `last_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._last_name = last_name
 
     @property
     def email_address(self):
         """Gets the email_address of this CreateUserRequest.  # noqa: E501
 
@@ -190,57 +165,26 @@
     @email_address.setter
     def email_address(self, email_address):
         """Sets the email_address of this CreateUserRequest.
 
         The user's email address - to which the account validation email will be sent. For user accounts  this should exactly match the Login.  # noqa: E501
 
         :param email_address: The email_address of this CreateUserRequest.  # noqa: E501
-        :type email_address: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and email_address is None:  # noqa: E501
+        if email_address is None:
             raise ValueError("Invalid value for `email_address`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                email_address is not None and len(email_address) > 80):
+        if email_address is not None and len(email_address) > 80:
             raise ValueError("Invalid value for `email_address`, length must be less than or equal to `80`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                email_address is not None and len(email_address) < 5):
-            raise ValueError("Invalid value for `email_address`, length must be greater than or equal to `5`")  # noqa: E501
+        if email_address is not None and len(email_address) < 0:
+            raise ValueError("Invalid value for `email_address`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._email_address = email_address
 
     @property
-    def second_email_address(self):
-        """Gets the second_email_address of this CreateUserRequest.  # noqa: E501
-
-        The user's second email address. Only allowed for Service users  # noqa: E501
-
-        :return: The second_email_address of this CreateUserRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._second_email_address
-
-    @second_email_address.setter
-    def second_email_address(self, second_email_address):
-        """Sets the second_email_address of this CreateUserRequest.
-
-        The user's second email address. Only allowed for Service users  # noqa: E501
-
-        :param second_email_address: The second_email_address of this CreateUserRequest.  # noqa: E501
-        :type second_email_address: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                second_email_address is not None and len(second_email_address) > 80):
-            raise ValueError("Invalid value for `second_email_address`, length must be less than or equal to `80`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                second_email_address is not None and len(second_email_address) < 5):
-            raise ValueError("Invalid value for `second_email_address`, length must be greater than or equal to `5`")  # noqa: E501
-
-        self._second_email_address = second_email_address
-
-    @property
     def login(self):
         """Gets the login of this CreateUserRequest.  # noqa: E501
 
         The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address.  # noqa: E501
 
         :return: The login of this CreateUserRequest.  # noqa: E501
         :rtype: str
@@ -250,46 +194,44 @@
     @login.setter
     def login(self, login):
         """Sets the login of this CreateUserRequest.
 
         The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address.  # noqa: E501
 
         :param login: The login of this CreateUserRequest.  # noqa: E501
-        :type login: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and login is None:  # noqa: E501
+        if login is None:
             raise ValueError("Invalid value for `login`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                login is not None and len(login) > 80):
+        if login is not None and len(login) > 80:
             raise ValueError("Invalid value for `login`, length must be less than or equal to `80`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                login is not None and len(login) < 5):
-            raise ValueError("Invalid value for `login`, length must be greater than or equal to `5`")  # noqa: E501
+        if login is not None and len(login) < 0:
+            raise ValueError("Invalid value for `login`, length must be greater than or equal to `0`")  # noqa: E501
 
         self._login = login
 
     @property
     def roles(self):
         """Gets the roles of this CreateUserRequest.  # noqa: E501
 
         Optional. Any known roles the user should be created with.  # noqa: E501
 
         :return: The roles of this CreateUserRequest.  # noqa: E501
-        :rtype: list[finbourne_identity.RoleId]
+        :rtype: list[RoleId]
         """
         return self._roles
 
     @roles.setter
     def roles(self, roles):
         """Sets the roles of this CreateUserRequest.
 
         Optional. Any known roles the user should be created with.  # noqa: E501
 
         :param roles: The roles of this CreateUserRequest.  # noqa: E501
-        :type roles: list[finbourne_identity.RoleId]
+        :type: list[RoleId]
         """
 
         self._roles = roles
 
     @property
     def type(self):
         """Gets the type of this CreateUserRequest.  # noqa: E501
@@ -304,59 +246,42 @@
     @type.setter
     def type(self, type):
         """Sets the type of this CreateUserRequest.
 
         The type of user (e.g. Personal or Service)  # noqa: E501
 
         :param type: The type of this CreateUserRequest.  # noqa: E501
-        :type type: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+        if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) > 20):
-            raise ValueError("Invalid value for `type`, length must be less than or equal to `20`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and not re.search(r'^[a-zA-Z]*$', type)):  # noqa: E501
-            raise ValueError(r"Invalid value for `type`, must be a follow pattern or equal to `/^[a-zA-Z]*$/`")  # noqa: E501
 
         self._type = type
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -365,15 +290,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, CreateUserRequest):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateUserRequest):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/error_detail.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/role_id.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class ErrorDetail(object):
+class RoleId(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,170 +29,133 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'str',
-        'type': 'str',
-        'detail': 'str'
+        'scope': 'str',
+        'code': 'str'
     }
 
     attribute_map = {
-        'id': 'id',
-        'type': 'type',
-        'detail': 'detail'
+        'scope': 'scope',
+        'code': 'code'
     }
 
     required_map = {
-        'id': 'optional',
-        'type': 'optional',
-        'detail': 'optional'
+        'scope': 'optional',
+        'code': 'required'
     }
 
-    def __init__(self, id=None, type=None, detail=None, local_vars_configuration=None):  # noqa: E501
-        """ErrorDetail - a model defined in OpenAPI"
-        
-        :param id:  Id of the entity this error relates to
-        :type id: str
-        :param type:  Error type
-        :type type: str
-        :param detail:  Human readable description of the error
-        :type detail: str
-
-        """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._id = None
-        self._type = None
-        self._detail = None
-        self.discriminator = None
-
-        self.id = id
-        self.type = type
-        self.detail = detail
-
-    @property
-    def id(self):
-        """Gets the id of this ErrorDetail.  # noqa: E501
-
-        Id of the entity this error relates to  # noqa: E501
-
-        :return: The id of this ErrorDetail.  # noqa: E501
-        :rtype: str
+    def __init__(self, scope=None, code=None):  # noqa: E501
         """
-        return self._id
+        RoleId - a model defined in OpenAPI
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this ErrorDetail.
+        :param scope: 
+        :type scope: str
+        :param code:  (required)
+        :type code: str
 
-        Id of the entity this error relates to  # noqa: E501
+        """  # noqa: E501
 
-        :param id: The id of this ErrorDetail.  # noqa: E501
-        :type id: str
-        """
+        self._scope = None
+        self._code = None
+        self.discriminator = None
 
-        self._id = id
+        self.scope = scope
+        self.code = code
 
     @property
-    def type(self):
-        """Gets the type of this ErrorDetail.  # noqa: E501
+    def scope(self):
+        """Gets the scope of this RoleId.  # noqa: E501
 
-        Error type  # noqa: E501
 
-        :return: The type of this ErrorDetail.  # noqa: E501
+        :return: The scope of this RoleId.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._scope
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ErrorDetail.
+    @scope.setter
+    def scope(self, scope):
+        """Sets the scope of this RoleId.
 
-        Error type  # noqa: E501
 
-        :param type: The type of this ErrorDetail.  # noqa: E501
-        :type type: str
+        :param scope: The scope of this RoleId.  # noqa: E501
+        :type: str
         """
+        if scope is not None and len(scope) > 100:
+            raise ValueError("Invalid value for `scope`, length must be less than or equal to `100`")  # noqa: E501
+        if scope is not None and len(scope) < 3:
+            raise ValueError("Invalid value for `scope`, length must be greater than or equal to `3`")  # noqa: E501
 
-        self._type = type
+        self._scope = scope
 
     @property
-    def detail(self):
-        """Gets the detail of this ErrorDetail.  # noqa: E501
+    def code(self):
+        """Gets the code of this RoleId.  # noqa: E501
 
-        Human readable description of the error  # noqa: E501
 
-        :return: The detail of this ErrorDetail.  # noqa: E501
+        :return: The code of this RoleId.  # noqa: E501
         :rtype: str
         """
-        return self._detail
+        return self._code
 
-    @detail.setter
-    def detail(self, detail):
-        """Sets the detail of this ErrorDetail.
+    @code.setter
+    def code(self, code):
+        """Sets the code of this RoleId.
 
-        Human readable description of the error  # noqa: E501
 
-        :param detail: The detail of this ErrorDetail.  # noqa: E501
-        :type detail: str
+        :param code: The code of this RoleId.  # noqa: E501
+        :type: str
         """
+        if code is None:
+            raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
+        if code is not None and len(code) > 100:
+            raise ValueError("Invalid value for `code`, length must be less than or equal to `100`")  # noqa: E501
+        if code is not None and len(code) < 3:
+            raise ValueError("Invalid value for `code`, length must be greater than or equal to `3`")  # noqa: E501
 
-        self._detail = detail
+        self._code = code
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ErrorDetail):
+        if not isinstance(other, RoleId):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ErrorDetail):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/id_selector_definition.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/o_auth_application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class IdSelectorDefinition(object):
+class OAuthApplication(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,211 +29,245 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'identifier': 'dict(str, str)',
-        'actions': 'list[ActionId]',
-        'name': 'str',
-        'description': 'str'
+        'id': 'str',
+        'type': 'str',
+        'display_name': 'str',
+        'secret': 'str',
+        'client_id': 'str',
+        'issuer': 'str'
     }
 
     attribute_map = {
-        'identifier': 'identifier',
-        'actions': 'actions',
-        'name': 'name',
-        'description': 'description'
+        'id': 'id',
+        'type': 'type',
+        'display_name': 'displayName',
+        'secret': 'secret',
+        'client_id': 'clientId',
+        'issuer': 'issuer'
     }
 
     required_map = {
-        'identifier': 'required',
-        'actions': 'required',
-        'name': 'optional',
-        'description': 'optional'
+        'id': 'required',
+        'type': 'required',
+        'display_name': 'required',
+        'secret': 'optional',
+        'client_id': 'required',
+        'issuer': 'required'
     }
 
-    def __init__(self, identifier=None, actions=None, name=None, description=None, local_vars_configuration=None):  # noqa: E501
-        """IdSelectorDefinition - a model defined in OpenAPI"
-        
-        :param identifier:  (required)
-        :type identifier: dict(str, str)
-        :param actions:  (required)
-        :type actions: list[finbourne_identity.ActionId]
-        :param name: 
-        :type name: str
-        :param description: 
-        :type description: str
+    def __init__(self, id=None, type=None, display_name=None, secret=None, client_id=None, issuer=None):  # noqa: E501
+        """
+        OAuthApplication - a model defined in OpenAPI
+
+        :param id:  (required)
+        :type id: str
+        :param type:  (required)
+        :type type: str
+        :param display_name:  (required)
+        :type display_name: str
+        :param secret: 
+        :type secret: str
+        :param client_id:  (required)
+        :type client_id: str
+        :param issuer:  (required)
+        :type issuer: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._identifier = None
-        self._actions = None
-        self._name = None
-        self._description = None
+
+        self._id = None
+        self._type = None
+        self._display_name = None
+        self._secret = None
+        self._client_id = None
+        self._issuer = None
         self.discriminator = None
 
-        self.identifier = identifier
-        self.actions = actions
-        self.name = name
-        self.description = description
+        self.id = id
+        self.type = type
+        self.display_name = display_name
+        self.secret = secret
+        self.client_id = client_id
+        self.issuer = issuer
 
     @property
-    def identifier(self):
-        """Gets the identifier of this IdSelectorDefinition.  # noqa: E501
+    def id(self):
+        """Gets the id of this OAuthApplication.  # noqa: E501
 
 
-        :return: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :rtype: dict(str, str)
+        :return: The id of this OAuthApplication.  # noqa: E501
+        :rtype: str
         """
-        return self._identifier
+        return self._id
 
-    @identifier.setter
-    def identifier(self, identifier):
-        """Sets the identifier of this IdSelectorDefinition.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this OAuthApplication.
 
 
-        :param identifier: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :type identifier: dict(str, str)
+        :param id: The id of this OAuthApplication.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and identifier is None:  # noqa: E501
-            raise ValueError("Invalid value for `identifier`, must not be `None`")  # noqa: E501
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._identifier = identifier
+        self._id = id
 
     @property
-    def actions(self):
-        """Gets the actions of this IdSelectorDefinition.  # noqa: E501
+    def type(self):
+        """Gets the type of this OAuthApplication.  # noqa: E501
 
 
-        :return: The actions of this IdSelectorDefinition.  # noqa: E501
-        :rtype: list[finbourne_identity.ActionId]
+        :return: The type of this OAuthApplication.  # noqa: E501
+        :rtype: str
         """
-        return self._actions
+        return self._type
 
-    @actions.setter
-    def actions(self, actions):
-        """Sets the actions of this IdSelectorDefinition.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this OAuthApplication.
 
 
-        :param actions: The actions of this IdSelectorDefinition.  # noqa: E501
-        :type actions: list[finbourne_identity.ActionId]
+        :param type: The type of this OAuthApplication.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and actions is None:  # noqa: E501
-            raise ValueError("Invalid value for `actions`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                actions is not None and len(actions) < 1):
-            raise ValueError("Invalid value for `actions`, number of items must be greater than or equal to `1`")  # noqa: E501
+        if type is None:
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._actions = actions
+        self._type = type
 
     @property
-    def name(self):
-        """Gets the name of this IdSelectorDefinition.  # noqa: E501
+    def display_name(self):
+        """Gets the display_name of this OAuthApplication.  # noqa: E501
 
 
-        :return: The name of this IdSelectorDefinition.  # noqa: E501
+        :return: The display_name of this OAuthApplication.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._display_name
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this IdSelectorDefinition.
+    @display_name.setter
+    def display_name(self, display_name):
+        """Sets the display_name of this OAuthApplication.
 
 
-        :param name: The name of this IdSelectorDefinition.  # noqa: E501
-        :type name: str
+        :param display_name: The display_name of this OAuthApplication.  # noqa: E501
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) > 100):
-            raise ValueError("Invalid value for `name`, length must be less than or equal to `100`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 0):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `0`")  # noqa: E501
+        if display_name is None:
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._display_name = display_name
 
     @property
-    def description(self):
-        """Gets the description of this IdSelectorDefinition.  # noqa: E501
+    def secret(self):
+        """Gets the secret of this OAuthApplication.  # noqa: E501
 
 
-        :return: The description of this IdSelectorDefinition.  # noqa: E501
+        :return: The secret of this OAuthApplication.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._secret
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this IdSelectorDefinition.
+    @secret.setter
+    def secret(self, secret):
+        """Sets the secret of this OAuthApplication.
 
 
-        :param description: The description of this IdSelectorDefinition.  # noqa: E501
-        :type description: str
+        :param secret: The secret of this OAuthApplication.  # noqa: E501
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 1024):
-            raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 0):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `0`")  # noqa: E501
 
-        self._description = description
+        self._secret = secret
 
-    def to_dict(self, serialize=False):
+    @property
+    def client_id(self):
+        """Gets the client_id of this OAuthApplication.  # noqa: E501
+
+
+        :return: The client_id of this OAuthApplication.  # noqa: E501
+        :rtype: str
+        """
+        return self._client_id
+
+    @client_id.setter
+    def client_id(self, client_id):
+        """Sets the client_id of this OAuthApplication.
+
+
+        :param client_id: The client_id of this OAuthApplication.  # noqa: E501
+        :type: str
+        """
+        if client_id is None:
+            raise ValueError("Invalid value for `client_id`, must not be `None`")  # noqa: E501
+
+        self._client_id = client_id
+
+    @property
+    def issuer(self):
+        """Gets the issuer of this OAuthApplication.  # noqa: E501
+
+
+        :return: The issuer of this OAuthApplication.  # noqa: E501
+        :rtype: str
+        """
+        return self._issuer
+
+    @issuer.setter
+    def issuer(self, issuer):
+        """Sets the issuer of this OAuthApplication.
+
+
+        :param issuer: The issuer of this OAuthApplication.  # noqa: E501
+        :type: str
+        """
+        if issuer is None:
+            raise ValueError("Invalid value for `issuer`, must not be `None`")  # noqa: E501
+
+        self._issuer = issuer
+
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IdSelectorDefinition):
+        if not isinstance(other, OAuthApplication):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, IdSelectorDefinition):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/identifier_part_schema.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/domain_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class IdentifierPartSchema(object):
+class DomainResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,267 +29,302 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'index': 'int',
-        'name': 'str',
-        'display_name': 'str',
+        'id': 'DomainId',
         'description': 'str',
-        'required': 'bool',
+        'company_name': 'str',
+        'owner': 'UserId',
+        'billing_contact': 'UserId',
+        'technical_contact': 'UserId',
+        'created': 'datetime',
         'links': 'list[Link]'
     }
 
     attribute_map = {
-        'index': 'index',
-        'name': 'name',
-        'display_name': 'displayName',
+        'id': 'id',
         'description': 'description',
-        'required': 'required',
+        'company_name': 'companyName',
+        'owner': 'owner',
+        'billing_contact': 'billingContact',
+        'technical_contact': 'technicalContact',
+        'created': 'created',
         'links': 'links'
     }
 
     required_map = {
-        'index': 'required',
-        'name': 'required',
-        'display_name': 'required',
-        'description': 'required',
-        'required': 'required',
+        'id': 'optional',
+        'description': 'optional',
+        'company_name': 'optional',
+        'owner': 'optional',
+        'billing_contact': 'optional',
+        'technical_contact': 'optional',
+        'created': 'optional',
         'links': 'optional'
     }
 
-    def __init__(self, index=None, name=None, display_name=None, description=None, required=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """IdentifierPartSchema - a model defined in OpenAPI"
-        
-        :param index:  (required)
-        :type index: int
-        :param name:  (required)
-        :type name: str
-        :param display_name:  (required)
-        :type display_name: str
-        :param description:  (required)
+    def __init__(self, id=None, description=None, company_name=None, owner=None, billing_contact=None, technical_contact=None, created=None, links=None):  # noqa: E501
+        """
+        DomainResponse - a model defined in OpenAPI
+
+        :param id: 
+        :type id: finbourne_identity.DomainId
+        :param description:  A description of the domain
         :type description: str
-        :param required:  (required)
-        :type required: bool
+        :param company_name:  The company name for the domain
+        :type company_name: str
+        :param owner: 
+        :type owner: finbourne_identity.UserId
+        :param billing_contact: 
+        :type billing_contact: finbourne_identity.UserId
+        :param technical_contact: 
+        :type technical_contact: finbourne_identity.UserId
+        :param created:  The
+        :type created: datetime
         :param links: 
         :type links: list[finbourne_identity.Link]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._index = None
-        self._name = None
-        self._display_name = None
+
+        self._id = None
         self._description = None
-        self._required = None
+        self._company_name = None
+        self._owner = None
+        self._billing_contact = None
+        self._technical_contact = None
+        self._created = None
         self._links = None
         self.discriminator = None
 
-        self.index = index
-        self.name = name
-        self.display_name = display_name
+        if id is not None:
+            self.id = id
         self.description = description
-        self.required = required
+        self.company_name = company_name
+        if owner is not None:
+            self.owner = owner
+        if billing_contact is not None:
+            self.billing_contact = billing_contact
+        if technical_contact is not None:
+            self.technical_contact = technical_contact
+        if created is not None:
+            self.created = created
         self.links = links
 
     @property
-    def index(self):
-        """Gets the index of this IdentifierPartSchema.  # noqa: E501
+    def id(self):
+        """Gets the id of this DomainResponse.  # noqa: E501
 
 
-        :return: The index of this IdentifierPartSchema.  # noqa: E501
-        :rtype: int
+        :return: The id of this DomainResponse.  # noqa: E501
+        :rtype: DomainId
         """
-        return self._index
+        return self._id
 
-    @index.setter
-    def index(self, index):
-        """Sets the index of this IdentifierPartSchema.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this DomainResponse.
 
 
-        :param index: The index of this IdentifierPartSchema.  # noqa: E501
-        :type index: int
+        :param id: The id of this DomainResponse.  # noqa: E501
+        :type: DomainId
         """
-        if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
-            raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
 
-        self._index = index
+        self._id = id
 
     @property
-    def name(self):
-        """Gets the name of this IdentifierPartSchema.  # noqa: E501
+    def description(self):
+        """Gets the description of this DomainResponse.  # noqa: E501
 
+        A description of the domain  # noqa: E501
 
-        :return: The name of this IdentifierPartSchema.  # noqa: E501
+        :return: The description of this DomainResponse.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._description
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this IdentifierPartSchema.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this DomainResponse.
 
+        A description of the domain  # noqa: E501
 
-        :param name: The name of this IdentifierPartSchema.  # noqa: E501
-        :type name: str
+        :param description: The description of this DomainResponse.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._name = name
+        self._description = description
 
     @property
-    def display_name(self):
-        """Gets the display_name of this IdentifierPartSchema.  # noqa: E501
+    def company_name(self):
+        """Gets the company_name of this DomainResponse.  # noqa: E501
 
+        The company name for the domain  # noqa: E501
 
-        :return: The display_name of this IdentifierPartSchema.  # noqa: E501
+        :return: The company_name of this DomainResponse.  # noqa: E501
         :rtype: str
         """
-        return self._display_name
+        return self._company_name
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this IdentifierPartSchema.
+    @company_name.setter
+    def company_name(self, company_name):
+        """Sets the company_name of this DomainResponse.
 
+        The company name for the domain  # noqa: E501
 
-        :param display_name: The display_name of this IdentifierPartSchema.  # noqa: E501
-        :type display_name: str
+        :param company_name: The company_name of this DomainResponse.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._display_name = display_name
+        self._company_name = company_name
 
     @property
-    def description(self):
-        """Gets the description of this IdentifierPartSchema.  # noqa: E501
+    def owner(self):
+        """Gets the owner of this DomainResponse.  # noqa: E501
 
 
-        :return: The description of this IdentifierPartSchema.  # noqa: E501
-        :rtype: str
+        :return: The owner of this DomainResponse.  # noqa: E501
+        :rtype: UserId
         """
-        return self._description
+        return self._owner
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this IdentifierPartSchema.
+    @owner.setter
+    def owner(self, owner):
+        """Sets the owner of this DomainResponse.
 
 
-        :param description: The description of this IdentifierPartSchema.  # noqa: E501
-        :type description: str
+        :param owner: The owner of this DomainResponse.  # noqa: E501
+        :type: UserId
         """
-        if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
-            raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 1):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._description = description
+        self._owner = owner
+
+    @property
+    def billing_contact(self):
+        """Gets the billing_contact of this DomainResponse.  # noqa: E501
+
+
+        :return: The billing_contact of this DomainResponse.  # noqa: E501
+        :rtype: UserId
+        """
+        return self._billing_contact
+
+    @billing_contact.setter
+    def billing_contact(self, billing_contact):
+        """Sets the billing_contact of this DomainResponse.
+
+
+        :param billing_contact: The billing_contact of this DomainResponse.  # noqa: E501
+        :type: UserId
+        """
+
+        self._billing_contact = billing_contact
 
     @property
-    def required(self):
-        """Gets the required of this IdentifierPartSchema.  # noqa: E501
+    def technical_contact(self):
+        """Gets the technical_contact of this DomainResponse.  # noqa: E501
 
 
-        :return: The required of this IdentifierPartSchema.  # noqa: E501
-        :rtype: bool
+        :return: The technical_contact of this DomainResponse.  # noqa: E501
+        :rtype: UserId
         """
-        return self._required
+        return self._technical_contact
 
-    @required.setter
-    def required(self, required):
-        """Sets the required of this IdentifierPartSchema.
+    @technical_contact.setter
+    def technical_contact(self, technical_contact):
+        """Sets the technical_contact of this DomainResponse.
 
 
-        :param required: The required of this IdentifierPartSchema.  # noqa: E501
-        :type required: bool
+        :param technical_contact: The technical_contact of this DomainResponse.  # noqa: E501
+        :type: UserId
         """
-        if self.local_vars_configuration.client_side_validation and required is None:  # noqa: E501
-            raise ValueError("Invalid value for `required`, must not be `None`")  # noqa: E501
 
-        self._required = required
+        self._technical_contact = technical_contact
+
+    @property
+    def created(self):
+        """Gets the created of this DomainResponse.  # noqa: E501
+
+        The  # noqa: E501
+
+        :return: The created of this DomainResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._created
+
+    @created.setter
+    def created(self, created):
+        """Sets the created of this DomainResponse.
+
+        The  # noqa: E501
+
+        :param created: The created of this DomainResponse.  # noqa: E501
+        :type: datetime
+        """
+
+        self._created = created
 
     @property
     def links(self):
-        """Gets the links of this IdentifierPartSchema.  # noqa: E501
+        """Gets the links of this DomainResponse.  # noqa: E501
 
 
-        :return: The links of this IdentifierPartSchema.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :return: The links of this DomainResponse.  # noqa: E501
+        :rtype: list[Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
-        """Sets the links of this IdentifierPartSchema.
+        """Sets the links of this DomainResponse.
 
 
-        :param links: The links of this IdentifierPartSchema.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :param links: The links of this DomainResponse.  # noqa: E501
+        :type: list[Link]
         """
 
         self._links = links
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IdentifierPartSchema):
+        if not isinstance(other, DomainResponse):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, IdentifierPartSchema):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/link.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/role.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class Link(object):
+class Role(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,198 +29,184 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'relation': 'str',
-        'href': 'str',
-        'description': 'str',
-        'method': 'str'
+        'id': 'str',
+        'role_id': 'RoleId',
+        'name': 'str',
+        'description': 'str'
     }
 
     attribute_map = {
-        'relation': 'relation',
-        'href': 'href',
-        'description': 'description',
-        'method': 'method'
+        'id': 'id',
+        'role_id': 'roleId',
+        'name': 'name',
+        'description': 'description'
     }
 
     required_map = {
-        'relation': 'required',
-        'href': 'required',
-        'description': 'optional',
-        'method': 'required'
+        'id': 'required',
+        'role_id': 'optional',
+        'name': 'required',
+        'description': 'optional'
     }
 
-    def __init__(self, relation=None, href=None, description=None, method=None, local_vars_configuration=None):  # noqa: E501
-        """Link - a model defined in OpenAPI"
-        
-        :param relation:  (required)
-        :type relation: str
-        :param href:  (required)
-        :type href: str
+    def __init__(self, id=None, role_id=None, name=None, description=None):  # noqa: E501
+        """
+        Role - a model defined in OpenAPI
+
+        :param id:  (required)
+        :type id: str
+        :param role_id: 
+        :type role_id: finbourne_identity.RoleId
+        :param name:  (required)
+        :type name: str
         :param description: 
         :type description: str
-        :param method:  (required)
-        :type method: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
-        self._relation = None
-        self._href = None
+        self._id = None
+        self._role_id = None
+        self._name = None
         self._description = None
-        self._method = None
         self.discriminator = None
 
-        self.relation = relation
-        self.href = href
+        self.id = id
+        if role_id is not None:
+            self.role_id = role_id
+        self.name = name
         self.description = description
-        self.method = method
 
     @property
-    def relation(self):
-        """Gets the relation of this Link.  # noqa: E501
+    def id(self):
+        """Gets the id of this Role.  # noqa: E501
 
 
-        :return: The relation of this Link.  # noqa: E501
+        :return: The id of this Role.  # noqa: E501
         :rtype: str
         """
-        return self._relation
+        return self._id
 
-    @relation.setter
-    def relation(self, relation):
-        """Sets the relation of this Link.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Role.
 
 
-        :param relation: The relation of this Link.  # noqa: E501
-        :type relation: str
+        :param id: The id of this Role.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and relation is None:  # noqa: E501
-            raise ValueError("Invalid value for `relation`, must not be `None`")  # noqa: E501
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._relation = relation
+        self._id = id
 
     @property
-    def href(self):
-        """Gets the href of this Link.  # noqa: E501
+    def role_id(self):
+        """Gets the role_id of this Role.  # noqa: E501
 
 
-        :return: The href of this Link.  # noqa: E501
-        :rtype: str
+        :return: The role_id of this Role.  # noqa: E501
+        :rtype: RoleId
         """
-        return self._href
+        return self._role_id
 
-    @href.setter
-    def href(self, href):
-        """Sets the href of this Link.
+    @role_id.setter
+    def role_id(self, role_id):
+        """Sets the role_id of this Role.
 
 
-        :param href: The href of this Link.  # noqa: E501
-        :type href: str
+        :param role_id: The role_id of this Role.  # noqa: E501
+        :type: RoleId
         """
-        if self.local_vars_configuration.client_side_validation and href is None:  # noqa: E501
-            raise ValueError("Invalid value for `href`, must not be `None`")  # noqa: E501
 
-        self._href = href
+        self._role_id = role_id
 
     @property
-    def description(self):
-        """Gets the description of this Link.  # noqa: E501
+    def name(self):
+        """Gets the name of this Role.  # noqa: E501
 
 
-        :return: The description of this Link.  # noqa: E501
+        :return: The name of this Role.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._name
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this Link.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this Role.
 
 
-        :param description: The description of this Link.  # noqa: E501
-        :type description: str
+        :param name: The name of this Role.  # noqa: E501
+        :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._description = description
+        self._name = name
 
     @property
-    def method(self):
-        """Gets the method of this Link.  # noqa: E501
+    def description(self):
+        """Gets the description of this Role.  # noqa: E501
 
 
-        :return: The method of this Link.  # noqa: E501
+        :return: The description of this Role.  # noqa: E501
         :rtype: str
         """
-        return self._method
+        return self._description
 
-    @method.setter
-    def method(self, method):
-        """Sets the method of this Link.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Role.
 
 
-        :param method: The method of this Link.  # noqa: E501
-        :type method: str
+        :param description: The description of this Role.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and method is None:  # noqa: E501
-            raise ValueError("Invalid value for `method`, must not be `None`")  # noqa: E501
 
-        self._method = method
+        self._description = description
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Link):
+        if not isinstance(other, Role):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Link):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/list_users_response.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/api_key.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class ListUsersResponse(object):
+class ApiKey(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,198 +29,193 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'href': 'str',
-        'values': 'dict(str, UserSummary)',
-        'failed': 'dict(str, ErrorDetail)',
-        'links': 'list[Link]'
+        'id': 'str',
+        'display_name': 'str',
+        'created_date': 'datetime',
+        'deactivation_date': 'datetime'
     }
 
     attribute_map = {
-        'href': 'href',
-        'values': 'values',
-        'failed': 'failed',
-        'links': 'links'
+        'id': 'id',
+        'display_name': 'displayName',
+        'created_date': 'createdDate',
+        'deactivation_date': 'deactivationDate'
     }
 
     required_map = {
-        'href': 'optional',
-        'values': 'optional',
-        'failed': 'optional',
-        'links': 'optional'
+        'id': 'required',
+        'display_name': 'required',
+        'created_date': 'required',
+        'deactivation_date': 'optional'
     }
 
-    def __init__(self, href=None, values=None, failed=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """ListUsersResponse - a model defined in OpenAPI"
-        
-        :param href:  Uri of this response
-        :type href: str
-        :param values:  Successful entities, indexed by their id
-        :type values: dict[str, finbourne_identity.UserSummary]
-        :param failed:  Failed entities, indexed by their id
-        :type failed: dict[str, finbourne_identity.ErrorDetail]
-        :param links: 
-        :type links: list[finbourne_identity.Link]
+    def __init__(self, id=None, display_name=None, created_date=None, deactivation_date=None):  # noqa: E501
+        """
+        ApiKey - a model defined in OpenAPI
+
+        :param id:  The unique Id of the API key (required)
+        :type id: str
+        :param display_name:  The display name of the API key (required)
+        :type display_name: str
+        :param created_date:  The creation date of the API key (required)
+        :type created_date: datetime
+        :param deactivation_date:  The deactivation date of the API key
+        :type deactivation_date: datetime
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._href = None
-        self._values = None
-        self._failed = None
-        self._links = None
+
+        self._id = None
+        self._display_name = None
+        self._created_date = None
+        self._deactivation_date = None
         self.discriminator = None
 
-        self.href = href
-        self.values = values
-        self.failed = failed
-        self.links = links
+        self.id = id
+        self.display_name = display_name
+        self.created_date = created_date
+        self.deactivation_date = deactivation_date
 
     @property
-    def href(self):
-        """Gets the href of this ListUsersResponse.  # noqa: E501
+    def id(self):
+        """Gets the id of this ApiKey.  # noqa: E501
 
-        Uri of this response  # noqa: E501
+        The unique Id of the API key  # noqa: E501
 
-        :return: The href of this ListUsersResponse.  # noqa: E501
+        :return: The id of this ApiKey.  # noqa: E501
         :rtype: str
         """
-        return self._href
+        return self._id
 
-    @href.setter
-    def href(self, href):
-        """Sets the href of this ListUsersResponse.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this ApiKey.
 
-        Uri of this response  # noqa: E501
+        The unique Id of the API key  # noqa: E501
 
-        :param href: The href of this ListUsersResponse.  # noqa: E501
-        :type href: str
+        :param id: The id of this ApiKey.  # noqa: E501
+        :type: str
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
-        self._href = href
+        self._id = id
 
     @property
-    def values(self):
-        """Gets the values of this ListUsersResponse.  # noqa: E501
+    def display_name(self):
+        """Gets the display_name of this ApiKey.  # noqa: E501
 
-        Successful entities, indexed by their id  # noqa: E501
+        The display name of the API key  # noqa: E501
 
-        :return: The values of this ListUsersResponse.  # noqa: E501
-        :rtype: dict[str, finbourne_identity.UserSummary]
+        :return: The display_name of this ApiKey.  # noqa: E501
+        :rtype: str
         """
-        return self._values
+        return self._display_name
 
-    @values.setter
-    def values(self, values):
-        """Sets the values of this ListUsersResponse.
+    @display_name.setter
+    def display_name(self, display_name):
+        """Sets the display_name of this ApiKey.
 
-        Successful entities, indexed by their id  # noqa: E501
+        The display name of the API key  # noqa: E501
 
-        :param values: The values of this ListUsersResponse.  # noqa: E501
-        :type values: dict[str, finbourne_identity.UserSummary]
+        :param display_name: The display_name of this ApiKey.  # noqa: E501
+        :type: str
         """
+        if display_name is None:
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
 
-        self._values = values
+        self._display_name = display_name
 
     @property
-    def failed(self):
-        """Gets the failed of this ListUsersResponse.  # noqa: E501
+    def created_date(self):
+        """Gets the created_date of this ApiKey.  # noqa: E501
 
-        Failed entities, indexed by their id  # noqa: E501
+        The creation date of the API key  # noqa: E501
 
-        :return: The failed of this ListUsersResponse.  # noqa: E501
-        :rtype: dict[str, finbourne_identity.ErrorDetail]
+        :return: The created_date of this ApiKey.  # noqa: E501
+        :rtype: datetime
         """
-        return self._failed
+        return self._created_date
 
-    @failed.setter
-    def failed(self, failed):
-        """Sets the failed of this ListUsersResponse.
+    @created_date.setter
+    def created_date(self, created_date):
+        """Sets the created_date of this ApiKey.
 
-        Failed entities, indexed by their id  # noqa: E501
+        The creation date of the API key  # noqa: E501
 
-        :param failed: The failed of this ListUsersResponse.  # noqa: E501
-        :type failed: dict[str, finbourne_identity.ErrorDetail]
+        :param created_date: The created_date of this ApiKey.  # noqa: E501
+        :type: datetime
         """
+        if created_date is None:
+            raise ValueError("Invalid value for `created_date`, must not be `None`")  # noqa: E501
 
-        self._failed = failed
+        self._created_date = created_date
 
     @property
-    def links(self):
-        """Gets the links of this ListUsersResponse.  # noqa: E501
+    def deactivation_date(self):
+        """Gets the deactivation_date of this ApiKey.  # noqa: E501
 
+        The deactivation date of the API key  # noqa: E501
 
-        :return: The links of this ListUsersResponse.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :return: The deactivation_date of this ApiKey.  # noqa: E501
+        :rtype: datetime
         """
-        return self._links
+        return self._deactivation_date
 
-    @links.setter
-    def links(self, links):
-        """Sets the links of this ListUsersResponse.
+    @deactivation_date.setter
+    def deactivation_date(self, deactivation_date):
+        """Sets the deactivation_date of this ApiKey.
 
+        The deactivation date of the API key  # noqa: E501
 
-        :param links: The links of this ListUsersResponse.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :param deactivation_date: The deactivation_date of this ApiKey.  # noqa: E501
+        :type: datetime
         """
 
-        self._links = links
+        self._deactivation_date = deactivation_date
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ListUsersResponse):
+        if not isinstance(other, ApiKey):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ListUsersResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/lusid_problem_details.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/lusid_problem_details.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class LusidProblemDetails(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -42,42 +36,46 @@
         'name': 'str',
         'error_details': 'list[dict(str, str)]',
         'code': 'int',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
-        'instance': 'str'
+        'instance': 'str',
+        'extensions': 'dict(str, object)'
     }
 
     attribute_map = {
         'name': 'name',
         'error_details': 'errorDetails',
         'code': 'code',
         'type': 'type',
         'title': 'title',
         'status': 'status',
         'detail': 'detail',
-        'instance': 'instance'
+        'instance': 'instance',
+        'extensions': 'extensions'
     }
 
     required_map = {
         'name': 'required',
         'error_details': 'optional',
         'code': 'required',
         'type': 'optional',
         'title': 'optional',
         'status': 'optional',
         'detail': 'optional',
-        'instance': 'optional'
+        'instance': 'optional',
+        'extensions': 'optional'
     }
 
-    def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
-        """LusidProblemDetails - a model defined in OpenAPI"
-        
+    def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, extensions=None):  # noqa: E501
+        """
+        LusidProblemDetails - a model defined in OpenAPI
+
         :param name:  (required)
         :type name: str
         :param error_details: 
         :type error_details: list[dict(str, str)]
         :param code:  (required)
         :type code: int
         :param type: 
@@ -86,38 +84,39 @@
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
         :type detail: str
         :param instance: 
         :type instance: str
+        :param extensions: 
+        :type extensions: dict(str, object)
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._error_details = None
         self._code = None
         self._type = None
         self._title = None
         self._status = None
         self._detail = None
         self._instance = None
+        self._extensions = None
         self.discriminator = None
 
         self.name = name
         self.error_details = error_details
         self.code = code
         self.type = type
         self.title = title
         self.status = status
         self.detail = detail
         self.instance = instance
+        self.extensions = extensions
 
     @property
     def name(self):
         """Gets the name of this LusidProblemDetails.  # noqa: E501
 
 
         :return: The name of this LusidProblemDetails.  # noqa: E501
@@ -127,21 +126,18 @@
 
     @name.setter
     def name(self, name):
         """Sets the name of this LusidProblemDetails.
 
 
         :param name: The name of this LusidProblemDetails.  # noqa: E501
-        :type name: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+        if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._name = name
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidProblemDetails.  # noqa: E501
 
@@ -153,15 +149,15 @@
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidProblemDetails.
 
 
         :param error_details: The error_details of this LusidProblemDetails.  # noqa: E501
-        :type error_details: list[dict(str, str)]
+        :type: list[dict(str, str)]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidProblemDetails.  # noqa: E501
@@ -174,17 +170,17 @@
 
     @code.setter
     def code(self, code):
         """Sets the code of this LusidProblemDetails.
 
 
         :param code: The code of this LusidProblemDetails.  # noqa: E501
-        :type code: int
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
+        if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
         self._code = code
 
     @property
     def type(self):
         """Gets the type of this LusidProblemDetails.  # noqa: E501
@@ -197,15 +193,15 @@
 
     @type.setter
     def type(self, type):
         """Sets the type of this LusidProblemDetails.
 
 
         :param type: The type of this LusidProblemDetails.  # noqa: E501
-        :type type: str
+        :type: str
         """
 
         self._type = type
 
     @property
     def title(self):
         """Gets the title of this LusidProblemDetails.  # noqa: E501
@@ -218,15 +214,15 @@
 
     @title.setter
     def title(self, title):
         """Sets the title of this LusidProblemDetails.
 
 
         :param title: The title of this LusidProblemDetails.  # noqa: E501
-        :type title: str
+        :type: str
         """
 
         self._title = title
 
     @property
     def status(self):
         """Gets the status of this LusidProblemDetails.  # noqa: E501
@@ -239,15 +235,15 @@
 
     @status.setter
     def status(self, status):
         """Sets the status of this LusidProblemDetails.
 
 
         :param status: The status of this LusidProblemDetails.  # noqa: E501
-        :type status: int
+        :type: int
         """
 
         self._status = status
 
     @property
     def detail(self):
         """Gets the detail of this LusidProblemDetails.  # noqa: E501
@@ -260,15 +256,15 @@
 
     @detail.setter
     def detail(self, detail):
         """Sets the detail of this LusidProblemDetails.
 
 
         :param detail: The detail of this LusidProblemDetails.  # noqa: E501
-        :type detail: str
+        :type: str
         """
 
         self._detail = detail
 
     @property
     def instance(self):
         """Gets the instance of this LusidProblemDetails.  # noqa: E501
@@ -281,48 +277,61 @@
 
     @instance.setter
     def instance(self, instance):
         """Sets the instance of this LusidProblemDetails.
 
 
         :param instance: The instance of this LusidProblemDetails.  # noqa: E501
-        :type instance: str
+        :type: str
         """
 
         self._instance = instance
 
-    def to_dict(self, serialize=False):
+    @property
+    def extensions(self):
+        """Gets the extensions of this LusidProblemDetails.  # noqa: E501
+
+
+        :return: The extensions of this LusidProblemDetails.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._extensions
+
+    @extensions.setter
+    def extensions(self, extensions):
+        """Sets the extensions of this LusidProblemDetails.
+
+
+        :param extensions: The extensions of this LusidProblemDetails.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._extensions = extensions
+
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -331,15 +340,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, LusidProblemDetails):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LusidProblemDetails):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/lusid_validation_problem_details.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/lusid_validation_problem_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class LusidValidationProblemDetails(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -43,44 +37,48 @@
         'error_details': 'list[dict(str, str)]',
         'code': 'int',
         'errors': 'dict(str, list[str])',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
-        'instance': 'str'
+        'instance': 'str',
+        'extensions': 'dict(str, object)'
     }
 
     attribute_map = {
         'name': 'name',
         'error_details': 'errorDetails',
         'code': 'code',
         'errors': 'errors',
         'type': 'type',
         'title': 'title',
         'status': 'status',
         'detail': 'detail',
-        'instance': 'instance'
+        'instance': 'instance',
+        'extensions': 'extensions'
     }
 
     required_map = {
         'name': 'required',
         'error_details': 'optional',
         'code': 'required',
         'errors': 'optional',
         'type': 'optional',
         'title': 'optional',
         'status': 'optional',
         'detail': 'optional',
-        'instance': 'optional'
+        'instance': 'optional',
+        'extensions': 'optional'
     }
 
-    def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
-        """LusidValidationProblemDetails - a model defined in OpenAPI"
-        
+    def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, extensions=None):  # noqa: E501
+        """
+        LusidValidationProblemDetails - a model defined in OpenAPI
+
         :param name:  (required)
         :type name: str
         :param error_details: 
         :type error_details: list[dict(str, str)]
         :param code:  (required)
         :type code: int
         :param errors: 
@@ -91,40 +89,41 @@
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
         :type detail: str
         :param instance: 
         :type instance: str
+        :param extensions: 
+        :type extensions: dict(str, object)
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._error_details = None
         self._code = None
         self._errors = None
         self._type = None
         self._title = None
         self._status = None
         self._detail = None
         self._instance = None
+        self._extensions = None
         self.discriminator = None
 
         self.name = name
         self.error_details = error_details
         self.code = code
         self.errors = errors
         self.type = type
         self.title = title
         self.status = status
         self.detail = detail
         self.instance = instance
+        self.extensions = extensions
 
     @property
     def name(self):
         """Gets the name of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The name of this LusidValidationProblemDetails.  # noqa: E501
@@ -134,21 +133,18 @@
 
     @name.setter
     def name(self, name):
         """Sets the name of this LusidValidationProblemDetails.
 
 
         :param name: The name of this LusidValidationProblemDetails.  # noqa: E501
-        :type name: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+        if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._name = name
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidValidationProblemDetails.  # noqa: E501
 
@@ -160,15 +156,15 @@
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidValidationProblemDetails.
 
 
         :param error_details: The error_details of this LusidValidationProblemDetails.  # noqa: E501
-        :type error_details: list[dict(str, str)]
+        :type: list[dict(str, str)]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidValidationProblemDetails.  # noqa: E501
@@ -181,17 +177,17 @@
 
     @code.setter
     def code(self, code):
         """Sets the code of this LusidValidationProblemDetails.
 
 
         :param code: The code of this LusidValidationProblemDetails.  # noqa: E501
-        :type code: int
+        :type: int
         """
-        if self.local_vars_configuration.client_side_validation and code is None:  # noqa: E501
+        if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
         self._code = code
 
     @property
     def errors(self):
         """Gets the errors of this LusidValidationProblemDetails.  # noqa: E501
@@ -204,15 +200,15 @@
 
     @errors.setter
     def errors(self, errors):
         """Sets the errors of this LusidValidationProblemDetails.
 
 
         :param errors: The errors of this LusidValidationProblemDetails.  # noqa: E501
-        :type errors: dict(str, list[str])
+        :type: dict(str, list[str])
         """
 
         self._errors = errors
 
     @property
     def type(self):
         """Gets the type of this LusidValidationProblemDetails.  # noqa: E501
@@ -225,15 +221,15 @@
 
     @type.setter
     def type(self, type):
         """Sets the type of this LusidValidationProblemDetails.
 
 
         :param type: The type of this LusidValidationProblemDetails.  # noqa: E501
-        :type type: str
+        :type: str
         """
 
         self._type = type
 
     @property
     def title(self):
         """Gets the title of this LusidValidationProblemDetails.  # noqa: E501
@@ -246,15 +242,15 @@
 
     @title.setter
     def title(self, title):
         """Sets the title of this LusidValidationProblemDetails.
 
 
         :param title: The title of this LusidValidationProblemDetails.  # noqa: E501
-        :type title: str
+        :type: str
         """
 
         self._title = title
 
     @property
     def status(self):
         """Gets the status of this LusidValidationProblemDetails.  # noqa: E501
@@ -267,15 +263,15 @@
 
     @status.setter
     def status(self, status):
         """Sets the status of this LusidValidationProblemDetails.
 
 
         :param status: The status of this LusidValidationProblemDetails.  # noqa: E501
-        :type status: int
+        :type: int
         """
 
         self._status = status
 
     @property
     def detail(self):
         """Gets the detail of this LusidValidationProblemDetails.  # noqa: E501
@@ -288,15 +284,15 @@
 
     @detail.setter
     def detail(self, detail):
         """Sets the detail of this LusidValidationProblemDetails.
 
 
         :param detail: The detail of this LusidValidationProblemDetails.  # noqa: E501
-        :type detail: str
+        :type: str
         """
 
         self._detail = detail
 
     @property
     def instance(self):
         """Gets the instance of this LusidValidationProblemDetails.  # noqa: E501
@@ -309,48 +305,61 @@
 
     @instance.setter
     def instance(self, instance):
         """Sets the instance of this LusidValidationProblemDetails.
 
 
         :param instance: The instance of this LusidValidationProblemDetails.  # noqa: E501
-        :type instance: str
+        :type: str
         """
 
         self._instance = instance
 
-    def to_dict(self, serialize=False):
+    @property
+    def extensions(self):
+        """Gets the extensions of this LusidValidationProblemDetails.  # noqa: E501
+
+
+        :return: The extensions of this LusidValidationProblemDetails.  # noqa: E501
+        :rtype: dict(str, object)
+        """
+        return self._extensions
+
+    @extensions.setter
+    def extensions(self, extensions):
+        """Sets the extensions of this LusidValidationProblemDetails.
+
+
+        :param extensions: The extensions of this LusidValidationProblemDetails.  # noqa: E501
+        :type: dict(str, object)
+        """
+
+        self._extensions = extensions
+
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -359,15 +368,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, LusidValidationProblemDetails):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LusidValidationProblemDetails):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/role_response.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/update_user_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class RoleResponse(object):
+class UpdateUserRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,245 +29,229 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'str',
-        'role_id': 'RoleId',
-        'source': 'str',
-        'name': 'str',
-        'description': 'str'
+        'first_name': 'str',
+        'last_name': 'str',
+        'email_address': 'str',
+        'login': 'str',
+        'roles': 'list[RoleId]'
     }
 
     attribute_map = {
-        'id': 'id',
-        'role_id': 'roleId',
-        'source': 'source',
-        'name': 'name',
-        'description': 'description'
+        'first_name': 'firstName',
+        'last_name': 'lastName',
+        'email_address': 'emailAddress',
+        'login': 'login',
+        'roles': 'roles'
     }
 
     required_map = {
-        'id': 'required',
-        'role_id': 'required',
-        'source': 'required',
-        'name': 'required',
-        'description': 'optional'
+        'first_name': 'required',
+        'last_name': 'required',
+        'email_address': 'required',
+        'login': 'required',
+        'roles': 'optional'
     }
 
-    def __init__(self, id=None, role_id=None, source=None, name=None, description=None, local_vars_configuration=None):  # noqa: E501
-        """RoleResponse - a model defined in OpenAPI"
-        
-        :param id:  The role's system supplied unique identifier (required)
-        :type id: str
-        :param role_id:  (required)
-        :type role_id: finbourne_identity.RoleId
-        :param source:  The source of the role (required)
-        :type source: str
-        :param name:  The role name, which must be unique within the system. (required)
-        :type name: str
-        :param description:  The description for this role
-        :type description: str
+    def __init__(self, first_name=None, last_name=None, email_address=None, login=None, roles=None):  # noqa: E501
+        """
+        UpdateUserRequest - a model defined in OpenAPI
+
+        :param first_name:  (required)
+        :type first_name: str
+        :param last_name:  (required)
+        :type last_name: str
+        :param email_address:  (required)
+        :type email_address: str
+        :param login:  The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address. (required)
+        :type login: str
+        :param roles: 
+        :type roles: list[finbourne_identity.RoleId]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._id = None
-        self._role_id = None
-        self._source = None
-        self._name = None
-        self._description = None
+
+        self._first_name = None
+        self._last_name = None
+        self._email_address = None
+        self._login = None
+        self._roles = None
         self.discriminator = None
 
-        self.id = id
-        self.role_id = role_id
-        self.source = source
-        self.name = name
-        self.description = description
+        self.first_name = first_name
+        self.last_name = last_name
+        self.email_address = email_address
+        self.login = login
+        self.roles = roles
 
     @property
-    def id(self):
-        """Gets the id of this RoleResponse.  # noqa: E501
+    def first_name(self):
+        """Gets the first_name of this UpdateUserRequest.  # noqa: E501
 
-        The role's system supplied unique identifier  # noqa: E501
 
-        :return: The id of this RoleResponse.  # noqa: E501
+        :return: The first_name of this UpdateUserRequest.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._first_name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this RoleResponse.
+    @first_name.setter
+    def first_name(self, first_name):
+        """Sets the first_name of this UpdateUserRequest.
 
-        The role's system supplied unique identifier  # noqa: E501
 
-        :param id: The id of this RoleResponse.  # noqa: E501
-        :type id: str
+        :param first_name: The first_name of this UpdateUserRequest.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) < 1):
-            raise ValueError("Invalid value for `id`, length must be greater than or equal to `1`")  # noqa: E501
+        if first_name is None:
+            raise ValueError("Invalid value for `first_name`, must not be `None`")  # noqa: E501
+        if first_name is not None and len(first_name) > 50:
+            raise ValueError("Invalid value for `first_name`, length must be less than or equal to `50`")  # noqa: E501
+        if first_name is not None and len(first_name) < 1:
+            raise ValueError("Invalid value for `first_name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._id = id
+        self._first_name = first_name
 
     @property
-    def role_id(self):
-        """Gets the role_id of this RoleResponse.  # noqa: E501
+    def last_name(self):
+        """Gets the last_name of this UpdateUserRequest.  # noqa: E501
 
 
-        :return: The role_id of this RoleResponse.  # noqa: E501
-        :rtype: finbourne_identity.RoleId
+        :return: The last_name of this UpdateUserRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._role_id
+        return self._last_name
 
-    @role_id.setter
-    def role_id(self, role_id):
-        """Sets the role_id of this RoleResponse.
+    @last_name.setter
+    def last_name(self, last_name):
+        """Sets the last_name of this UpdateUserRequest.
 
 
-        :param role_id: The role_id of this RoleResponse.  # noqa: E501
-        :type role_id: finbourne_identity.RoleId
+        :param last_name: The last_name of this UpdateUserRequest.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and role_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `role_id`, must not be `None`")  # noqa: E501
+        if last_name is None:
+            raise ValueError("Invalid value for `last_name`, must not be `None`")  # noqa: E501
+        if last_name is not None and len(last_name) > 50:
+            raise ValueError("Invalid value for `last_name`, length must be less than or equal to `50`")  # noqa: E501
+        if last_name is not None and len(last_name) < 2:
+            raise ValueError("Invalid value for `last_name`, length must be greater than or equal to `2`")  # noqa: E501
 
-        self._role_id = role_id
+        self._last_name = last_name
 
     @property
-    def source(self):
-        """Gets the source of this RoleResponse.  # noqa: E501
+    def email_address(self):
+        """Gets the email_address of this UpdateUserRequest.  # noqa: E501
 
-        The source of the role  # noqa: E501
 
-        :return: The source of this RoleResponse.  # noqa: E501
+        :return: The email_address of this UpdateUserRequest.  # noqa: E501
         :rtype: str
         """
-        return self._source
+        return self._email_address
 
-    @source.setter
-    def source(self, source):
-        """Sets the source of this RoleResponse.
+    @email_address.setter
+    def email_address(self, email_address):
+        """Sets the email_address of this UpdateUserRequest.
 
-        The source of the role  # noqa: E501
 
-        :param source: The source of this RoleResponse.  # noqa: E501
-        :type source: str
+        :param email_address: The email_address of this UpdateUserRequest.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and source is None:  # noqa: E501
-            raise ValueError("Invalid value for `source`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                source is not None and len(source) < 1):
-            raise ValueError("Invalid value for `source`, length must be greater than or equal to `1`")  # noqa: E501
+        if email_address is None:
+            raise ValueError("Invalid value for `email_address`, must not be `None`")  # noqa: E501
+        if email_address is not None and len(email_address) > 80:
+            raise ValueError("Invalid value for `email_address`, length must be less than or equal to `80`")  # noqa: E501
+        if email_address is not None and len(email_address) < 0:
+            raise ValueError("Invalid value for `email_address`, length must be greater than or equal to `0`")  # noqa: E501
 
-        self._source = source
+        self._email_address = email_address
 
     @property
-    def name(self):
-        """Gets the name of this RoleResponse.  # noqa: E501
+    def login(self):
+        """Gets the login of this UpdateUserRequest.  # noqa: E501
 
-        The role name, which must be unique within the system.  # noqa: E501
+        The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address.  # noqa: E501
 
-        :return: The name of this RoleResponse.  # noqa: E501
+        :return: The login of this UpdateUserRequest.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._login
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RoleResponse.
+    @login.setter
+    def login(self, login):
+        """Sets the login of this UpdateUserRequest.
 
-        The role name, which must be unique within the system.  # noqa: E501
+        The user's login username, in the form of an email address, which must be unique within the system.  For user accounts this should exactly match the user's email address.  # noqa: E501
 
-        :param name: The name of this RoleResponse.  # noqa: E501
-        :type name: str
+        :param login: The login of this UpdateUserRequest.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
+        if login is None:
+            raise ValueError("Invalid value for `login`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._login = login
 
     @property
-    def description(self):
-        """Gets the description of this RoleResponse.  # noqa: E501
+    def roles(self):
+        """Gets the roles of this UpdateUserRequest.  # noqa: E501
 
-        The description for this role  # noqa: E501
 
-        :return: The description of this RoleResponse.  # noqa: E501
-        :rtype: str
+        :return: The roles of this UpdateUserRequest.  # noqa: E501
+        :rtype: list[RoleId]
         """
-        return self._description
+        return self._roles
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this RoleResponse.
+    @roles.setter
+    def roles(self, roles):
+        """Sets the roles of this UpdateUserRequest.
 
-        The description for this role  # noqa: E501
 
-        :param description: The description of this RoleResponse.  # noqa: E501
-        :type description: str
+        :param roles: The roles of this UpdateUserRequest.  # noqa: E501
+        :type: list[RoleId]
         """
 
-        self._description = description
+        self._roles = roles
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RoleResponse):
+        if not isinstance(other, UpdateUserRequest):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RoleResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/set_password.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/create_role_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class SetPassword(object):
+class CreateRoleRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,118 +29,129 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'value': 'str'
+        'name': 'str',
+        'description': 'str'
     }
 
     attribute_map = {
-        'value': 'value'
+        'name': 'name',
+        'description': 'description'
     }
 
     required_map = {
-        'value': 'required'
+        'name': 'required',
+        'description': 'optional'
     }
 
-    def __init__(self, value=None, local_vars_configuration=None):  # noqa: E501
-        """SetPassword - a model defined in OpenAPI"
-        
-        :param value:  The value of the new password (required)
-        :type value: str
+    def __init__(self, name=None, description=None):  # noqa: E501
+        """
+        CreateRoleRequest - a model defined in OpenAPI
+
+        :param name:  The role name, which must be unique within the system. (required)
+        :type name: str
+        :param description:  The description for this role
+        :type description: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
-        self._value = None
+        self._name = None
+        self._description = None
         self.discriminator = None
 
-        self.value = value
+        self.name = name
+        self.description = description
 
     @property
-    def value(self):
-        """Gets the value of this SetPassword.  # noqa: E501
+    def name(self):
+        """Gets the name of this CreateRoleRequest.  # noqa: E501
 
-        The value of the new password  # noqa: E501
+        The role name, which must be unique within the system.  # noqa: E501
 
-        :return: The value of this SetPassword.  # noqa: E501
+        :return: The name of this CreateRoleRequest.  # noqa: E501
         :rtype: str
         """
-        return self._value
+        return self._name
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this SetPassword.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this CreateRoleRequest.
 
-        The value of the new password  # noqa: E501
+        The role name, which must be unique within the system.  # noqa: E501
 
-        :param value: The value of this SetPassword.  # noqa: E501
-        :type value: str
+        :param name: The name of this CreateRoleRequest.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and value is None:  # noqa: E501
-            raise ValueError("Invalid value for `value`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                value is not None and len(value) > 50):
-            raise ValueError("Invalid value for `value`, length must be less than or equal to `50`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                value is not None and len(value) < 12):
-            raise ValueError("Invalid value for `value`, length must be greater than or equal to `12`")  # noqa: E501
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._value = value
+        self._name = name
 
-    def to_dict(self, serialize=False):
+    @property
+    def description(self):
+        """Gets the description of this CreateRoleRequest.  # noqa: E501
+
+        The description for this role  # noqa: E501
+
+        :return: The description of this CreateRoleRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this CreateRoleRequest.
+
+        The description for this role  # noqa: E501
+
+        :param description: The description of this CreateRoleRequest.  # noqa: E501
+        :type: str
+        """
+
+        self._description = description
+
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SetPassword):
+        if not isinstance(other, CreateRoleRequest):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SetPassword):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/set_password_response.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/agreement_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class SetPasswordResponse(object):
+class AgreementResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,140 +29,158 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'updated_at': 'datetime',
-        'links': 'list[Link]'
+        'name': 'str',
+        'signed_by': 'str',
+        'signed_at': 'datetime'
     }
 
     attribute_map = {
-        'updated_at': 'updatedAt',
-        'links': 'links'
+        'name': 'name',
+        'signed_by': 'signedBy',
+        'signed_at': 'signedAt'
     }
 
     required_map = {
-        'updated_at': 'required',
-        'links': 'optional'
+        'name': 'optional',
+        'signed_by': 'optional',
+        'signed_at': 'optional'
     }
 
-    def __init__(self, updated_at=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """SetPasswordResponse - a model defined in OpenAPI"
-        
-        :param updated_at:  The date and time at which the password was successfully updated (required)
-        :type updated_at: datetime
-        :param links: 
-        :type links: list[finbourne_identity.Link]
+    def __init__(self, name=None, signed_by=None, signed_at=None):  # noqa: E501
+        """
+        AgreementResponse - a model defined in OpenAPI
+
+        :param name:  Name of the agreement
+        :type name: str
+        :param signed_by:  UserID (obfuscated) of the user who signed this agreement
+        :type signed_by: str
+        :param signed_at:  Datetime at which the agreement was signed
+        :type signed_at: datetime
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
-        self._updated_at = None
-        self._links = None
+        self._name = None
+        self._signed_by = None
+        self._signed_at = None
         self.discriminator = None
 
-        self.updated_at = updated_at
-        self.links = links
+        self.name = name
+        self.signed_by = signed_by
+        if signed_at is not None:
+            self.signed_at = signed_at
 
     @property
-    def updated_at(self):
-        """Gets the updated_at of this SetPasswordResponse.  # noqa: E501
+    def name(self):
+        """Gets the name of this AgreementResponse.  # noqa: E501
 
-        The date and time at which the password was successfully updated  # noqa: E501
+        Name of the agreement  # noqa: E501
 
-        :return: The updated_at of this SetPasswordResponse.  # noqa: E501
-        :rtype: datetime
+        :return: The name of this AgreementResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        """Sets the name of this AgreementResponse.
+
+        Name of the agreement  # noqa: E501
+
+        :param name: The name of this AgreementResponse.  # noqa: E501
+        :type: str
         """
-        return self._updated_at
 
-    @updated_at.setter
-    def updated_at(self, updated_at):
-        """Sets the updated_at of this SetPasswordResponse.
+        self._name = name
 
-        The date and time at which the password was successfully updated  # noqa: E501
+    @property
+    def signed_by(self):
+        """Gets the signed_by of this AgreementResponse.  # noqa: E501
+
+        UserID (obfuscated) of the user who signed this agreement  # noqa: E501
+
+        :return: The signed_by of this AgreementResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._signed_by
+
+    @signed_by.setter
+    def signed_by(self, signed_by):
+        """Sets the signed_by of this AgreementResponse.
 
-        :param updated_at: The updated_at of this SetPasswordResponse.  # noqa: E501
-        :type updated_at: datetime
+        UserID (obfuscated) of the user who signed this agreement  # noqa: E501
+
+        :param signed_by: The signed_by of this AgreementResponse.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and updated_at is None:  # noqa: E501
-            raise ValueError("Invalid value for `updated_at`, must not be `None`")  # noqa: E501
 
-        self._updated_at = updated_at
+        self._signed_by = signed_by
 
     @property
-    def links(self):
-        """Gets the links of this SetPasswordResponse.  # noqa: E501
+    def signed_at(self):
+        """Gets the signed_at of this AgreementResponse.  # noqa: E501
 
+        Datetime at which the agreement was signed  # noqa: E501
 
-        :return: The links of this SetPasswordResponse.  # noqa: E501
-        :rtype: list[finbourne_identity.Link]
+        :return: The signed_at of this AgreementResponse.  # noqa: E501
+        :rtype: datetime
         """
-        return self._links
+        return self._signed_at
 
-    @links.setter
-    def links(self, links):
-        """Sets the links of this SetPasswordResponse.
+    @signed_at.setter
+    def signed_at(self, signed_at):
+        """Sets the signed_at of this AgreementResponse.
 
+        Datetime at which the agreement was signed  # noqa: E501
 
-        :param links: The links of this SetPasswordResponse.  # noqa: E501
-        :type links: list[finbourne_identity.Link]
+        :param signed_at: The signed_at of this AgreementResponse.  # noqa: E501
+        :type: datetime
         """
 
-        self._links = links
+        self._signed_at = signed_at
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SetPasswordResponse):
+        if not isinstance(other, AgreementResponse):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SetPasswordResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_expiry.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_expiry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class SupportAccessExpiry(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -46,24 +40,22 @@
         'expiry': 'expiry'
     }
 
     required_map = {
         'expiry': 'required'
     }
 
-    def __init__(self, expiry=None, local_vars_configuration=None):  # noqa: E501
-        """SupportAccessExpiry - a model defined in OpenAPI"
-        
+    def __init__(self, expiry=None):  # noqa: E501
+        """
+        SupportAccessExpiry - a model defined in OpenAPI
+
         :param expiry:  DateTimeOffset at which the access will be revoked (required)
         :type expiry: datetime
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._expiry = None
         self.discriminator = None
 
         self.expiry = expiry
 
     @property
@@ -80,50 +72,42 @@
     @expiry.setter
     def expiry(self, expiry):
         """Sets the expiry of this SupportAccessExpiry.
 
         DateTimeOffset at which the access will be revoked  # noqa: E501
 
         :param expiry: The expiry of this SupportAccessExpiry.  # noqa: E501
-        :type expiry: datetime
+        :type: datetime
         """
-        if self.local_vars_configuration.client_side_validation and expiry is None:  # noqa: E501
+        if expiry is None:
             raise ValueError("Invalid value for `expiry`, must not be `None`")  # noqa: E501
 
         self._expiry = expiry
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -132,15 +116,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, SupportAccessExpiry):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SupportAccessExpiry):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/support_access_response.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
 class SupportAccessResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -43,47 +37,45 @@
         'duration': 'str',
         'description': 'str',
         'created_at': 'datetime',
         'expiry': 'datetime',
         'created_by': 'str',
         'terminated': 'bool',
         'terminated_at': 'datetime',
-        'terminated_by': 'str',
-        'permitted_roles': 'list[str]'
+        'terminated_by': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'duration': 'duration',
         'description': 'description',
         'created_at': 'createdAt',
         'expiry': 'expiry',
         'created_by': 'createdBy',
         'terminated': 'terminated',
         'terminated_at': 'terminatedAt',
-        'terminated_by': 'terminatedBy',
-        'permitted_roles': 'permittedRoles'
+        'terminated_by': 'terminatedBy'
     }
 
     required_map = {
         'id': 'required',
         'duration': 'required',
         'description': 'optional',
         'created_at': 'required',
         'expiry': 'required',
         'created_by': 'required',
         'terminated': 'optional',
         'terminated_at': 'optional',
-        'terminated_by': 'optional',
-        'permitted_roles': 'optional'
+        'terminated_by': 'optional'
     }
 
-    def __init__(self, id=None, duration=None, description=None, created_at=None, expiry=None, created_by=None, terminated=None, terminated_at=None, terminated_by=None, permitted_roles=None, local_vars_configuration=None):  # noqa: E501
-        """SupportAccessResponse - a model defined in OpenAPI"
-        
+    def __init__(self, id=None, duration=None, description=None, created_at=None, expiry=None, created_by=None, terminated=None, terminated_at=None, terminated_by=None):  # noqa: E501
+        """
+        SupportAccessResponse - a model defined in OpenAPI
+
         :param id:  ID of the support access request (required)
         :type id: str
         :param duration:  The duration for which access is requested (in any ISO-8601 format) (required)
         :type duration: str
         :param description:  The description of why the support access has been granted (i.e. support ticket numbers)
         :type description: str
         :param created_at:  DateTimeOffset at which the access was granted (required)
@@ -94,45 +86,38 @@
         :type created_by: str
         :param terminated:  Whether or not that access has been invalidated
         :type terminated: bool
         :param terminated_at:  DateTimeOffset at which the access was invalidated
         :type terminated_at: datetime
         :param terminated_by:  Obfuscated UserId of the user who revoked the access
         :type terminated_by: str
-        :param permitted_roles:  A list of permitted roles, valid for support staff to assume, for the duration of the access request
-        :type permitted_roles: list[str]
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._duration = None
         self._description = None
         self._created_at = None
         self._expiry = None
         self._created_by = None
         self._terminated = None
         self._terminated_at = None
         self._terminated_by = None
-        self._permitted_roles = None
         self.discriminator = None
 
         self.id = id
         self.duration = duration
         self.description = description
         self.created_at = created_at
         self.expiry = expiry
         self.created_by = created_by
         if terminated is not None:
             self.terminated = terminated
         self.terminated_at = terminated_at
         self.terminated_by = terminated_by
-        self.permitted_roles = permitted_roles
 
     @property
     def id(self):
         """Gets the id of this SupportAccessResponse.  # noqa: E501
 
         ID of the support access request  # noqa: E501
 
@@ -144,21 +129,18 @@
     @id.setter
     def id(self, id):
         """Sets the id of this SupportAccessResponse.
 
         ID of the support access request  # noqa: E501
 
         :param id: The id of this SupportAccessResponse.  # noqa: E501
-        :type id: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
+        if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) < 1):
-            raise ValueError("Invalid value for `id`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._id = id
 
     @property
     def duration(self):
         """Gets the duration of this SupportAccessResponse.  # noqa: E501
 
@@ -172,23 +154,21 @@
     @duration.setter
     def duration(self, duration):
         """Sets the duration of this SupportAccessResponse.
 
         The duration for which access is requested (in any ISO-8601 format)  # noqa: E501
 
         :param duration: The duration of this SupportAccessResponse.  # noqa: E501
-        :type duration: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and duration is None:  # noqa: E501
+        if duration is None:
             raise ValueError("Invalid value for `duration`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                duration is not None and len(duration) > 50):
+        if duration is not None and len(duration) > 50:
             raise ValueError("Invalid value for `duration`, length must be less than or equal to `50`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                duration is not None and len(duration) < 3):
+        if duration is not None and len(duration) < 3:
             raise ValueError("Invalid value for `duration`, length must be greater than or equal to `3`")  # noqa: E501
 
         self._duration = duration
 
     @property
     def description(self):
         """Gets the description of this SupportAccessResponse.  # noqa: E501
@@ -203,25 +183,20 @@
     @description.setter
     def description(self, description):
         """Sets the description of this SupportAccessResponse.
 
         The description of why the support access has been granted (i.e. support ticket numbers)  # noqa: E501
 
         :param description: The description of this SupportAccessResponse.  # noqa: E501
-        :type description: str
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 1024):
+        if description is not None and len(description) > 1024:
             raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 0):
+        if description is not None and len(description) < 0:
             raise ValueError("Invalid value for `description`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
-            raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
     @property
     def created_at(self):
         """Gets the created_at of this SupportAccessResponse.  # noqa: E501
 
@@ -235,17 +210,17 @@
     @created_at.setter
     def created_at(self, created_at):
         """Sets the created_at of this SupportAccessResponse.
 
         DateTimeOffset at which the access was granted  # noqa: E501
 
         :param created_at: The created_at of this SupportAccessResponse.  # noqa: E501
-        :type created_at: datetime
+        :type: datetime
         """
-        if self.local_vars_configuration.client_side_validation and created_at is None:  # noqa: E501
+        if created_at is None:
             raise ValueError("Invalid value for `created_at`, must not be `None`")  # noqa: E501
 
         self._created_at = created_at
 
     @property
     def expiry(self):
         """Gets the expiry of this SupportAccessResponse.  # noqa: E501
@@ -260,17 +235,17 @@
     @expiry.setter
     def expiry(self, expiry):
         """Sets the expiry of this SupportAccessResponse.
 
         DateTimeOffset at which the access will be revoked  # noqa: E501
 
         :param expiry: The expiry of this SupportAccessResponse.  # noqa: E501
-        :type expiry: datetime
+        :type: datetime
         """
-        if self.local_vars_configuration.client_side_validation and expiry is None:  # noqa: E501
+        if expiry is None:
             raise ValueError("Invalid value for `expiry`, must not be `None`")  # noqa: E501
 
         self._expiry = expiry
 
     @property
     def created_by(self):
         """Gets the created_by of this SupportAccessResponse.  # noqa: E501
@@ -285,21 +260,18 @@
     @created_by.setter
     def created_by(self, created_by):
         """Sets the created_by of this SupportAccessResponse.
 
         Obfuscated UserId of the user who granted the support access  # noqa: E501
 
         :param created_by: The created_by of this SupportAccessResponse.  # noqa: E501
-        :type created_by: str
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and created_by is None:  # noqa: E501
+        if created_by is None:
             raise ValueError("Invalid value for `created_by`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                created_by is not None and len(created_by) < 1):
-            raise ValueError("Invalid value for `created_by`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._created_by = created_by
 
     @property
     def terminated(self):
         """Gets the terminated of this SupportAccessResponse.  # noqa: E501
 
@@ -313,15 +285,15 @@
     @terminated.setter
     def terminated(self, terminated):
         """Sets the terminated of this SupportAccessResponse.
 
         Whether or not that access has been invalidated  # noqa: E501
 
         :param terminated: The terminated of this SupportAccessResponse.  # noqa: E501
-        :type terminated: bool
+        :type: bool
         """
 
         self._terminated = terminated
 
     @property
     def terminated_at(self):
         """Gets the terminated_at of this SupportAccessResponse.  # noqa: E501
@@ -336,15 +308,15 @@
     @terminated_at.setter
     def terminated_at(self, terminated_at):
         """Sets the terminated_at of this SupportAccessResponse.
 
         DateTimeOffset at which the access was invalidated  # noqa: E501
 
         :param terminated_at: The terminated_at of this SupportAccessResponse.  # noqa: E501
-        :type terminated_at: datetime
+        :type: datetime
         """
 
         self._terminated_at = terminated_at
 
     @property
     def terminated_by(self):
         """Gets the terminated_by of this SupportAccessResponse.  # noqa: E501
@@ -359,71 +331,40 @@
     @terminated_by.setter
     def terminated_by(self, terminated_by):
         """Sets the terminated_by of this SupportAccessResponse.
 
         Obfuscated UserId of the user who revoked the access  # noqa: E501
 
         :param terminated_by: The terminated_by of this SupportAccessResponse.  # noqa: E501
-        :type terminated_by: str
+        :type: str
         """
 
         self._terminated_by = terminated_by
 
-    @property
-    def permitted_roles(self):
-        """Gets the permitted_roles of this SupportAccessResponse.  # noqa: E501
-
-        A list of permitted roles, valid for support staff to assume, for the duration of the access request  # noqa: E501
-
-        :return: The permitted_roles of this SupportAccessResponse.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._permitted_roles
-
-    @permitted_roles.setter
-    def permitted_roles(self, permitted_roles):
-        """Sets the permitted_roles of this SupportAccessResponse.
-
-        A list of permitted roles, valid for support staff to assume, for the duration of the access request  # noqa: E501
-
-        :param permitted_roles: The permitted_roles of this SupportAccessResponse.  # noqa: E501
-        :type permitted_roles: list[str]
-        """
-
-        self._permitted_roles = permitted_roles
-
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
@@ -432,15 +373,12 @@
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
         if not isinstance(other, SupportAccessResponse):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SupportAccessResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/models/update_role_request.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/models/support_access_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
-try:
-    from inspect import getfullargspec
-except ImportError:
-    from inspect import getargspec as getfullargspec
 import pprint
 import re  # noqa: F401
-import six
-
-from finbourne_identity.configuration import Configuration
 
+import six
 
-class UpdateRoleRequest(object):
+class SupportAccessRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,119 +29,137 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'duration': 'str',
         'description': 'str'
     }
 
     attribute_map = {
+        'duration': 'duration',
         'description': 'description'
     }
 
     required_map = {
+        'duration': 'required',
         'description': 'optional'
     }
 
-    def __init__(self, description=None, local_vars_configuration=None):  # noqa: E501
-        """UpdateRoleRequest - a model defined in OpenAPI"
-        
-        :param description:  The description for this role
+    def __init__(self, duration=None, description=None):  # noqa: E501
+        """
+        SupportAccessRequest - a model defined in OpenAPI
+
+        :param duration:  The duration for which access is requested (in any ISO-8601 format) (required)
+        :type duration: str
+        :param description:  The description of why the support access has been granted (i.e. support ticket numbers)
         :type description: str
 
         """  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration.get_default_copy()
-        self.local_vars_configuration = local_vars_configuration
 
+        self._duration = None
         self._description = None
         self.discriminator = None
 
+        self.duration = duration
         self.description = description
 
     @property
+    def duration(self):
+        """Gets the duration of this SupportAccessRequest.  # noqa: E501
+
+        The duration for which access is requested (in any ISO-8601 format)  # noqa: E501
+
+        :return: The duration of this SupportAccessRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._duration
+
+    @duration.setter
+    def duration(self, duration):
+        """Sets the duration of this SupportAccessRequest.
+
+        The duration for which access is requested (in any ISO-8601 format)  # noqa: E501
+
+        :param duration: The duration of this SupportAccessRequest.  # noqa: E501
+        :type: str
+        """
+        if duration is None:
+            raise ValueError("Invalid value for `duration`, must not be `None`")  # noqa: E501
+        if duration is not None and len(duration) > 50:
+            raise ValueError("Invalid value for `duration`, length must be less than or equal to `50`")  # noqa: E501
+        if duration is not None and len(duration) < 3:
+            raise ValueError("Invalid value for `duration`, length must be greater than or equal to `3`")  # noqa: E501
+
+        self._duration = duration
+
+    @property
     def description(self):
-        """Gets the description of this UpdateRoleRequest.  # noqa: E501
+        """Gets the description of this SupportAccessRequest.  # noqa: E501
 
-        The description for this role  # noqa: E501
+        The description of why the support access has been granted (i.e. support ticket numbers)  # noqa: E501
 
-        :return: The description of this UpdateRoleRequest.  # noqa: E501
+        :return: The description of this SupportAccessRequest.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this UpdateRoleRequest.
+        """Sets the description of this SupportAccessRequest.
 
-        The description for this role  # noqa: E501
+        The description of why the support access has been granted (i.e. support ticket numbers)  # noqa: E501
 
-        :param description: The description of this UpdateRoleRequest.  # noqa: E501
-        :type description: str
+        :param description: The description of this SupportAccessRequest.  # noqa: E501
+        :type: str
         """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 1024):
+        if description is not None and len(description) > 1024:
             raise ValueError("Invalid value for `description`, length must be less than or equal to `1024`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 0):
+        if description is not None and len(description) < 0:
             raise ValueError("Invalid value for `description`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
-            raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
-    def to_dict(self, serialize=False):
+    def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        def convert(x):
-            if hasattr(x, "to_dict"):
-                args = getfullargspec(x.to_dict).args
-                if len(args) == 1:
-                    return x.to_dict()
-                else:
-                    return x.to_dict(serialize)
-            else:
-                return x
-
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
-            attr = self.attribute_map.get(attr, attr) if serialize else attr
             if isinstance(value, list):
                 result[attr] = list(map(
-                    lambda x: convert(x),
+                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
+            elif hasattr(value, "to_dict"):
+                result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(map(
-                    lambda item: (item[0], convert(item[1])),
+                    lambda item: (item[0], item[1].to_dict())
+                    if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
-                result[attr] = convert(value)
+                result[attr] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UpdateRoleRequest):
+        if not isinstance(other, SupportAccessRequest):
             return False
 
-        return self.to_dict() == other.to_dict()
+        return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, UpdateRoleRequest):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        return not self == other
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/rest.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/rest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Identity Service API
 
-    FINBOURNE Technology  # noqa: E501
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.2469
+    The version of the OpenAPI document: 0.0.840
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -79,61 +79,36 @@
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
-        # tcp_keep_alive cannot be put in additional_pool_args without errors in the base pool manager
         if configuration.proxy:
-            if configuration.tcp_keep_alive:
-                self.pool_manager = TCPKeepAliveProxyManager(
-                    num_pools=pools_size,
-                    maxsize=maxsize,
-                    cert_reqs=cert_reqs,
-                    ca_certs=ca_certs,
-                    cert_file=configuration.cert_file,
-                    key_file=configuration.key_file,
-                    proxy_url=configuration.proxy,
-                    proxy_headers=configuration.proxy_headers,
-                    **addition_pool_args
-                )
-            else:
-                self.pool_manager = urllib3.ProxyManager(
-                    num_pools=pools_size,
-                    maxsize=maxsize,
-                    cert_reqs=cert_reqs,
-                    ca_certs=ca_certs,
-                    cert_file=configuration.cert_file,
-                    key_file=configuration.key_file,
-                    proxy_url=configuration.proxy,
-                    proxy_headers=configuration.proxy_headers,
-                    **addition_pool_args
-                )
+            self.pool_manager = TCPKeepAliveProxyManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=ca_certs,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                proxy_url=configuration.proxy,
+                proxy_headers=configuration.proxy_headers,
+                **addition_pool_args
+            )
         else:
-            if configuration.tcp_keep_alive:
-                self.pool_manager = TCPKeepAlivePoolManager(
-                    num_pools=pools_size,
-                    maxsize=maxsize,
-                    cert_reqs=cert_reqs,
-                    ca_certs=ca_certs,
-                    cert_file=configuration.cert_file,
-                    key_file=configuration.key_file,
-                    **addition_pool_args
-                )
-            else:
-                self.pool_manager = urllib3.PoolManager(
-                    num_pools=pools_size,
-                    maxsize=maxsize,
-                    cert_reqs=cert_reqs,
-                    ca_certs=ca_certs,
-                    cert_file=configuration.cert_file,
-                    key_file=configuration.key_file,
-                    **addition_pool_args
-                )
+            self.pool_manager = TCPKeepAlivePoolManager(
+                num_pools=pools_size,
+                maxsize=maxsize,
+                cert_reqs=cert_reqs,
+                ca_certs=ca_certs,
+                cert_file=configuration.cert_file,
+                key_file=configuration.key_file,
+                **addition_pool_args
+            )
 
     def request(self, method, url, query_params=None, headers=None,
                 body=None, post_params=None, _preload_content=True,
                 _request_timeout=None):
         """Perform requests.
 
         :param method: http request method
@@ -238,14 +213,18 @@
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
+            # In the python 3, the response.data is bytes.
+            # we need to decode it to string.
+            if six.PY3:
+                r.data = r.data.decode('utf8')
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/tcp/tcp_keep_alive_probes.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/tcp/tcp_keep_alive_probes.py`

 * *Files identical despite different names*

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_client_builder.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_client_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from urllib3 import make_headers
-import os
+from urllib.request import pathname2url
+import requests
 
 from finbourne_identity import Configuration, ApiClient
 
 from .api_configuration_loader import ApiConfigurationLoader
 from .refreshing_token import RefreshingToken
 
 
@@ -31,89 +32,112 @@
         # Raise an error if any fields have a value of None
         if len(missing_fields) > 0:
             raise ValueError(
                 f"The fields {str(missing_fields)} on the {object_to_check.__class__.__name__} are set to None, "
                 f"please ensure that you have provided them directly, via a secrets file or environment "
                 f"variables")
 
-    @classmethod
-    def __resolve_api_token(cls, token=None, configuration=None, id_provider_response_handler=None):
-
+    @staticmethod
+    def __generate_access_token(configuration, okta_response_handler):
         """
-        Description:
-        This method uses a PAT (Personal Access Token) or secrets to return an API token.
-        The method uses the following conditional logic in order of precedence to resolve an
-        authentication path:
+        This function generates an access token by making a call to Okta
 
-            1. Use PAT passed into the function
-            2. Use secrets files passed into the function
-            3. Use environment variables
-
-        PAT are used in preference to supplied credentials.
-        secrets files are used in preference to environment variables.
-
-        :param str token: The pre-populated access token to use instead of asking Okta for a token
-        :param ApiConfiguration configuration: configuration object containing secrets loaded from env vars
-        :param typing.callable id_provider_response_handler: An optional function to handle the Okta response
+        :param ApiConfiguration configuration: The configuration to use
+        :param typing.callable okta_response_handler: An optional function to handle the Okta response
 
-        :return: str api_token
+        :return: RefreshingToken api_token: A refreshing API token
         """
+        # Encode credentials that may contain special characters
+        encoded_password = pathname2url(configuration.password)
+        encoded_client_id = pathname2url(configuration.client_id)
+        encoded_client_secret = pathname2url(configuration.client_secret)
 
-        # If token is passed in by user, then use that token
-        if token is not None:
-            cls.__check_required_fields(configuration, ["api_url"])
-            api_token = token
+        # Prepare our authentication request
+        token_request_body = f"grant_type=password&username={configuration.username}" \
+            f"&password={encoded_password}&scope=openid client groups offline_access" \
+            f"&client_id={encoded_client_id}&client_secret={encoded_client_secret}"
 
-        # If there is a token provided use it
-        elif configuration.access_token is not None:
-            # Check that there is an api_url available
-            cls.__check_required_fields(configuration, ["api_url"])
-            api_token = configuration.access_token
+        headers = {"Accept": "application/json", "Content-Type": "application/x-www-form-urlencoded"}
 
-        # Otherwise generate an access token from Okta and use a RefreshingToken going forward
-        else:
-            # Check that all the required fields for generating a token exist
-            cls.__check_required_fields(configuration, [
-                "api_url",
-                "password",
-                "username",
-                "client_id",
-                "client_secret",
-                "token_url"])
+        # extra request args
+        kwargs = {"headers": headers}
 
-            # Generate an access token
-            api_token = RefreshingToken(
-                api_configuration=configuration,
-                id_provider_response_handler=id_provider_response_handler
-            )
+        if configuration.proxy_config is not None:
+            kwargs["proxies"] = configuration.proxy_config.format_proxy_schema()
+
+        # use certificate if supplied
+        if configuration.certificate_filename is not None:
+            kwargs["verify"] = configuration.certificate_filename
+
+        # make request to Okta to get an authentication token
+        okta_response = requests.post(configuration.token_url, data=token_request_body, **kwargs)
+
+        if okta_response_handler is not None:
+            okta_response_handler(okta_response)
+
+        # Ensure that we have a 200 response code
+        if okta_response.status_code != 200:
+            raise ValueError(okta_response.json())
+
+        # convert the json encoded response to be able to extract the token values
+        okta_json = okta_response.json()
+
+        # Retrieve our api token from the authentication response
+        api_token = RefreshingToken(token_url=configuration.token_url,
+                                    client_id=encoded_client_id,
+                                    client_secret=encoded_client_secret,
+                                    initial_access_token=okta_json["access_token"],
+                                    initial_token_expiry=okta_json["expires_in"],
+                                    refresh_token=okta_json["refresh_token"],
+                                    proxies=kwargs.get("proxies", None),
+                                    certificate_filename=kwargs.get("verify", None))
 
         return api_token
 
     @classmethod
-    def build(cls, api_secrets_filename=None, id_provider_response_handler=None, api_configuration=None, token=None, correlation_id=None, tcp_keep_alive=False):
+    def build(cls, api_secrets_filename=None, okta_response_handler=None, api_configuration=None, token=None):
         """
         :param str api_secrets_filename: The full path to the JSON file containing the API credentials and optional proxy details
-        :param typing.callable id_provider_response_handler: An optional function to handle the Okta response
+        :param typing.callable okta_response_handler: An optional function to handle the Okta response
         :param finbourne_identity.utilities.ApiConfiguration api_configuration: A pre-populated ApiConfiguration
         :param str token: The pre-populated access token to use instead of asking Okta for a token
-        :param str correlation_id: Correlation id for all calls made from the returned ApiClient instance, added as a header to each request
 
         :return: finbourne_identity.ApiClient: The configured LUSID ApiClient
         """
 
         # Load the configuration
         configuration = ApiConfigurationLoader.load(api_secrets_filename)
 
         # If an api_configuration has been provided override the loaded configuration with any properties that it has
         if api_configuration is not None:
             for key, value in vars(api_configuration).items():
                 if value is not None:
                     setattr(configuration, key, value)
 
-        api_token = cls.__resolve_api_token(token, configuration, id_provider_response_handler)
+        # Use the access token provided if it exists
+        if token is not None:
+            # Check that there is an api_url available
+            cls.__check_required_fields(configuration, ["api_url"])
+            api_token = token
+        # Otherwise generate an access token from Okta and use a RefreshingToken going forward
+        else:
+            # Check that all the required fields for generating a token exist
+            cls.__check_required_fields(configuration, [
+                "api_url",
+                "password",
+                "username",
+                "client_id",
+                "client_secret",
+                "token_url"])
+
+            # Generate an access token
+            api_token = cls.__generate_access_token(
+                configuration=configuration,
+                okta_response_handler=okta_response_handler
+            )
 
         # Initialise the API client using the token so that it can be included in all future requests
         config = Configuration()
         config.access_token = api_token
         config.host = configuration.api_url
 
         # Set the certificate from the configuration
@@ -124,19 +148,11 @@
             config.proxy = configuration.proxy_config.address
             if configuration.proxy_config.username is not None and configuration.proxy_config.password is not None:
                 config.proxy_headers = make_headers(
                     proxy_basic_auth=f"{configuration.proxy_config.username}:{configuration.proxy_config.password}"
                 )
 
         # Create and return the ApiClient
-        api_client = ApiClient(configuration=config)
-
-        # set the application name if specified
-        if configuration.app_name is not None:
-            api_client.set_default_header("X-LUSID-Application", configuration.app_name)
-
-        # set a correlation id for all requests initiated with this ApiClient
-        corr_id = correlation_id or os.getenv("FBN_CORRELATION_ID")
-        if corr_id is not None:
-            api_client.set_default_header("CorrelationId", corr_id)
-
-        return api_client
+        return ApiClient(
+            configuration=config,
+            header_name="X-LUSID-Application" if configuration.app_name is not None else None,
+            header_value=configuration.app_name)
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_client_factory.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_client_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,28 +18,25 @@
     def __init__(self, **kwargs):
         """
         Iniitalise an ApiClientFactory by passing the token, api_url and app_name, or by
         passing in the api_secrets_filename
 
         :param str token: Bearer token used to initialise the API
         :param str api_secrets_filename: Name of secrets file (including full path)
-        :param str api_url: Identity API url
+        :param str api_url: LUSID API url
         :param str app_name: Application name (optional)
         :param str certificate_filename: Name of the certificate file (.pem, .cer or .crt)
         :param str proxy_url: The url of the proxy to use including the port e.g. http://myproxy.com:8888
         :param str proxy_username: The username for the proxy to use
         :param str proxy_password: The password for the proxy to use
-        :param str correlation_id: Correlation id for all calls made from the returned Identity API instances
-        :param bool tcp_keep_alive: A flag for controlling if the API client uses TCP keep-alive probes
         """
 
         builder_kwargs = {}
 
         if "token" in kwargs and str(kwargs["token"]) != "None":
-
             # If there is a token use it along with the specified proxy details if specified
             config = ApiConfiguration(
                 api_url=kwargs.get("api_url", None),
                 certificate_filename=kwargs.get("certificate_filename", None),
                 proxy_config=ProxyConfig(
                     address=kwargs.get("proxy_url", None),
                     username=kwargs.get("proxy_username", None),
@@ -50,22 +47,14 @@
 
             builder_kwargs["api_configuration"] = config
             builder_kwargs["token"] = kwargs["token"]
 
         # Otherwise use a secrets file if it exists
         builder_kwargs["api_secrets_filename"] = kwargs.get("api_secrets_filename", None)
 
-        # add the correlation id if specified
-        builder_kwargs["correlation_id"] = kwargs.get("correlation_id", None)
-
-        # add the id provider response handler if specified
-        builder_kwargs["id_provider_response_handler"] = kwargs.get("id_provider_response_handler", None)
-
-        builder_kwargs["tcp_keep_alive"] = kwargs.get("tcp_keep_alive", False)
-
         # Call the client builder, this will result in using either a token, secrets file or environment variables
         self.api_client = ApiClientBuilder.build(**builder_kwargs)
 
     def build(self, metaclass):
         """
         :param type metaclass:  type of the LUSID API to create
         :return: Initalised LUSID API for the type passed in
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/api_configuration.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/api_configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class ApiConfiguration:
 
     def __init__(self, token_url=None, api_url=None, username=None, password=None, client_id=None, client_secret=None,
-                 app_name=None, certificate_filename=None, proxy_config=None, access_token=None):
+                 app_name=None, certificate_filename=None, proxy_config=None):
         """
         The configuration required to access LUSID, read more at https://support.finbourne.com/getting-started-with-apis-sdks
 
         :param str token_url: The token URL of the identity provider
         :param str api_url: The API URL for the LUSID client
         :param str username: The username to use
         :param str password: The password to use
@@ -20,15 +20,14 @@
         self.__username = username
         self.__password = password
         self.__client_id = client_id
         self.__client_secret = client_secret
         self.__app_name = app_name
         self.__certificate_filename = certificate_filename
         self.__proxy_config = proxy_config
-        self.__access_token = access_token
 
     @property
     def token_url(self):
         return self.__token_url
 
     @token_url.setter
     def token_url(self, value):
@@ -93,15 +92,7 @@
     @property
     def proxy_config(self):
         return self.__proxy_config
 
     @proxy_config.setter
     def proxy_config(self, value):
         self.__proxy_config = value
-
-    @property
-    def access_token(self):
-        return self.__access_token
-
-    @access_token.setter
-    def access_token(self, value):
-        self.__access_token = value
```

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/finbourne_identity_retry.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/finbourne_identity_retry.py`

 * *Files identical despite different names*

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity/utilities/proxy_config.py` & `finbourne-identity-sdk-0.0.840/finbourne_identity/utilities/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne-identity-sdk-0.0.2469/finbourne_identity_sdk.egg-info/SOURCES.txt` & `finbourne-identity-sdk-0.0.840/finbourne_identity_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,65 @@
 MANIFEST.in
-README.md
 setup.py
 finbourne_identity/__init__.py
 finbourne_identity/__version__.py
 finbourne_identity/api_client.py
 finbourne_identity/configuration.py
 finbourne_identity/exceptions.py
 finbourne_identity/rest.py
 finbourne_identity/api/__init__.py
 finbourne_identity/api/application_metadata_api.py
 finbourne_identity/api/applications_api.py
 finbourne_identity/api/authentication_api.py
-finbourne_identity/api/identity_provider_api.py
-finbourne_identity/api/me_api.py
+finbourne_identity/api/domains_api.py
 finbourne_identity/api/personal_authentication_tokens_api.py
 finbourne_identity/api/roles_api.py
 finbourne_identity/api/tokens_api.py
 finbourne_identity/api/users_api.py
 finbourne_identity/models/__init__.py
 finbourne_identity/models/access_controlled_action.py
 finbourne_identity/models/access_controlled_resource.py
 finbourne_identity/models/action_id.py
-finbourne_identity/models/add_scim_response.py
+finbourne_identity/models/agreement_response.py
 finbourne_identity/models/api_key.py
 finbourne_identity/models/authentication_information.py
 finbourne_identity/models/create_api_key.py
 finbourne_identity/models/create_application_request.py
+finbourne_identity/models/create_domain_request.py
 finbourne_identity/models/create_role_request.py
 finbourne_identity/models/create_user_request.py
 finbourne_identity/models/created_api_key.py
-finbourne_identity/models/current_user_response.py
-finbourne_identity/models/error_detail.py
+finbourne_identity/models/domain_id.py
+finbourne_identity/models/domain_response.py
 finbourne_identity/models/id_selector_definition.py
 finbourne_identity/models/identifier_part_schema.py
 finbourne_identity/models/link.py
-finbourne_identity/models/list_users_response.py
 finbourne_identity/models/lusid_problem_details.py
 finbourne_identity/models/lusid_validation_problem_details.py
 finbourne_identity/models/o_auth_application.py
+finbourne_identity/models/problem_details.py
 finbourne_identity/models/resource_list_of_access_controlled_resource.py
+finbourne_identity/models/role.py
 finbourne_identity/models/role_id.py
 finbourne_identity/models/role_response.py
-finbourne_identity/models/set_password.py
-finbourne_identity/models/set_password_response.py
 finbourne_identity/models/support_access_expiry.py
-finbourne_identity/models/support_access_expiry_with_role.py
 finbourne_identity/models/support_access_request.py
 finbourne_identity/models/support_access_response.py
-finbourne_identity/models/support_role.py
-finbourne_identity/models/support_roles_response.py
-finbourne_identity/models/temporary_password.py
 finbourne_identity/models/update_role_request.py
 finbourne_identity/models/update_user_request.py
+finbourne_identity/models/user_id.py
 finbourne_identity/models/user_response.py
-finbourne_identity/models/user_summary.py
 finbourne_identity/tcp/__init__.py
 finbourne_identity/tcp/tcp_keep_alive_probes.py
 finbourne_identity/utilities/__init__.py
 finbourne_identity/utilities/api_client_builder.py
 finbourne_identity/utilities/api_client_factory.py
 finbourne_identity/utilities/api_configuration.py
 finbourne_identity/utilities/api_configuration_loader.py
 finbourne_identity/utilities/config_keys.json
-finbourne_identity/utilities/config_keys.py
 finbourne_identity/utilities/finbourne_identity_retry.py
 finbourne_identity/utilities/proxy_config.py
 finbourne_identity/utilities/refreshing_token.py
 finbourne_identity_sdk.egg-info/PKG-INFO
 finbourne_identity_sdk.egg-info/SOURCES.txt
 finbourne_identity_sdk.egg-info/dependency_links.txt
 finbourne_identity_sdk.egg-info/requires.txt
```

### Comparing `finbourne-identity-sdk-0.0.2469/setup.py` & `finbourne-identity-sdk-0.0.840/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = [
+    "six >= 1.10",
     "certifi >= 14.05.14",
     "python-dateutil >= 2.5.3",
-    "requests >= 2.27.1",
-    "six >= 1.10",
-    "urllib3 >= 1.26.9",
-
-    "finbourne-sdk-utilities >= 0.0.10",
+    "urllib3 >= 1.15.1",
+    "requests >= 2.21.0"
 ]
 
 version = {}
 with open("./finbourne_identity/__version__.py") as fp:
     exec(fp.read(), version)
 
 setup(
```

