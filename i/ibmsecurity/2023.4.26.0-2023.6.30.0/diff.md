# Comparing `tmp/ibmsecurity-2023.4.26.0.tar.gz` & `tmp/ibmsecurity-2023.6.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmsecurity-2023.4.26.0.tar", last modified: Wed Apr 26 06:43:56 2023, max compression
+gzip compressed data, was "ibmsecurity-2023.6.30.0.tar", last modified: Fri Jun 30 15:38:48 2023, max compression
```

## Comparing `ibmsecurity-2023.4.26.0.tar` & `ibmsecurity-2023.6.30.0.tar`

### file list

```diff
@@ -1,482 +1,482 @@
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.788097 ibmsecurity-2023.4.26.0/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11357 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/LICENSE
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       20 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/MANIFEST.in
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8525 2023-04-26 06:43:56.788097 ibmsecurity-2023.4.26.0/PKG-INFO
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7743 2023-04-26 06:40:53.000000 ibmsecurity-2023.4.26.0/README.md
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.734097 ibmsecurity-2023.4.26.0/ibmsecurity/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.736097 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3433 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/ibmappliance.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    31351 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isamappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1644 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isamappliance_adminproxy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18326 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isdsappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isdsappliance_adminproxy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18192 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isvgappliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isvgappliance_adminproxy.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.736097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.738097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.739097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9327 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policies.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17324 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policy_attachments.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12329 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policy_sets.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9048 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_policy.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10224 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/advanced_configuration.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.739097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    32357 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/clients.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    22725 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/definitions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2135 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1337 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3427 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/grants.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1972 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/grants_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5722 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/attribute_matchers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7605 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/attributes.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.740097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2140 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/mechanism_types.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11692 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/mechanisms.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9722 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/policies.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.741097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      519 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1674 2023-03-10 12:33:20.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2441 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1758 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5016 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4225 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/database.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.741097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2845 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/fingerprints.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2450 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/userids.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7519 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/extensions.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.742097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)        0 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6842 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/metadata.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2260 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/registrations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7358 2023-04-26 06:28:55.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/relying_parties.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     1002 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/u2f_migration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9375 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mapping_rules.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.742097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/__init__.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     1547 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6601 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1808 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/transactions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1873 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/obligation_types.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6944 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/obligations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1767 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/password_vault.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.743097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3504 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4072 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/database.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4159 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7172 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/javascript.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4034 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/ldap.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4238 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/qradar.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4147 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/restful.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1963 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/types.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8728 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/risk_profiles.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.744097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/__init__.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     6341 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/directory.py
--rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     9107 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5894 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/root.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.745097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2295 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/enterprise_profile.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2900 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ext_auth_service.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2709 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/general.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4086 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/isam_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1226 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ldap_attrs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      812 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ldap_objs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4968 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/mode.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20221 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/scim.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2635 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/user_profile.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7630 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.746097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6662 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ci.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2248 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/connection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6994 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/isamruntime.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6985 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/jdbc.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7368 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ldap.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8952 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/redis.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7129 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/smtp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7285 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ws.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1831 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_info.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.747097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4826 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7573 2023-03-10 12:33:20.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4287 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/application_logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.751097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3882 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/activation.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20896 2023-02-16 15:32:19.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4351 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3653 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/application_database_settings.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      912 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/application_locale.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8126 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/audit_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6044 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      863 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cli.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.753097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      652 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/config_database.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11257 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2218 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/log.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6205 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/node.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2472 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      653 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/runtime_database.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      622 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/signature.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1483 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4844 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/date_time.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2903 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/dsc.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8366 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/extensions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1077 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/file_downloads.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5289 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/fips.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3328 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/firmware.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     5699 2021-10-07 13:52:15.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1839 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/geolocation_db.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.753097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2130 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/name.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4087 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2902 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/license.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2757 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/lmi.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1914 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/lmi_tracing.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5491 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authentication.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.754097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1368 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      793 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/feature.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4427 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2166 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_feature.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2474 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2447 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2023-04-26 06:40:53.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_ssl_certificate.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.755097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      704 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/active_status.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      344 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3982 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/dns.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.756097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.756097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2622 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6312 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.757097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5935 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2157 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/log.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4414 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4736 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/error_page.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5983 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/ha.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.757097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6046 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8785 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2691 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/layer.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6110 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/servers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4456 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/ssl.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8331 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1354 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/hostname.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5962 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7005 2021-10-07 13:52:15.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_ipv4.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6360 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_ipv6.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5669 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_vlan.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3269 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/packet_trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13725 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/static_routes.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2109 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/test_connection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      544 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/overview.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.758098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/facility.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6350 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/forwarder.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4537 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      646 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      582 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/instances.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/severity.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      474 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/sources.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.759097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1365 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/cluster.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5240 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/listening_interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2927 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3567 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/scheduled_security_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1638 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/service_agreement.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)      834 2021-10-07 13:52:15.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/setup_complete.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5499 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/silent_config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10170 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/snmp_monitoring.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.760097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7048 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4258 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9568 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1782 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/replication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9229 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6520 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.760097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2147 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/groups.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3798 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/users.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.761098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2033 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4748 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/email.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4977 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/logdb.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4755 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7408 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/snmp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      524 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/update_history.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8752 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/update_servers.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      307 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/version.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.762097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.762097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.762097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.762097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/db_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/db_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4851 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      862 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/publish.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.762097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/service_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/service_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4484 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/service_configuration/configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1411 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/event_log.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.764098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1935 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/alias_service.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1703 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/alias_service_settings.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6693 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/attribute_source.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1414 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/connector_instructions.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13427 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/federations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/partner_templates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14331 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/partners.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9196 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/point_of_contact.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.765097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13879 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/module_chains.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2200 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/modules.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7364 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/templates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9066 2023-03-10 12:33:20.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/statistics.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.767097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.768097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8798 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/cors_policies.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11745 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/documentation_root.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7880 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/policies.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.768097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1190 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/instances.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    28901 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/resources.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    50909 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/servers.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.769097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2527 2023-04-21 16:11:07.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      522 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/group.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.769097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3012 2023-04-21 16:11:07.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/cleanup.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.770097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12469 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4436 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4392 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8025 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/instance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3375 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6440 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6798 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/client_certificate_mapping.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4502 2023-03-10 12:33:20.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/dsc.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.771098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      647 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3038 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/debug.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3262 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/group.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2542 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/suffix.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/user.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10067 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/fsso.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.771098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.771098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7943 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2387 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8572 2023-04-21 16:11:07.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/http_transformation.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.771098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/iag/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/iag/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3274 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/iag/export.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6591 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/junction_mapping.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.773097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3633 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6590 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6410 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4593 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/domains.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3231 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8384 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3996 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      808 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/test.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3307 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/ltpa_key.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4930 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/password_strength.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1924 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/query_sitecontents.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7102 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/rate_limiting.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.775097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2314 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1223 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2544 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.775097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13869 2023-01-20 12:28:18.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3853 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4108 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4206 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10967 2023-04-21 16:11:07.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/instance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2062 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    37637 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/junctions.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6224 2023-02-16 15:32:19.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2698 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/logs.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.776097 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5472 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5021 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9878 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2745 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3510 2021-06-04 12:46:11.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7434 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/statistics.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8251 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9736 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5145 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/rsa_securid_config.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.777098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/__init__.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.777098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11148 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/entry.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3006 2021-10-07 13:52:15.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3402 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/stanza.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.777098 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6922 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2895 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3118 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/object.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      840 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/pdadmin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4728 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/pop.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8404 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1242 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/replication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/trace.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4361 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/sso_keys.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7154 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/url_mapping.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11682 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/user_name_mapping.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.780098 ibmsecurity-2023.4.26.0/ibmsecurity/isds/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3372 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6037 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1982 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/config.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/date_time.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/firmware.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/hostnames.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1677 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2930 2021-03-08 12:58:33.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/license.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3849 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/server.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/snmp_monitoring.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1713 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/statistics.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.781098 ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/snmp.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/token.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8747 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isds/update_servers.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.784098 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/admin.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/advanced_tuning_parameters.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4858 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/appliance.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7701 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/available_updates.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2448 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/certstore_personal.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2233 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/certstore_signer.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.784098 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/cm/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/cm/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1998 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/cm/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/date_time.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.784098 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/db/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/db/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      340 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/db/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/firmware.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/fixpack.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/host_records.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/hostnames.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.786097 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2418 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/certstore_personal.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4253 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/certstore_signer.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13698 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/db.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3888 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/external_library.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      921 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/guided_setup.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4584 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/jvm_property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3691 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/keystore.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7897 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/ldap.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6874 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/mail.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3778 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/nls.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10525 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/openid.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1937 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6655 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/property.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1000 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/property_file.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4902 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/workflowextension.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1735 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/interfaces.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1425 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/lmi.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7315 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/lmi_auth.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/logs.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4135 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/management_authentication.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2454 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/management_ssl_certificate.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      329 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/notifications.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.786097 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/sdi/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/sdi/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2088 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/sdi/process.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1781 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/service_agreement.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      946 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/setup_complete.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/snapshots.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/snmp_monitoring.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      323 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/startup.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/support.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.787098 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/alerts.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/rsyslog.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2023-03-10 08:34:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/snmp.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.787098 ibmsecurity-2023.4.26.0/ibmsecurity/user/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/user/__init__.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      528 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/user/applianceuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      483 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/user/isamuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      526 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/user/isdsapplianceuser.py
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      409 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/user/user.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.788097 ibmsecurity-2023.4.26.0/ibmsecurity/utilities/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.4.26.0/ibmsecurity/utilities/__init__.py
--rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    10333 2022-05-19 14:24:42.000000 ibmsecurity-2023.4.26.0/ibmsecurity/utilities/tools.py
-drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:43:56.734097 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8525 2023-04-26 06:43:56.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/PKG-INFO
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18207 2023-04-26 06:43:56.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/SOURCES.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-04-26 06:43:56.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/dependency_links.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-03-10 12:34:43.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/not-zip-safe
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       32 2023-04-26 06:43:56.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/requires.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       12 2023-04-26 06:43:56.000000 ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/top_level.txt
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      899 2023-04-26 06:43:44.000000 ibmsecurity-2023.4.26.0/pyproject.toml
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       38 2023-04-26 06:43:56.788097 ibmsecurity-2023.4.26.0/setup.cfg
--rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1164 2023-04-26 06:43:44.000000 ibmsecurity-2023.4.26.0/setup.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.844297 ibmsecurity-2023.6.30.0/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11357 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/LICENSE
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       20 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/MANIFEST.in
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8525 2023-06-30 15:38:48.844297 ibmsecurity-2023.6.30.0/PKG-INFO
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7743 2023-04-26 06:40:53.000000 ibmsecurity-2023.6.30.0/README.md
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.755297 ibmsecurity-2023.6.30.0/ibmsecurity/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.757297 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3433 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/ibmappliance.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    31351 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isamappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1644 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isamappliance_adminproxy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18326 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isdsappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isdsappliance_adminproxy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18192 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isvgappliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1899 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isvgappliance_adminproxy.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.758297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.761297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.762297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9327 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policies.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    17324 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policy_attachments.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12329 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policy_sets.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9048 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_policy.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10224 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/advanced_configuration.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.764297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    32357 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/clients.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    22725 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/definitions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2135 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1337 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3427 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/grants.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1972 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/grants_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5722 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/attribute_matchers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7605 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/attributes.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.765297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2140 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/mechanism_types.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11692 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/mechanisms.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9722 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/policies.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.766297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      519 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1674 2023-03-10 12:33:20.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2441 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1758 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5016 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4225 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/database.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.766297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2845 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/fingerprints.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2450 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/userids.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7519 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/extensions.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.767297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)        0 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6842 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/metadata.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2260 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/registrations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7358 2023-04-26 06:28:55.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/relying_parties.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     1002 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/u2f_migration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9375 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mapping_rules.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.768297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/__init__.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     1547 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6601 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1808 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/transactions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1873 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/obligation_types.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6944 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/obligations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1767 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/password_vault.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.770297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3504 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4072 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/database.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4159 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7172 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/javascript.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4034 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/ldap.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4238 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/qradar.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4147 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/restful.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1963 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/types.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8728 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/risk_profiles.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.771297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/__init__.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     6341 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/directory.py
+-rwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)     9107 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5894 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/root.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.773297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2295 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/enterprise_profile.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2900 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ext_auth_service.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2709 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/general.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4086 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/isam_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1226 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ldap_attrs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      812 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ldap_objs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4968 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/mode.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20221 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/scim.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2635 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/user_profile.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7630 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.775297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6662 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ci.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2248 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/connection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6994 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/isamruntime.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6985 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/jdbc.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7368 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ldap.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     8952 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/redis.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7129 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/smtp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7285 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ws.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1831 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_info.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.776297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4826 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7573 2023-03-10 12:33:20.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4287 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/application_logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.784297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3882 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/activation.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    20896 2023-02-16 15:32:19.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4351 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3653 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/application_database_settings.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      912 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/application_locale.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8126 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/audit_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6572 2023-06-30 14:06:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      863 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cli.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.786297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      652 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/config_database.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    11257 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2218 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/log.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6205 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/node.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2472 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      653 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/runtime_database.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      622 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/signature.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1483 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4844 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/date_time.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2903 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/dsc.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8366 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/extensions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1077 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/file_downloads.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5289 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/fips.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3328 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/firmware.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     5699 2021-10-07 13:52:15.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1839 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/geolocation_db.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.786297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2130 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/name.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4087 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2902 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/license.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2757 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/lmi.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1914 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/lmi_tracing.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5491 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authentication.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.788297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1368 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      793 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/feature.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4427 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2166 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_feature.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2474 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2447 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2023-04-26 06:40:53.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_ssl_certificate.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.791297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      704 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/active_status.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      344 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3982 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/dns.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.792297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.792297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2622 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6312 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.793297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5935 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2157 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/log.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4414 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4736 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/error_page.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5983 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/ha.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.794297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6046 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8785 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2691 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/layer.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6110 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/servers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4456 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/ssl.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8331 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1354 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/hostname.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5962 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7005 2021-10-07 13:52:15.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_ipv4.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6360 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_ipv6.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5669 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_vlan.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3269 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/packet_trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13725 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/static_routes.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2109 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/test_connection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      544 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/overview.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.796297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/facility.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     6350 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/forwarder.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4537 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      646 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      582 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/instances.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      490 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/severity.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      474 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/sources.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.797297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1365 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/cluster.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5240 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/listening_interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2927 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3567 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/scheduled_security_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1638 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/service_agreement.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)      834 2021-10-07 13:52:15.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/setup_complete.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5499 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/silent_config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10170 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/snmp_monitoring.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.798297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     7048 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4258 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9568 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1782 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/replication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9229 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6520 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.799297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2147 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/groups.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3798 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/users.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.800297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2033 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4748 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/email.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4977 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/logdb.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4755 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7408 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/snmp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      524 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/update_history.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8752 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/update_servers.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      307 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/version.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.800297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.800297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.801297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.801297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/db_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/db_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4851 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      862 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/publish.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.801297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/service_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/service_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4484 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/service_configuration/configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1411 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/event_log.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.803297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1935 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/alias_service.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1703 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/alias_service_settings.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6693 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/attribute_source.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1414 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/connector_instructions.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13427 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/federations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2194 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/partner_templates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    14331 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/partners.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     9196 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/point_of_contact.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.804297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13879 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/module_chains.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2200 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/modules.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7364 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/templates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9066 2023-03-10 12:33:20.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/statistics.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.808297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.808297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8798 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/cors_policies.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11745 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/documentation_root.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7880 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/policies.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.809297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1190 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/instances.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    28901 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/resources.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    53403 2023-06-30 14:43:30.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/servers.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.810297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2527 2023-04-21 16:11:07.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      522 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/group.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.811297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3012 2023-04-21 16:11:07.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/cleanup.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.812297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    12469 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4436 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4392 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8025 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/instance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3375 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6440 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6798 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/client_certificate_mapping.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4502 2023-03-10 12:33:20.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/dsc.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.813297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      647 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3038 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/debug.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3262 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/group.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2542 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/suffix.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3831 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/user.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10067 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/fsso.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.813297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.814297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7943 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     2387 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8572 2023-04-21 16:11:07.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/http_transformation.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.814297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/iag/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/iag/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3274 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/iag/export.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6591 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/junction_mapping.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.816297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3633 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6590 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6410 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4593 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/domains.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4092 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3231 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8384 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3996 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      808 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/test.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3307 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/ltpa_key.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4930 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/password_strength.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1924 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/query_sitecontents.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7102 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/rate_limiting.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.820297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2314 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1223 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2544 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.821297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    13869 2023-01-20 12:28:18.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3853 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4108 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     4206 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10967 2023-04-21 16:11:07.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/instance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2062 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    39328 2023-06-30 14:50:05.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/junctions.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6970 2023-06-30 14:32:23.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2698 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/logs.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.822297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5472 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5021 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9878 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2745 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3510 2021-06-04 12:46:11.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7434 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/statistics.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8251 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     9736 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     5145 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/rsa_securid_config.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.824297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/__init__.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.825297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11148 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/entry.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)     3006 2021-10-07 13:52:15.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3402 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/stanza.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.826297 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6922 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2895 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3118 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/object.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      840 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/pdadmin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4728 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/pop.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8404 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1242 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/replication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3765 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/trace.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4361 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/sso_keys.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7154 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/url_mapping.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    11682 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/user_name_mapping.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.831297 ibmsecurity-2023.6.30.0/ibmsecurity/isds/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3372 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6037 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1982 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/config.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/date_time.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/firmware.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/hostnames.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1677 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2930 2021-03-08 12:58:33.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/license.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3849 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/server.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/snmp_monitoring.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1713 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/statistics.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.832297 ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/snmp.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/token.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8747 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isds/update_servers.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.837297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3470 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/admin.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4859 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/advanced_tuning_parameters.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4858 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/appliance.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7701 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/available_updates.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2448 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/certstore_personal.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2233 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/certstore_signer.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.837297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/cm/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/cm/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1998 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/cm/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3468 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/date_time.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.838297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/db/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/db/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      340 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/db/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2943 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/firmware.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3978 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/fixpack.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2117 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/host_records.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1827 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/hostnames.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.841297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2418 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/certstore_personal.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4253 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/certstore_signer.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    13698 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/db.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3888 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/external_library.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      921 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/guided_setup.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4584 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/jvm_property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3691 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/keystore.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7897 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/ldap.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6874 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/mail.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     3778 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/nls.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    10525 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/openid.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1937 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6655 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/property.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1000 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/property_file.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4902 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/workflowextension.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1735 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/interfaces.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1425 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/lmi.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7315 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/lmi_auth.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      267 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/logs.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4135 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/management_authentication.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2454 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/management_ssl_certificate.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      329 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/notifications.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.842297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/sdi/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-04-26 06:28:55.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/sdi/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2088 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/sdi/process.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1781 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/service_agreement.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      946 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/setup_complete.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     6043 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/snapshots.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4746 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/snmp_monitoring.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      323 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/startup.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4740 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/support.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.842297 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     2018 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/alerts.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     4730 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/rsyslog.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     7383 2023-03-10 08:34:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/snmp.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.844297 ibmsecurity-2023.6.30.0/ibmsecurity/user/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/user/__init__.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      528 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/user/applianceuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      483 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/user/isamuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      526 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/user/isdsapplianceuser.py
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      409 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/user/user.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.844297 ibmsecurity-2023.6.30.0/ibmsecurity/utilities/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        0 2020-03-11 13:09:08.000000 ibmsecurity-2023.6.30.0/ibmsecurity/utilities/__init__.py
+-rw-r--r--   0 tbosmans  (1000) tbosmans  (1001)    10333 2022-05-19 14:24:42.000000 ibmsecurity-2023.6.30.0/ibmsecurity/utilities/tools.py
+drwxrwxr-x   0 tbosmans  (1000) tbosmans  (1001)        0 2023-06-30 15:38:48.756297 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     8525 2023-06-30 15:38:48.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/PKG-INFO
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)    18207 2023-06-30 15:38:48.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-06-30 15:38:48.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)        1 2023-03-10 12:34:43.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/not-zip-safe
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       32 2023-06-30 15:38:48.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/requires.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       12 2023-06-30 15:38:48.000000 ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/top_level.txt
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)      899 2023-06-30 15:35:46.000000 ibmsecurity-2023.6.30.0/pyproject.toml
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)       38 2023-06-30 15:38:48.844297 ibmsecurity-2023.6.30.0/setup.cfg
+-rw-rw-r--   0 tbosmans  (1000) tbosmans  (1001)     1164 2023-06-30 15:35:46.000000 ibmsecurity-2023.6.30.0/setup.py
```

### Comparing `ibmsecurity-2023.4.26.0/LICENSE` & `ibmsecurity-2023.6.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/PKG-INFO` & `ibmsecurity-2023.6.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmsecurity
-Version: 2023.4.26.0
+Version: 2023.6.30.0
 Summary: Idempotent functions for IBM Security Appliance REST APIs
 Home-page: 
 Author: IBM
 Author-email: IBM <secorch@us.ibm.com>
 Project-URL: Homepage, https://github.com/IBM-Security/ibmsecurity
 Project-URL: Bug Tracker, https://github.com/IBM-Security/ibmsecurity/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibmsecurity-2023.4.26.0/README.md` & `ibmsecurity-2023.6.30.0/README.md`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/ibmappliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/ibmappliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isamappliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isamappliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isamappliance_adminproxy.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isamappliance_adminproxy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isdsappliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isdsappliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isdsappliance_adminproxy.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isdsappliance_adminproxy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isvgappliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isvgappliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/appliance/isvgappliance_adminproxy.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/appliance/isvgappliance_adminproxy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policies.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policy_attachments.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policy_attachments.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_control/policy_sets.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_control/policy_sets.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/access_policy.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/access_policy.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/advanced_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/advanced_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/clients.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/clients.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/definitions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/definitions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/dynamic_clients.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/dynamic_clients_migration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/grants.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/grants.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/api_protection/grants_user.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/api_protection/grants_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/attribute_matchers.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/attribute_matchers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/attributes.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/attributes.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/mechanism_types.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/mechanism_types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/mechanisms.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/mechanisms.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/policies.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdconf.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/sdopts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp/securid.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/authentication/rsa_otp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/authentication/rsa_otp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/database.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/fingerprints.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/fingerprints.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/devices/userids.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/devices/userids.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/extensions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/extensions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/metadata.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/metadata.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/registrations.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/registrations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/relying_parties.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/relying_parties.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/fido2/u2f_migration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/fido2/u2f_migration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mapping_rules.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mapping_rules.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/push_notification_registration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/mmfa/transactions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/mmfa/transactions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/obligation_types.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/obligation_types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/obligations.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/obligations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/password_vault.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/password_vault.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/all.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/database.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/fiberlink.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/javascript.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/javascript.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/ldap.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/qradar.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/qradar.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/restful.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/restful.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/policy_information_points/types.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/policy_information_points/types.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/risk_profiles.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/risk_profiles.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/directory.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/directory.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/file.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/runtime_template/root.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/runtime_template/root.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/enterprise_profile.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/enterprise_profile.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ext_auth_service.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ext_auth_service.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/general.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/general.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/group.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/isam_user.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/isam_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ldap_attrs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ldap_attrs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/ldap_objs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/ldap_objs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/mode.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/mode.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/scim.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/scim.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim/user_profile.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim/user_profile.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/scim_custom_schema_extensions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ci.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ci.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/connection.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/connection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/isamruntime.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/isamruntime.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/jdbc.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/jdbc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ldap.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/redis.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/redis.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/smtp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/smtp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/server_connections/ws.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/server_connections/ws.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_info.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_info.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/group.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/aac/user_registry/user.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/aac/user_registry/user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/appliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/application_logs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/application_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/activation.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/activation.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/admin.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/advanced_tuning_parameters.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/application_database_settings.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/application_database_settings.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/application_locale.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/application_locale.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/audit_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/audit_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/available_updates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/available_updates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import ibmsecurity.utilities.tools
 
 logger = logging.getLogger(__name__)
 
 
 def get(isamAppliance, check_mode=False, force=False):
     """
     Retrieve available updates
@@ -126,22 +127,30 @@
                                                 ]
                                                 })
             isamAppliance.facts['version'] = version
             return ret_obj
 
     return isamAppliance.create_return_object()
 
-
 def _check(isamAppliance, type, version, release_date, name):
     ret_obj = get(isamAppliance)
+    warnings = []
     for upd in ret_obj['data']:
         # If there is an installation in progress then abort
-        if upd['state'] == 'Installing':
-            logger.debug("Detecting a state of installing...")
-            return False
+        # API changed in v10.0.5.0 , state, schedule_date, iso_scheduled_date and expired_install are no longer available.
+        if ibmsecurity.utilities.tools.version_compare(isamAppliance.facts["version"], "10.0.5.0") < 0:
+            if upd['state'] == 'Installing':
+                logger.debug("Detecting a state of installing...")
+                return False
+        else:
+            warnings.append("Appliance at version: {0}, state can no longer be checked in 10.0.5.0 or higher. Ignoring for this call.".format(
+                    isamAppliance.facts["version"]))
+
+        logger.info(upd)
+
         if upd['type'] == type and upd['version'] == version and upd['release_date'] == release_date and upd[
             'name'] == name:
             logger.debug("Requested firmware ready for install...")
             return True
 
     logger.debug("Requested firmware not available for install...")
```

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cli.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cli.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/config_database.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/config_database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/log.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/node.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/node.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/property.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/runtime_database.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/runtime_database.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/signature.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/signature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/cluster/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/cluster/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/date_time.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/dsc.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/dsc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/extensions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/extensions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/file_downloads.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/file_downloads.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/fips.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/fips.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/firmware.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/fixpack.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/geolocation_db.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/geolocation_db.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/name.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/name.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/host/records.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/host/records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/license.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/license.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/lmi.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/lmi.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/lmi_tracing.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/lmi_tracing.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authentication.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authentication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/feature.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/feature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_feature.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_feature.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_group.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_authorization/role_user.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_authorization/role_user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/management_ssl_certificate.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/management_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/active_status.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/active_status.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/dns.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/dns.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/at_logging.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/advanced_tuning/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/attributes/log.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/attributes/log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/error_page.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/error_page.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/ha.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/ha.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/layer.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/layer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/services/servers.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/services/servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/felb/ssl.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/felb/ssl.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/host_records.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/hostname.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/hostname.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_ipv4.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_ipv4.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_ipv6.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_ipv6.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/interfaces_vlan.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/interfaces_vlan.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/packet_trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/packet_trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/static_routes.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/static_routes.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/network/test_connection.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/network/test_connection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/overview.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/overview.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/forwarder.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/forwarder.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/forwarder_sources.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/instance_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/remote_syslog/instances.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/remote_syslog/instances.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/cluster.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/cluster.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/listening_interfaces.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/listening_interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/process.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/runtime/tuning_parameters.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/runtime/tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/scheduled_security_updates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/scheduled_security_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/service_agreement.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/service_agreement.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/setup_complete.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/setup_complete.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/silent_config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/silent_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/snapshots.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/snmp_monitoring.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/certificate_databases.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/certificate_requests.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/personal_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/replication.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/replication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/ssl_certificates/signer_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/support.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/groups.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/groups.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/sysaccount/users.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/sysaccount/users.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/alerts.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/email.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/email.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/logdb.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/logdb.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/rsyslog.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/system_alerts/snmp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/update_history.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/update_history.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/base/update_servers.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/base/update_servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/base/network/db_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/publish.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/publish.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/docker/service_configuration/configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/docker/service_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/event_log.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/event_log.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/alias_service.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/alias_service.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/alias_service_settings.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/alias_service_settings.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/attribute_source.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/attribute_source.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/connector_instructions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/connector_instructions.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/federations.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/federations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/partner_templates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/partner_templates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/partners.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/partners.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/point_of_contact.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/point_of_contact.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/module_chains.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/module_chains.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/modules.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/modules.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/fed/sts/templates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/fed/sts/templates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/statistics.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/cors_policies.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/cors_policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/documentation_root.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/documentation_root.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/policies.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/policies.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/instances.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/instances.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/resources.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/resources.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/resources/servers.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/resources/servers.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         insert_session_cookies=None, request_encoding=None, enable_basic_auth=None, key_label=None,
         gso_resource_group=None, junction_cookie_javascript_block=None, client_ip_http=None,
         version_two_cookies=None, ltpa_keyfile=None, authz_rules=None, fsso_config_file=None, username=None,
         password=None, server_uuid=None, server_port=None, virtual_hostname=None, server_dn=None, local_ip=None,
         query_contents=None, case_sensitive_url=None, windows_style_url=None, ltpa_keyfile_password=None,
         https_port=None, http_port=None, proxy_hostname=None, proxy_port=None, sms_environment=None,
         vhost_label=None, junction_force=None, delegation_support=None, scripting_support=None,
+        case_insensitive_url=None,
         check_mode=False, force=False):
     """
     Creating a new API Access Control Resource Server
     """
     server_exist, warnings = _check_server_exist(isamAppliance, instance_name, junction_point)
 
     if force is True or server_exist is False:
@@ -165,15 +166,25 @@
 
             if local_ip is not None:
                 json_data['local_ip'] = local_ip
 
             if query_contents is not None:
                 json_data['query_contents'] = query_contents
 
-            if case_sensitive_url is not None:
+            if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                # If no case_insensitive_url is passed, we take the old one and invert it.
+                # Who thinks it's a good idea to make changes in an API like this ?
+                if case_insensitive_url is not None:
+                    json_data["case_insensitive_url"] = case_insensitive_url
+                elif case_sensitive_url is not None:
+                    if case_sensitive_url.lower() == 'yes':
+                        jct_srv_json["case_insensitive_url"] = 'no'
+                    else:
+                        jct_srv_json["case_insensitive_url"] = 'yes'
+            elif case_sensitive_url is not None:
                 json_data['case_sensitive_url'] = case_sensitive_url
 
             if windows_style_url is not None:
                 json_data['windows_style_url'] = windows_style_url
 
             if ltpa_keyfile_password is not None:
                 json_data['ltpa_keyfile_password'] = ltpa_keyfile_password
@@ -222,14 +233,15 @@
            enable_basic_auth=None, key_label=None, gso_resource_group=None,
            junction_cookie_javascript_block=None, client_ip_http=None, version_two_cookies=None,
            ltpa_keyfile=None, authz_rules=None, fsso_config_file=None, username=None, password=None,
            server_uuid=None, server_port=None, virtual_hostname=None, server_dn=None, local_ip=None,
            query_contents=None, case_sensitive_url=None, windows_style_url=None, ltpa_keyfile_password=None,
            https_port=None, http_port=None, proxy_hostname=None, proxy_port=None, sms_environment=None,
            vhost_label=None, junction_force=True, delegation_support=None, scripting_support=None,
+           case_insensitive_url=None,
            check_mode=False, force=False):
     """
     Updating an existing API Access Control Resource Server
     """
 
     server_exist, warnings = _check_server_exist(isamAppliance, instance_name, junction_point)
     if server_exist is True:
@@ -267,14 +279,15 @@
                                                           username=username,
                                                           password=password,
                                                           server_uuid=server_uuid, server_port=server_port,
                                                           virtual_hostname=virtual_hostname,
                                                           server_dn=server_dn,
                                                           local_ip=local_ip, query_contents=query_contents,
                                                           case_sensitive_url=case_sensitive_url,
+                                                          case_insensitive_url=case_insensitive_url,
                                                           windows_style_url=windows_style_url,
                                                           ltpa_keyfile_password=ltpa_keyfile_password,
                                                           https_port=https_port,
                                                           http_port=http_port, proxy_hostname=proxy_hostname,
                                                           proxy_port=proxy_port,
                                                           sms_environment=sms_environment,
                                                           vhost_label=vhost_label,
@@ -397,15 +410,25 @@
 
             if local_ip is not None:
                 json_data['local_ip'] = local_ip
 
             if query_contents is not None:
                 json_data['query_contents'] = query_contents
 
-            if case_sensitive_url is not None:
+            if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                # If no case_insensitive_url is passed, we take the old one and invert it.
+                # Who thinks it's a good idea to make changes in an API like this ?
+                if case_insensitive_url is not None:
+                    json_data["case_insensitive_url"] = case_insensitive_url
+                elif case_sensitive_url is not None:
+                    if case_sensitive_url.lower() == 'yes':
+                        json_data["case_insensitive_url"] = 'no'
+                    else:
+                        json_data["case_insensitive_url"] = 'yes'
+            elif case_sensitive_url is not None:
                 json_data['case_sensitive_url'] = case_sensitive_url
 
             if windows_style_url is not None:
                 json_data['windows_style_url'] = windows_style_url
 
             if ltpa_keyfile_password is not None:
                 json_data['ltpa_keyfile_password'] = ltpa_keyfile_password
@@ -454,14 +477,15 @@
         enable_basic_auth=None, key_label=None, gso_resource_group=None,
         junction_cookie_javascript_block=None, client_ip_http=None, version_two_cookies=None,
         ltpa_keyfile=None, authz_rules=None, fsso_config_file=None, username=None, password=None,
         server_uuid=None, server_port=None, virtual_hostname=None, server_dn=None, local_ip=None,
         query_contents=None, case_sensitive_url=None, windows_style_url=None, ltpa_keyfile_password=None,
         https_port=None, http_port=None, proxy_hostname=None, proxy_port=None, sms_environment=None,
         vhost_label=None, junction_force=True, delegation_support=None, scripting_support=None,
+        case_insensitive_url=None,
         check_mode=False, force=False):
     server_exist, warnings = _check_server_exist(isamAppliance, instance_name, junction_point)
 
     if server_exist is True:
         return update(isamAppliance=isamAppliance, instance_name=instance_name, junction_point=junction_point,
                       server_hostname=server_hostname, junction_type=junction_type, policy=policy,
                       authentication=authentication, server_type=server_type,
@@ -482,15 +506,17 @@
                       username=username, password=password, server_uuid=server_uuid, server_port=server_port,
                       virtual_hostname=virtual_hostname, server_dn=server_dn, local_ip=local_ip,
                       query_contents=query_contents, case_sensitive_url=case_sensitive_url,
                       windows_style_url=windows_style_url, ltpa_keyfile_password=ltpa_keyfile_password,
                       https_port=https_port, http_port=http_port, proxy_hostname=proxy_hostname,
                       proxy_port=proxy_port, sms_environment=sms_environment, vhost_label=vhost_label,
                       junction_force=junction_force, delegation_support=delegation_support,
-                      scripting_support=scripting_support, check_mode=check_mode, force=force)
+                      scripting_support=scripting_support,
+                      case_insensitive_url=case_insensitive_url,
+                      check_mode=check_mode, force=force)
     else:
         return add(isamAppliance=isamAppliance, instance_name=instance_name, server_hostname=server_hostname,
                    junction_point=junction_point, junction_type=junction_type, policy=policy,
                    authentication=authentication, static_response_headers=static_response_headers, jwt=jwt,
                    junction_hard_limit=junction_hard_limit, junction_soft_limit=junction_soft_limit,
                    basic_auth_mode=basic_auth_mode, tfim_sso=tfim_sso, remote_http_header=remote_http_header,
                    stateful_junction=stateful_junction, http2_junction=http2_junction, http2_proxy=http2_proxy,
@@ -505,15 +531,17 @@
                    username=username, password=password, server_uuid=server_uuid, server_port=server_port,
                    virtual_hostname=virtual_hostname, server_dn=server_dn, local_ip=local_ip,
                    query_contents=query_contents, case_sensitive_url=case_sensitive_url,
                    windows_style_url=windows_style_url, ltpa_keyfile_password=ltpa_keyfile_password,
                    https_port=https_port, http_port=http_port, proxy_hostname=proxy_hostname,
                    proxy_port=proxy_port, sms_environment=sms_environment, vhost_label=vhost_label,
                    junction_force=junction_force, delegation_support=delegation_support,
-                   scripting_support=scripting_support, check_mode=check_mode, force=force)
+                   scripting_support=scripting_support,
+                   case_insensitive_url=case_insensitive_url,
+                   check_mode=check_mode, force=force)
 
 
 def delete(isamAppliance, instance_name, resource_server_name, server_type='standard',
            check_mode=False, force=False):
     """
     Delete an existing API Access Control Resource Server
     """
@@ -735,15 +763,15 @@
                           basic_auth_mode, tfim_sso, remote_http_header, stateful_junction, http2_junction, http2_proxy,
                           sni_name, preserve_cookie, cookie_include_path, transparent_path_junction, mutual_auth,
                           insert_ltpa_cookies, insert_session_cookies, request_encoding, enable_basic_auth, key_label,
                           gso_resource_group, junction_cookie_javascript_block, client_ip_http, version_two_cookies,
                           ltpa_keyfile, authz_rules, fsso_config_file, username, password, server_uuid, server_port,
                           virtual_hostname, server_dn, local_ip, query_contents, case_sensitive_url,
                           windows_style_url, ltpa_keyfile_password, https_port, http_port, proxy_hostname, proxy_port,
-                          sms_environment, vhost_label, delegation_support, scripting_support):
+                          sms_environment, vhost_label, delegation_support, scripting_support, case_insensitive_url):
     ret_obj = get(isamAppliance, instance_name, junction_point)
     current_data = ret_obj['data']
     add_required = False
     json_data = {
         'server_hostname': server_hostname,
         'junction_point': junction_point,
         'junction_type': junction_type.lower(),
@@ -772,18 +800,31 @@
         if srv['server_hostname'] == server_hostname and str(srv['server_port']) == str(server_port):
             logger.debug("Matched a server - {0}.".format(srv))
             server_found = True
             server_json = {
                 'server_hostname': server_hostname,
                 'server_port': str(server_port)
             }
-            if case_sensitive_url is None:
-                server_json['case_sensitive_url'] = 'no'
-            else:
+
+            if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                # If no case_insensitive_url is passed, we take the old one and invert it.
+                # Who thinks it's a good idea to make changes in an API like this ?
+                if case_insensitive_url is not None:
+                    server_json["case_insensitive_url"] = case_insensitive_url
+                elif case_sensitive_url is not None:
+                    if case_sensitive_url.lower() == 'yes':
+                        server_json["case_insensitive_url"] = 'no'
+                    else:
+                        server_json["case_insensitive_url"] = 'yes'
+                else:
+                    server_json["case_insensitive_url"] = 'yes'
+            elif case_sensitive_url is not None:
                 server_json['case_sensitive_url'] = case_sensitive_url
+            else:
+                server_json['case_sensitive_url'] = 'no'
 
             if http_port is None:
                 server_json['http_port'] = str(server_port)
             else:
                 server_json['http_port'] = str(http_port)
 
             if https_port is not None:
```

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/credential.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/api_access_control/utilities/group.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/api_access_control/utilities/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/cleanup.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/cleanup.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/configuration/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/instance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/instance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/logs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/authorization_server/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/authorization_server/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/client_certificate_mapping.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/client_certificate_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/dsc.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/dsc.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/admin.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/debug.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/debug.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/group.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/group.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/suffix.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/suffix.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/embedded_ldap/user.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/embedded_ldap/user.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/fsso.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/fsso.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/collections.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/global_settings/redis_configuration/wrp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/http_transformation.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/http_transformation.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/iag/export.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/iag/export.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/junction_mapping.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/junction_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/ca_paths_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/domains.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/domains.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/keyfiles.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/realms_subsection.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/kerberos_configuration/test.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/kerberos_configuration/test.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/ltpa_key.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/ltpa_key.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/password_strength.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/password_strength.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/query_sitecontents.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/query_sitecontents.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/rate_limiting.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/aac_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/common_configurations.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/common_logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/configuration/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/federation_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/instance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/instance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/junctions.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/junctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         transparent_path_junction=None, mutual_auth=None, insert_session_cookies=None, request_encoding=None,
         enable_basic_auth=None, key_label=None, gso_resource_group=None, junction_cookie_javascript_block=None,
         client_ip_http=None, version_two_cookies=None, ltpa_keyfile=None, authz_rules=None, fsso_config_file=None,
         username=None, password=None, server_uuid=None, local_ip=None, ltpa_keyfile_password=None,
         delegation_support=None, scripting_support=None, insert_ltpa_cookies=None, check_mode=False, force=False,
         http2_junction=None, http2_proxy=None, sni_name=None, description=None,
         priority=None, server_cn=None, silent=None,
+        case_insensitive_url=None,
         warnings=[]):
     """
     Creating a standard or virtual junction
 
     :param isamAppliance:
     :param reverseproxy_id:
     :param junction_point:
@@ -112,14 +113,15 @@
     :param server_port:
     :param junction_type:
     :param virtual_hostname:
     :param server_dn:
     :param query_contents:
     :param stateful_junction:
     :param case_sensitive_url:
+    :param case_insensitive_url: #v10.0.6
     :param windows_style_url:
     :param https_port:
     :param http_port:
     :param proxy_hostname:
     :param proxy_port:
     :param sms_environment:
     :param vhost_label:
@@ -233,16 +235,26 @@
                 jct_json["virtual_hostname"] = virtual_hostname
             if server_dn is not None:
                 jct_json["server_dn"] = server_dn
             if local_ip is not None:
                 jct_json["local_ip"] = local_ip
             if query_contents is not None:
                 jct_json["query_contents"] = query_contents
-            if case_sensitive_url is not None:
-                jct_json["case_sensitive_url"] = case_sensitive_url
+            if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                # If no case_insensitive_url is passed, we take the old one and invert it.
+                # Who thinks it's a good idea to make changes in an API like this ?
+                if case_insensitive_url is not None:
+                    jct_json["case_insensitive_url"] = case_insensitive_url
+                elif case_sensitive_url is not None:
+                    if case_sensitive_url.lower() == 'yes':
+                        jct_json["case_insensitive_url"] = 'no'
+                    else:
+                        jct_json["case_insensitive_url"] = 'yes'
+            elif case_sensitive_url is not None:
+                jct_json['case_sensitive_url'] = case_sensitive_url
             if windows_style_url is not None:
                 jct_json["windows_style_url"] = windows_style_url
             if ltpa_keyfile_password is not None:
                 jct_json["ltpa_keyfile_password"] = ltpa_keyfile_password
             if https_port is not None:
                 jct_json["https_port"] = https_port
             if http_port is not None:
@@ -343,15 +355,16 @@
         basic_auth_mode=None, tfim_sso=None, remote_http_header=None, preserve_cookie=None, cookie_include_path=None,
         transparent_path_junction=None, mutual_auth=None, insert_session_cookies=None, request_encoding=None,
         enable_basic_auth=None, key_label=None, gso_resource_group=None, junction_cookie_javascript_block=None,
         client_ip_http=None, version_two_cookies=None, ltpa_keyfile=None, authz_rules=None, fsso_config_file=None,
         username=None, password=None, server_uuid=None, local_ip=None, ltpa_keyfile_password=None,
         delegation_support=None, scripting_support=None, insert_ltpa_cookies=None, check_mode=False, force=False,
         http2_junction=None, http2_proxy=None, sni_name=None, description=None,
-        priority=None, server_cn=None, silent=None):
+        priority=None, server_cn=None, silent=None,
+        case_insensitive_url=None):
     """
     Setting a standard or virtual junction - compares with existing junction and replaces if changes are detected
     TODO: Compare all the parameters in the function - LTPA, BA are some that are not being compared
     """
     warnings = []
     add_required = False
     # See if it's a virtual or standard junction
@@ -373,18 +386,30 @@
                 if srv['server_hostname'] == server_hostname and str(srv['server_port']) == str(server_port):
                     logger.debug("Matched a server - {0}.".format(srv))
                     server_found = True
                     server_json = {
                         'server_hostname': server_hostname,
                         'server_port': str(server_port)
                     }
-                    if case_sensitive_url is None:
-                        server_json['case_sensitive_url'] = 'no'
-                    else:
+                    if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                        # If no case_insensitive_url is passed, we take the old one and invert it.
+                        # Who thinks it's a good idea to make changes in an API like this ?
+                        if case_insensitive_url is not None:
+                            server_json["case_insensitive_url"] = case_insensitive_url
+                        elif case_sensitive_url is not None:
+                            if case_sensitive_url.lower() == 'yes':
+                                server_json["case_insensitive_url"] = 'no'
+                            else:
+                                server_json["case_insensitive_url"] = 'yes'
+                        else:
+                            server_json["case_insensitive_url"] = 'yes'
+                    elif case_sensitive_url is not None:
                         server_json['case_sensitive_url'] = case_sensitive_url
+                    else:
+                        server_json['case_sensitive_url'] = 'no'
                     if http_port is None:
                         server_json['http_port'] = str(server_port)
                     else:
                         server_json['http_port'] = str(http_port)
                     if local_ip is None:
                         server_json['local_ip'] = ''
                     else:
@@ -651,14 +676,15 @@
                    version_two_cookies=version_two_cookies, ltpa_keyfile=ltpa_keyfile, authz_rules=authz_rules,
                    fsso_config_file=fsso_config_file, username=username, password=password, server_uuid=server_uuid,
                    local_ip=local_ip, ltpa_keyfile_password=ltpa_keyfile_password,
                    delegation_support=delegation_support, scripting_support=scripting_support,
                    insert_ltpa_cookies=insert_ltpa_cookies, check_mode=check_mode, force=True,
                    http2_junction=http2_junction, http2_proxy=http2_proxy, sni_name=sni_name, description=description,
                    priority=priority, server_cn=server_cn, silent=silent,
+                   case_insensitive_url=case_insensitive_url,
                    warnings=warnings)
 
     return isamAppliance.create_return_object()
 
 
 def compare(isamAppliance1, isamAppliance2, reverseproxy_id, reverseproxy_id2=None):
     """
```

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/junctions_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
     return ret_obj_new
 
 
 def add(isamAppliance, reverseproxy_id, junction_point, server_hostname, junction_type, server_port, server_dn=None,
         stateful_junction='no', case_sensitive_url='no', windows_style_url='no', virtual_hostname=None,
         virtual_https_hostname=None, query_contents=None, https_port=None, http_port=None, proxy_hostname=None,
-        proxy_port=None, sms_environment=None, vhost_label=None, server_uuid=None, priority=None, server_cn=None, check_mode=False, force=False):
+        proxy_port=None, sms_environment=None, vhost_label=None, server_uuid=None, priority=None, server_cn=None,
+        case_insensitive_url=None, check_mode=False, force=False):
     """
     Adding a back-end server to an existing standard or virtual junctions
 
     :param isamAppliance:
     :param reverseproxy_id:
     :param junctionname:
     :param server_hostname:
@@ -35,14 +36,15 @@
     :param server_port:
     :param virtual_hostname:
     :param virtual_https_hostname:
     :param server_dn:
     :param query_contents:
     :param stateful_junction:
     :param case_sensitive_url:
+    :param case_insensitive_url:  #v1.0.6+
     :param windows_style_url:
     :param https_port:
     :param http_port:
     :param proxy_hostname:
     :param proxy_port:
     :param sms_environment:
     :param vhost_label:
@@ -63,17 +65,28 @@
         else:
             jct_srv_json = {
                 "junction_point": junction_point,
                 "junction_type": junction_type,
                 "server_hostname": server_hostname,
                 "server_port": server_port,
                 "stateful_junction": stateful_junction,
-                "case_sensitive_url": case_sensitive_url,
                 "windows_style_url": windows_style_url,
             }
+            if tools.version_compare(isamAppliance.facts["version"], "10.0.6.0") >= 0:
+                # If no case_insensitive_url is passed, we take the old one and invert it.
+                # Who thinks it's a good idea to make changes in an API like this ?
+                if case_insensitive_url is None:
+                    if case_sensitive_url.lower() == 'yes':
+                        jct_srv_json["case_insensitive_url"] = 'no'
+                    else:
+                        jct_srv_json["case_insensitive_url"] = 'yes'
+                else:
+                    jct_srv_json["case_insensitive_url"] = case_insensitive_url
+            else:
+                jct_srv_json["case_sensitive_url"] = case_sensitive_url
             if https_port is not None:
                 jct_srv_json["https_port"] = https_port
             if http_port is not None:
                 jct_srv_json["http_port"] = http_port
             if proxy_hostname is not None:
                 jct_srv_json["proxy_hostname"] = proxy_hostname
             if proxy_port is not None:
```

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/logs.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/logs.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/all.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/directory.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/management_root/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/mmfa_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/oauth_configuration.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/statistics.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/reverse_proxy/transaction_logging.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/rsa_securid_config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/rsa_securid_config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/entry.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/entry.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/file.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/configuration/stanza.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/configuration/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/stanza.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/federated_directories/suffix.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/object.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/object.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/pdadmin.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/pdadmin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/pop.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/pop.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/process.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/replication.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/replication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/runtime/trace.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/runtime/trace.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/sso_keys.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/sso_keys.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/url_mapping.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/url_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isam/web/user_name_mapping.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isam/web/user_name_mapping.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/admin.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/advanced_tuning_parameters.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/appliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/available_updates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/available_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/config.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/config.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/date_time.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/firmware.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/fixpack.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/host_records.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/hostnames.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/hostnames.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/interfaces.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/license.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/license.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/server.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/server.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/snapshots.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/snmp_monitoring.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/statistics.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/statistics.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/support.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/alerts.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/rsyslog.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/system_alerts/snmp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isds/update_servers.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isds/update_servers.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/admin.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/admin.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/advanced_tuning_parameters.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/advanced_tuning_parameters.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/appliance.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/appliance.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/available_updates.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/available_updates.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/certstore_personal.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/certstore_personal.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/certstore_signer.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/certstore_signer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/cm/process.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/cm/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/date_time.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/date_time.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/firmware.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/firmware.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/fixpack.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/fixpack.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/host_records.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/host_records.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/hostnames.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/hostnames.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/certstore_personal.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/certstore_personal.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/certstore_signer.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/certstore_signer.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/db.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/db.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/external_library.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/external_library.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/guided_setup.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/guided_setup.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/jvm_property.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/jvm_property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/keystore.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/keystore.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/ldap.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/ldap.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/mail.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/mail.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/nls.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/nls.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/openid.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/openid.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/process.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/property.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/property.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/property_file.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/property_file.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/im/workflowextension.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/im/workflowextension.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/interfaces.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/interfaces.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/lmi.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/lmi.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/lmi_auth.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/lmi_auth.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/management_authentication.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/management_authentication.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/management_ssl_certificate.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/management_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/sdi/process.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/sdi/process.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/service_agreement.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/service_agreement.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/setup_complete.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/setup_complete.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/snapshots.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/snapshots.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/snmp_monitoring.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/snmp_monitoring.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/support.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/support.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/alerts.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/rsyslog.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/rsyslog.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/isvg/system_alerts/snmp.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/isvg/system_alerts/snmp.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/user/applianceuser.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/user/applianceuser.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/user/isdsapplianceuser.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/user/isdsapplianceuser.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity/utilities/tools.py` & `ibmsecurity-2023.6.30.0/ibmsecurity/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/PKG-INFO` & `ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmsecurity
-Version: 2023.4.26.0
+Version: 2023.6.30.0
 Summary: Idempotent functions for IBM Security Appliance REST APIs
 Home-page: 
 Author: IBM
 Author-email: IBM <secorch@us.ibm.com>
 Project-URL: Homepage, https://github.com/IBM-Security/ibmsecurity
 Project-URL: Bug Tracker, https://github.com/IBM-Security/ibmsecurity/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibmsecurity-2023.4.26.0/ibmsecurity.egg-info/SOURCES.txt` & `ibmsecurity-2023.6.30.0/ibmsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmsecurity-2023.4.26.0/pyproject.toml` & `ibmsecurity-2023.6.30.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ibmsecurity"
-version = "2023.4.26.0"
+version = "2023.6.30.0"
 authors = [
   { name="IBM", email="secorch@us.ibm.com" },
 ]
 description = "Idempotent functions for IBM Security Appliance REST APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ibmsecurity-2023.4.26.0/setup.py` & `ibmsecurity-2023.6.30.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'ibmsecurity',
     packages = find_packages(),
     # Date of release used for version - please be sure to use YYYY.MM.DD.seq#, MM and DD should be two digits e.g. 2017.02.05.0
     # seq# will be zero unless there are multiple release on a given day - then increment by one for additional release for that date
-    version = '2023.4.26.0',
+    version = '2023.6.30.0',
     description = 'Idempotent functions for IBM Security Appliance REST APIs',
     author='IBM',
     author_email='secorch@us.ibm.com',
     url='',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
```

