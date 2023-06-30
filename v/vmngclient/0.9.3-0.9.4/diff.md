# Comparing `tmp/vmngclient-0.9.3.tar.gz` & `tmp/vmngclient-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmngclient-0.9.3.tar", max compression
+gzip compressed data, was "vmngclient-0.9.4.tar", max compression
```

## Comparing `vmngclient-0.9.3.tar` & `vmngclient-0.9.4.tar`

### file list

```diff
@@ -1,107 +1,111 @@
--rw-r--r--   0        0        0     3612 2023-05-18 08:05:34.916999 vmngclient-0.9.3/README.md
--rw-r--r--   0        0        0      827 2023-05-18 08:05:34.916999 vmngclient-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2259 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/__init__.py
--rw-r--r--   0        0        0     6090 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/admin_tech_api.py
--rw-r--r--   0        0        0     8709 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/administration.py
--rw-r--r--   0        0        0     6253 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/alarms_api.py
--rw-r--r--   0        0        0     1919 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/api_containter.py
--rw-r--r--   0        0        0    11322 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/basic_api.py
--rw-r--r--   0        0        0     7051 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/dashboard_api.py
--rw-r--r--   0        0        0     6508 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/device_action_api.py
--rw-r--r--   0        0        0     1651 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/logs_api.py
--rw-r--r--   0        0        0     5971 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4040 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/omp_api.py
--rw-r--r--   0        0        0     5631 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/packet_capture_api.py
--rw-r--r--   0        0        0     4945 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/partition_manager_api.py
--rw-r--r--   0        0        0     2041 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/resource_pool_api.py
--rw-r--r--   0        0        0     7330 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/software_action_api.py
--rw-r--r--   0        0        0     5412 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/speedtest_api.py
--rw-r--r--   0        0        0     8577 2023-05-18 08:05:34.916999 vmngclient-0.9.3/vmngclient/api/task_status_api.py
--rw-r--r--   0        0        0    24704 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/template_api.py
--rw-r--r--   0        0        0     3194 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/README.md
--rw-r--r--   0        0        0     1476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/__init__.py
--rw-r--r--   0        0        0     7232 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/cli_template.py
--rw-r--r--   0        0        0     2093 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0     1306 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template.py
--rw-r--r--   0        0        0     3101 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      599 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     2430 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0     1159 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      656 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     2199 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0      476 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
--rw-r--r--   0        0        0     6752 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
--rw-r--r--   0        0        0     2465 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4529 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2123 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      627 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     2745 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
--rw-r--r--   0        0        0     8179 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
--rw-r--r--   0        0        0     9926 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
--rw-r--r--   0        0        0     7057 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1730 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     1119 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/tenant_api.py
--rw-r--r--   0        0        0     4953 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0    10808 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/api/versions_utils.py
--rw-r--r--   0        0        0    20283 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/dataclasses.py
--rw-r--r--   0        0        0     2974 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/exceptions.py
--rw-r--r--   0        0        0      672 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/logging.conf
--rw-r--r--   0        0        0     5727 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/__init__.py
--rw-r--r--   0        0        0     2299 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/client.py
--rw-r--r--   0        0        0      780 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/primitive_container.py
--rw-r--r--   0        0        0      832 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_backup_restore.py
--rw-r--r--   0        0        0     6568 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_management.py
--rw-r--r--   0        0        0      669 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/primitives/tenant_migration.py
--rw-r--r--   0        0        0     6987 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/response.py
--rw-r--r--   0        0        0    14290 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/session.py
--rw-r--r--   0        0        0     7877 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    11881 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_administration.py
--rw-r--r--   0        0        0    11034 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8053 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_cli_template.py
--rw-r--r--   0        0        0     4460 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3878 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_device_action_api.py
--rw-r--r--   0        0        0    25969 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_devices_api.py
--rw-r--r--   0        0        0      836 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1485 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_logs_api.py
--rw-r--r--   0        0        0    10911 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16398 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_omp_api.py
--rw-r--r--   0        0        0     5153 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_packet_capture.py
--rw-r--r--   0        0        0     4967 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7454 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_primitives.py
--rw-r--r--   0        0        0     5724 2023-05-18 08:05:34.920999 vmngclient-0.9.3/vmngclient/tests/test_response.py
--rw-r--r--   0        0        0     4753 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_session.py
--rw-r--r--   0        0        0     3774 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6005 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_speed_test_api.py
--rw-r--r--   0        0        0     3862 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_task_status_api.py
--rw-r--r--   0        0        0     8686 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_templates.py
--rw-r--r--   0        0        0     3625 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     8432 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_typed_list.py
--rw-r--r--   0        0        0     5170 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_version_utils.py
--rw-r--r--   0        0        0     3132 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     7341 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/typed_list.py
--rw-r--r--   0        0        0        0 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/__init__.py
--rw-r--r--   0        0        0      190 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/alarm_status.py
--rw-r--r--   0        0        0      196 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/certificate_status.py
--rw-r--r--   0        0        0       97 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/config_status.py
--rw-r--r--   0        0        0     4677 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/creation_tools.py
--rw-r--r--   0        0        0     7219 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/dashboard.py
--rw-r--r--   0        0        0     2369 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/device_model.py
--rw-r--r--   0        0        0      472 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/operation_status.py
--rw-r--r--   0        0        0      139 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/personality.py
--rw-r--r--   0        0        0      115 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/reachability.py
--rw-r--r--   0        0        0      278 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/session_type.py
--rw-r--r--   0        0        0       92 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/template_type.py
--rw-r--r--   0        0        0     1944 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/upgrades_helper.py
--rw-r--r--   0        0        0      102 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/utils/validate_status.py
--rw-r--r--   0        0        0     5302 2023-05-18 08:05:34.925000 vmngclient-0.9.3/vmngclient/vmanage_auth.py
--rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 vmngclient-0.9.3/setup.py
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 vmngclient-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     4005 2023-05-30 10:13:08.036970 vmngclient-0.9.4/README.md
+-rw-r--r--   0        0        0      827 2023-05-30 10:13:08.040970 vmngclient-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2398 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/__init__.py
+-rw-r--r--   0        0        0     6090 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/admin_tech_api.py
+-rw-r--r--   0        0        0     8709 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/administration.py
+-rw-r--r--   0        0        0     6253 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/alarms_api.py
+-rw-r--r--   0        0        0     1919 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/api_containter.py
+-rw-r--r--   0        0        0    11322 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/basic_api.py
+-rw-r--r--   0        0        0     7051 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/dashboard_api.py
+-rw-r--r--   0        0        0     6508 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/device_action_api.py
+-rw-r--r--   0        0        0     1651 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/logs_api.py
+-rw-r--r--   0        0        0     5971 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4040 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/omp_api.py
+-rw-r--r--   0        0        0     5631 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/packet_capture_api.py
+-rw-r--r--   0        0        0     4945 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/partition_manager_api.py
+-rw-r--r--   0        0        0     2041 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/resource_pool_api.py
+-rw-r--r--   0        0        0     7330 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/software_action_api.py
+-rw-r--r--   0        0        0     5412 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/speedtest_api.py
+-rw-r--r--   0        0        0     7078 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/task_status_api.py
+-rw-r--r--   0        0        0    24807 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/template_api.py
+-rw-r--r--   0        0        0     3194 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/README.md
+-rw-r--r--   0        0        0     1476 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/__init__.py
+-rw-r--r--   0        0        0     7232 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/cli_template.py
+-rw-r--r--   0        0        0     2093 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      476 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0     1306 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/feature_template.py
+-rw-r--r--   0        0        0     3101 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      599 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     2430 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0     1159 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      656 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     2044 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2199 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0      476 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
+-rw-r--r--   0        0        0     6752 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
+-rw-r--r--   0        0        0     2465 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4529 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2123 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      627 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     2745 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
+-rw-r--r--   0        0        0     8179 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
+-rw-r--r--   0        0        0     9926 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
+-rw-r--r--   0        0        0     7057 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1730 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     1119 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/tenant_api.py
+-rw-r--r--   0        0        0     4953 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0    10808 2023-05-30 10:13:08.040970 vmngclient-0.9.4/vmngclient/api/versions_utils.py
+-rw-r--r--   0        0        0    22354 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/dataclasses.py
+-rw-r--r--   0        0        0     3081 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/exceptions.py
+-rw-r--r--   0        0        0      672 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/logging.conf
+-rw-r--r--   0        0        0     5727 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/client.py
+-rw-r--r--   0        0        0     3656 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/configuration_dashboard_status.py
+-rw-r--r--   0        0        0      978 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/primitive_container.py
+-rw-r--r--   0        0        0      832 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/tenant_backup_restore.py
+-rw-r--r--   0        0        0     6568 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/tenant_management.py
+-rw-r--r--   0        0        0      669 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/primitives/tenant_migration.py
+-rw-r--r--   0        0        0     6987 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/response.py
+-rw-r--r--   0        0        0    14290 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/session.py
+-rw-r--r--   0        0        0     7877 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    11881 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_administration.py
+-rw-r--r--   0        0        0    11034 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8053 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_cli_template.py
+-rw-r--r--   0        0        0     4460 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3878 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    25969 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_devices_api.py
+-rw-r--r--   0        0        0      836 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1485 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_logs_api.py
+-rw-r--r--   0        0        0    10911 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16398 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5153 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     4967 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7454 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_primitives.py
+-rw-r--r--   0        0        0     5724 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_response.py
+-rw-r--r--   0        0        0     4753 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_session.py
+-rw-r--r--   0        0        0     3774 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6005 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0     3321 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_task_status_api.py
+-rw-r--r--   0        0        0     8686 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_templates.py
+-rw-r--r--   0        0        0     3625 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     8432 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_typed_list.py
+-rw-r--r--   0        0        0     5170 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3132 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     7341 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/typed_list.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/alarm_status.py
+-rw-r--r--   0        0        0      196 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/certificate_status.py
+-rw-r--r--   0        0        0      222 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/colors.py
+-rw-r--r--   0        0        0       97 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/config_status.py
+-rw-r--r--   0        0        0     4677 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/creation_tools.py
+-rw-r--r--   0        0        0     7219 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/dashboard.py
+-rw-r--r--   0        0        0     2369 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/device_model.py
+-rw-r--r--   0        0        0      518 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/operation_status.py
+-rw-r--r--   0        0        0      139 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/personality.py
+-rw-r--r--   0        0        0      115 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/reachability.py
+-rw-r--r--   0        0        0      278 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/session_type.py
+-rw-r--r--   0        0        0       92 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/template_type.py
+-rw-r--r--   0        0        0    19159 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/timezones_enum.py
+-rw-r--r--   0        0        0     1944 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      102 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/utils/validate_status.py
+-rw-r--r--   0        0        0     5302 2023-05-30 10:13:08.044970 vmngclient-0.9.4/vmngclient/vmanage_auth.py
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 vmngclient-0.9.4/setup.py
+-rw-r--r--   0        0        0     5191 1970-01-01 00:00:00.000000 vmngclient-0.9.4/PKG-INFO
```

### Comparing `vmngclient-0.9.3/README.md` & `vmngclient-0.9.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,38 +53,58 @@
 </details>
 
 <details>
     <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>
 
 ```python
 # Prepare devices list
-vsmarts = session.api.devices.get().filter(personality = Personality.VSMART)
+vsmarts = session.api.devices.get().filter(personality=Personality.VSMART)
 image = "viptela-20.7.2-x86_64.tar.gz"
 
 # Upload image
-session.api.repository.upload_image(software_image)
+session.api.repository.upload_image(image)
 
 # Install software
 
-install_task = session.api.software.install(devices = vsmarts,
-    image= image)
+install_task = session.api.software.install(devices=vsmarts, image=image)
 
 # Check action status
 install_task.wait_for_completed()
 ```
 
 </details>
 
 <details>
     <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>
+To get all alarms:
 
 ```python
 alarms = session.api.alarms.get()
 ```
 
+To get all not viewed alarms:
+
+```python
+not_viewed_alarms = session.api.alarms.get().filter(viewed=False)
+```
+
+To get all alarms from past `n` hours:
+
+```python
+n = 24
+alarms_from_n_hours = session.api.alarms.get(from_time=n)
+```
+
+To get all critical alarms from past `n` hours:
+
+```python
+n = 48
+critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
+```
+
 </details>
 
 <details>
     <summary> <b>User operations</b> <i>(click to expand)</i></summary>
 
 ```python
 from vmngclient.api.administration import User, UsersAPI
```

### Comparing `vmngclient-0.9.3/pyproject.toml` & `vmngclient-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vmngclient"
-version = "0.9.3"
+version = "0.9.4"
 description = "Universal vManage API"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/CiscoDevNet/vManage-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `vmngclient-0.9.3/vmngclient/__init__.py` & `vmngclient-0.9.4/vmngclient/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 import multiprocessing
 from functools import lru_cache, wraps
 from importlib import metadata
 from importlib.machinery import PathFinder
 from os import environ
 from pathlib import Path
 from traceback import FrameSummary, StackSummary, extract_stack
-from typing import Callable, Final, List
+from typing import Callable, Final, List, Optional
 
 import urllib3
 
 
 def with_proc_info_header(method: Callable[..., str]) -> Callable[..., str]:
     """
     Adds process ID and external caller information before first line of returned string
     """
 
     @wraps(method)
     def wrapper(*args, **kwargs) -> str:
         wrapped = method(*args, **kwargs)
-        fname, line_no, function, _ = get_first_external_stack_frame(extract_stack())
-        external_caller_info = "%s:%d %s(...)" % (fname, line_no, function)
-        header = f"{multiprocessing.current_process()} {external_caller_info}\n"
+        header = f"{multiprocessing.current_process()}"
+        if frame_summary := get_first_external_stack_frame(extract_stack()):
+            fname, line_no, function, _ = frame_summary
+            header += " %s:%d %s(...)" % (fname, line_no, function)
+        header += "\n"
         return header + wrapped
 
     return wrapper
 
 
-def get_first_external_stack_frame(stack: StackSummary) -> FrameSummary:
+def get_first_external_stack_frame(stack: StackSummary) -> Optional[FrameSummary]:
     """
     Get the first python frame
     on the stack before entering vmngclient module
     """
+    if len(stack) < 1:
+        return None
     for index, frame in enumerate(stack):
         if is_file_in_package(frame.filename):
             break
+    if index == 0:
+        return None
     return stack[index - 1]
 
 
 @lru_cache()
 def is_file_in_package(fname: str) -> bool:
     """
     Checks if filepath given by string
```

### Comparing `vmngclient-0.9.3/vmngclient/api/admin_tech_api.py` & `vmngclient-0.9.4/vmngclient/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/administration.py` & `vmngclient-0.9.4/vmngclient/api/administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/alarms_api.py` & `vmngclient-0.9.4/vmngclient/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/api_containter.py` & `vmngclient-0.9.4/vmngclient/api/api_containter.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/basic_api.py` & `vmngclient-0.9.4/vmngclient/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/dashboard_api.py` & `vmngclient-0.9.4/vmngclient/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/device_action_api.py` & `vmngclient-0.9.4/vmngclient/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/logs_api.py` & `vmngclient-0.9.4/vmngclient/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/mtt_aaa_api.py` & `vmngclient-0.9.4/vmngclient/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/omp_api.py` & `vmngclient-0.9.4/vmngclient/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/packet_capture_api.py` & `vmngclient-0.9.4/vmngclient/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/partition_manager_api.py` & `vmngclient-0.9.4/vmngclient/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/resource_pool_api.py` & `vmngclient-0.9.4/vmngclient/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/software_action_api.py` & `vmngclient-0.9.4/vmngclient/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/speedtest_api.py` & `vmngclient-0.9.4/vmngclient/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/task_status_api.py` & `vmngclient-0.9.4/vmngclient/api/task_status_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,47 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, List, Optional, cast
+from typing import TYPE_CHECKING, List, cast
 
 from tenacity import retry, retry_if_result, stop_after_attempt, wait_fixed  # type: ignore
 
+from vmngclient.exceptions import TaskValidationError
+
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
-from pydantic import BaseModel, Field
-
+from vmngclient.primitives.configuration_dashboard_status import (
+    ConfigurationDashboardStatusPrimitives,
+    SubTaskData,
+    TaskData,
+    TaskResult,
+)
 from vmngclient.utils.operation_status import OperationStatus, OperationStatusId
 
 logger = logging.getLogger(__name__)
 
 
-class SubTaskData(BaseModel):
-    status: str
-    status_id: str = Field(alias="statusId")
-    action: str
-    activity: List[str]
-    current_activity: str = Field(alias="currentActivity")
-    action_config: Optional[str] = Field(alias="actionConfig")
-    order: Optional[int]
-    uuid: Optional[str]
-    hostname: Optional[str] = Field(alias="host-name")
-    site_id: Optional[str] = Field(alias="site-id")
-
-
-class TaskResult(BaseModel):
-    result: bool
-    sub_tasks_data: List[SubTaskData]
-
-
-class RunningTaskData(BaseModel):
-    details_url: str = Field(alias="detailsURL")
-    user_session_username: str = Field(alias="userSessionUserName")
-    rid: int = Field(alias="@rid")
-    tenant_name: str = Field("tenantName")
-    process_id: str = Field(alias="processId")
-    name: str
-    tenant_id: str = Field(alias="tenantId")
-    user_session_ip: str = Field(alias="userSessionIP")
-    action: str
-    start_time: int = Field(alias="startTime")
-    end_time: int = Field(alias="endTime")
-    status: str
-
-
-class TasksData(BaseModel):
-    running_tasks: List[RunningTaskData] = Field(alias="runningTasks")
-
-
-class TasksAPI:
-    """
-    API class for getting data about tasks
-    """
-
-    def __init__(self, session: vManageSession, task_id: str):
-        self.session = session
-        self.task_id = task_id
-        self.url = f"/dataservice/device/action/status/{self.task_id}"
-
-    def get_all_tasks(self) -> TasksData:
-        """
-        Get list of active tasks id's in vmanage
-
-        Args:
-            session (vManageSession): session
-
-        Returns:
-        TasksData: Data about all tasks in vmanage
-        """
-        url = "dataservice/device/action/status/tasks"
-        json = self.session.get_json(url)
-        return TasksData.parse_obj(json)
-
-    def get_task_data(self) -> List[SubTaskData]:
-        """
-        Get data about all sub-tasks in task
-
-        Args:
-            delay_seconds (int, optional): If vmanage doesn't get data about task, after this time will asks again.
-            Defaults to 5.
-
-        Returns:
-            List[SubTaskData]: List of all sub-tusks
-        """
-        task_data = self.session.get_data(self.url)
-        return [SubTaskData.parse_obj(subtask_data) for subtask_data in task_data]
-
-
 class Task:
     """
     API class for getting data about task/sub-tasks
     """
 
     def __init__(self, session: vManageSession, task_id: str):
         self.session = session
         self.task_id = task_id
         self.url = f"/dataservice/device/action/status/{self.task_id}"
         self.task_data: List[SubTaskData]
 
+    def __check_validation_status(self, task: TaskData):
+        if not task.validation:
+            return None
+        if task.validation.status in (OperationStatus.FAILURE, OperationStatus.VALIDATION_FAILURE):
+            raise TaskValidationError(f"Task status validation failed, validation status is:{task.validation.status}")
+
     def wait_for_completed(
         self,
         timeout_seconds: int = 300,
         interval_seconds: int = 5,
         success_statuses: List[OperationStatus] = [
             OperationStatus.SUCCESS,
         ],
@@ -141,14 +77,15 @@
                 #do something else
 
         Args:
 
 
             timeout_seconds (int): After this time, function will stop requesting action status
             interval_seconds (int): interval between action status requests
+            validation_timeout_seconds (int): After this time, task validation call will be send
             delay_seconds (int): if Vmanage didn't report task status, after this time api call would be repeated
             success_statuses (Union[List[OperationStatus], str]): list of positive sub-tasks statuses
             success_statuses_ids (Union[List[OperationStatus], str]): list of positive sub-tasks statuses id's
             fails_statuses_id (Union[List[OperationStatusId], str]): list of negative sub-tasks statuses
             fails_statuses_ids (Union[List[OperationStatusId], str]): list of negative sub-tasks statuses id's
             activity_text (str): activity text
 
@@ -173,15 +110,16 @@
 
             Args:
                 task_data (List[SubTaskData]): list of all sub_tasks
 
             Returns:
                 bool: False if condition is met
             """
-
+            if not task_data:
+                return True
             task_statuses_success = [task.status in success_statuses for task in task_data]
             task_statuses_failure = [task.status in failure_statuses for task in task_data]
             task_statuses_id_success = [task.status_id in success_statuses_ids for task in task_data]
             task_statuses_id_failure = [task.status_id in failure_statuses_ids for task in task_data]
             task_activities = [activity_text in task.activity for task in task_data]
 
             if all(task_statuses_success + task_statuses_id_success) or any(
@@ -204,16 +142,17 @@
             """
             Keep asking for task status, status_id,
             activity(optional), untill check_status is True
 
             Returns:
                 List[SubTaskData]
             """
-
-            self.task_data = TasksAPI(self.session, self.task_id).get_task_data()
+            task = ConfigurationDashboardStatusPrimitives(self.session).find_status(self.task_id)
+            self.__check_validation_status(task)
+            self.task_data = task.data
             sub_task_statuses = [task.status for task in self.task_data]
             sub_task_statuses_id = [task.status_id for task in self.task_data]
             sub_task_activities = [task.activity for task in self.task_data]
             logger.info(
                 f"Sub-tasks data for task {self.task_id}: \n "
                 f"statuses: {sub_task_statuses}, status_ids: {sub_task_statuses_id}, activities: {sub_task_activities}."
             )
```

### Comparing `vmngclient-0.9.3/vmngclient/api/template_api.py` & `vmngclient-0.9.4/vmngclient/api/template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.api.templates.feature_template_field import FeatureTemplateField, get_path_dict
 from vmngclient.api.templates.feature_template_payload import FeatureTemplatePayload
 from vmngclient.api.templates.models.cisco_aaa_model import CiscoAAAModel
 from vmngclient.api.templates.models.omp_vsmart_model import OMPvSmart
 from vmngclient.api.templates.models.security_vsmart_model import SecurityvSmart
+from vmngclient.api.templates.models.system_vsmart_model import SystemVsmart
 from vmngclient.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, FeatureTemplatesTypes, TemplateInfo
 from vmngclient.exceptions import AlreadyExistsError, AttachedError, TemplateNotFoundError
 from vmngclient.response import vManageResponse
 from vmngclient.typed_list import DataSequence
 from vmngclient.utils.device_model import DeviceModel
 from vmngclient.utils.template_type import TemplateType
 
@@ -458,14 +459,15 @@
 
         Method will be deleted if every template's payload will be generated dynamically.
         """
         ported_templates = (
             CiscoAAAModel,
             OMPvSmart,
             SecurityvSmart,
+            SystemVsmart,
         )
 
         return isinstance(template, ported_templates)
 
     def get_feature_template_schema(self, template: FeatureTemplate, debug: bool = False) -> Any:
         endpoint = f"/dataservice/template/feature/types/definition/{template.type}/15.0.0"
         schema = self.session.get(url=endpoint).json()
```

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/README.md` & `vmngclient-0.9.4/vmngclient/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/__init__.py` & `vmngclient-0.9.4/vmngclient/api/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/cli_template.py` & `vmngclient-0.9.4/vmngclient/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/device_template/device_template.py` & `vmngclient-0.9.4/vmngclient/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/feature_template.py` & `vmngclient-0.9.4/vmngclient/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/feature_template_field.py` & `vmngclient-0.9.4/vmngclient/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/feature_template_payload.py` & `vmngclient-0.9.4/vmngclient/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/models/cisco_aaa_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/models/omp_vsmart_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/models/security_vsmart_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/aaa_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/aaa/feature/user.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant.json.j2` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/templates/payloads/tenant/tenant_model.py` & `vmngclient-0.9.4/vmngclient/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/tenant_api.py` & `vmngclient-0.9.4/vmngclient/api/tenant_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/tenant_backup_restore_api.py` & `vmngclient-0.9.4/vmngclient/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/api/versions_utils.py` & `vmngclient-0.9.4/vmngclient/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/dataclasses.py` & `vmngclient-0.9.4/vmngclient/dataclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from attr import define, field  # type: ignore
 from pydantic import BaseModel, Field
 
 from vmngclient.exceptions import RetrieveIntervalOutOfRange
 from vmngclient.utils.alarm_status import Severity
 from vmngclient.utils.certificate_status import ValidityPeriod
+from vmngclient.utils.colors import PrintColors
 from vmngclient.utils.creation_tools import FIELD_NAME, asdict, convert_attributes
 from vmngclient.utils.personality import Personality
 from vmngclient.utils.reachability import Reachability
 from vmngclient.utils.template_type import TemplateType
 
 
 class DataclassBase:
@@ -41,25 +42,40 @@
     size: int
     state: str
     token_id: Optional[str] = field(default=None, metadata={FIELD_NAME: "requestTokenId"})
 
 
 @define(frozen=True, field_transformer=convert_attributes)
 class AlarmData(DataclassBase):
+    severity: Severity = field(converter=Severity, default=None)
     component: Optional[str] = field(default=None)
     active: Optional[bool] = field(default=None)
-    severity: Optional[Severity] = field(converter=Severity, default=None)
+    severity_number: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None, metadata={FIELD_NAME: "type"})
     system_ip: Optional[str] = field(default=None, metadata={FIELD_NAME: "system-ip"})
     hostname: Optional[str] = field(default=None, metadata={FIELD_NAME: "host-name"})
     site_id: Optional[str] = field(default=None, metadata={FIELD_NAME: "site-id"})
     new_state: Optional[str] = field(default=None, metadata={FIELD_NAME: "new-state"})
     interface_name: Optional[str] = field(default=None, metadata={FIELD_NAME: "if-name"})
     vpn_id: Optional[str] = field(default=None, metadata={FIELD_NAME: "vpn-id"})
     viewed: Optional[bool] = field(default=None, metadata={FIELD_NAME: "acknowledged"})
+    message: Optional[str] = field(default=None)
+    values: Optional[list] = field(default=None)
+    values_short_display: Optional[list] = field(default=None)
+    event_name: Optional[str] = field(default=None, metadata={FIELD_NAME: "eventname"})
+    rule_name: Optional[str] = field(default=None, metadata={FIELD_NAME: "rulename"})
+    entry_time: Optional[int] = field(default=None)
+    receive_time: Optional[int] = field(default=None)
+    rule_name_display: Optional[str] = field(default=None)
+    uuid: Optional[str] = field(default=None)
+    possible_causes: Optional[List[str]] = field(default=None)
+    consumed_events: Optional[list] = field(default=None)
+    devices: Optional[list] = field(default=None)
+    tenant: Optional[str] = field(default=None)
+    id: Optional[str] = field(default=None)
 
     def issubset(self, other: "AlarmData") -> bool:
         field_keys = {field_key for field_key in self.__annotations__ if getattr(self, field_key)}
         return all(getattr(self, field_key) == getattr(other, field_key) for field_key in field_keys)
 
     def lowercase(self) -> "AlarmData":
         data = dict()
@@ -68,14 +84,42 @@
             try:
                 data[field_key] = attr.lower()
             except AttributeError:
                 data[field_key] = attr
 
         return AlarmData(**data)
 
+    def alarm_severity_print(self) -> str:
+        color = {
+            Severity.CRITICAL: PrintColors.RED,
+            Severity.MAJOR: PrintColors.YELLOW,
+            Severity.MEDIUM: PrintColors.BLUE,
+            Severity.MINOR: PrintColors.GREEN,
+            Severity.UNKNOWN: PrintColors.NONE,
+        }
+
+        return f"{color[self.severity].value}{self.severity}{PrintColors.NONE.value}"
+
+    def format_datetime(self, time: int) -> str:
+        if time is None:
+            return "N/A"
+        return dt.datetime.fromtimestamp(time / 1e3).strftime("%H:%M:%S %Y-%m-%d")
+
+    def __str__(self):
+        result = (
+            f"{self.__class__.__name__}:\n    "
+            f"{self.message}\n    "
+            f"{self.alarm_severity_print()}\n    "
+            f"Alarm received at {self.format_datetime(self.receive_time)} "
+            f"(entry time: {self.format_datetime(self.entry_time)}).\n    "
+            f"Device {self.hostname} (system ip: {self.system_ip}).\n    "
+            f"Alarm type: {self.name}."
+        )
+        return result
+
 
 @define
 class Device(DataclassBase):
     uuid: str
     personality: Personality = field(converter=Personality)
     id: str = field(metadata={FIELD_NAME: "deviceId"})
     hostname: str = field(metadata={FIELD_NAME: "host-name"})
@@ -228,14 +272,15 @@
 
 
 @define
 class FeatureTemplateInfo(TemplateInfo):
     template_type: str = field(metadata={FIELD_NAME: "templateType"})
     device_type: List[str] = field(metadata={FIELD_NAME: "deviceType"})
     version: str = field(metadata={FIELD_NAME: "templateMinVersion"})
+    resource_group: Optional[str] = field(default="", metadata={FIELD_NAME: "resourceGroup"})  # type: ignore
 
 
 @define
 class DeviceTemplateInfo(TemplateInfo):
     device_type: str = field(metadata={FIELD_NAME: "deviceType"})
     template_class: str = field(metadata={FIELD_NAME: "templateClass"})
     config_type: TemplateType = field(converter=TemplateType, metadata={FIELD_NAME: "configType"})
@@ -399,15 +444,15 @@
         if not RETRIEVE_INTERVAL_MIN <= int(value) <= RETRIEVE_INTERVAL_MAX:
             raise RetrieveIntervalOutOfRange("Retrieve interval must be value between 1 and 60 minutes")
 
 
 @define
 class Vbond(DataclassBase):
     vbond_address: str = field(metadata={FIELD_NAME: "domainIp"})
-    vbond_port: int = field(metadata={FIELD_NAME: "port"})
+    vbond_port: str = field(metadata={FIELD_NAME: "port"})
 
 
 @define(frozen=True)
 class TenantAAA(DataclassBase):
     """
     Provider-Tenant -> Tenant -> Administration -> Manage users -> Remote AAA
     """
```

### Comparing `vmngclient-0.9.3/vmngclient/exceptions.py` & `vmngclient-0.9.4/vmngclient/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,20 @@
 
 class TaskNotRegisteredError(vManageClientError):
     """Raised if task_id is generated, but it's not registere in vManage"""
 
     pass
 
 
+class TaskValidationError(vManageClientError):
+    """Raised if task has not been validated"""
+
+    pass
+
+
 class MultiplePersonalityError(vManageClientError):
     """Raised if Device DataSequnce contains devices with multiples personalities"""
 
 
 class SessionNotCreatedError(vManageClientError):
     """Raised when vManage session cannot be created"""
```

### Comparing `vmngclient-0.9.3/vmngclient/logging.conf` & `vmngclient-0.9.4/vmngclient/logging.conf`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/primitives/__init__.py` & `vmngclient-0.9.4/vmngclient/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/primitives/client.py` & `vmngclient-0.9.4/vmngclient/primitives/client.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/primitives/tenant_backup_restore.py` & `vmngclient-0.9.4/vmngclient/primitives/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/primitives/tenant_management.py` & `vmngclient-0.9.4/vmngclient/primitives/tenant_management.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/primitives/tenant_migration.py` & `vmngclient-0.9.4/vmngclient/primitives/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/response.py` & `vmngclient-0.9.4/vmngclient/response.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/session.py` & `vmngclient-0.9.4/vmngclient/session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_admin_tech_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_administration.py` & `vmngclient-0.9.4/vmngclient/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_alarms_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_cli_template.py` & `vmngclient-0.9.4/vmngclient/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_creation_tools.py` & `vmngclient-0.9.4/vmngclient/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_device_action_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_devices_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_feature_template_field.py` & `vmngclient-0.9.4/vmngclient/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_logs_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_mtt_aaa_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_omp_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_packet_capture.py` & `vmngclient-0.9.4/vmngclient/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_partition_manager_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_primitives.py` & `vmngclient-0.9.4/vmngclient/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_response.py` & `vmngclient-0.9.4/vmngclient/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_session.py` & `vmngclient-0.9.4/vmngclient/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_software_action_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_speed_test_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_templates.py` & `vmngclient-0.9.4/vmngclient/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_tenant_backup_restore_api.py` & `vmngclient-0.9.4/vmngclient/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_typed_list.py` & `vmngclient-0.9.4/vmngclient/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_version_utils.py` & `vmngclient-0.9.4/vmngclient/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/tests/test_vmanage_auth.py` & `vmngclient-0.9.4/vmngclient/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/typed_list.py` & `vmngclient-0.9.4/vmngclient/typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/utils/creation_tools.py` & `vmngclient-0.9.4/vmngclient/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/utils/dashboard.py` & `vmngclient-0.9.4/vmngclient/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/utils/device_model.py` & `vmngclient-0.9.4/vmngclient/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/utils/upgrades_helper.py` & `vmngclient-0.9.4/vmngclient/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/vmngclient/vmanage_auth.py` & `vmngclient-0.9.4/vmngclient/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.9.3/setup.py` & `vmngclient-0.9.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,17 +37,17 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'vmngclient',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Universal vManage API',
-    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality = Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices = vsmarts,\n    image= image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>User operations</b> <i>(click to expand)</i></summary>\n\n```python\nfrom vmngclient.api.administration import User, UsersAPI\n\n# Get all users\nall_users = UsersAPI(session).get_all_users()\n\n# Create a user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nstatus = UsersAPI(session).create_user(new_user)\n\n# Delete a user\nstatus = UsersAPI(session).delete_user(username="new_user")\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n\tsession.api.users.delete_user("XYZ")\nexcept vManageBadRequestError as error:\n\t# Process an error.\n\tlogger.error(error.info.details)\n\n# message = \'Delete users request failed\' \n# details = \'No user with name XYZ was found\' \n# code = \'USER0006\'\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
+    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>User operations</b> <i>(click to expand)</i></summary>\n\n```python\nfrom vmngclient.api.administration import User, UsersAPI\n\n# Get all users\nall_users = UsersAPI(session).get_all_users()\n\n# Create a user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nstatus = UsersAPI(session).create_user(new_user)\n\n# Delete a user\nstatus = UsersAPI(session).delete_user(username="new_user")\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n\tsession.api.users.delete_user("XYZ")\nexcept vManageBadRequestError as error:\n\t# Process an error.\n\tlogger.error(error.info.details)\n\n# message = \'Delete users request failed\' \n# details = \'No user with name XYZ was found\' \n# code = \'USER0006\'\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CiscoDevNet/vManage-client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vmngclient-0.9.3/PKG-INFO` & `vmngclient-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmngclient
-Version: 0.9.3
+Version: 0.9.4
 Summary: Universal vManage API
 Home-page: https://github.com/CiscoDevNet/vManage-client
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -83,38 +83,58 @@
 </details>
 
 <details>
     <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>
 
 ```python
 # Prepare devices list
-vsmarts = session.api.devices.get().filter(personality = Personality.VSMART)
+vsmarts = session.api.devices.get().filter(personality=Personality.VSMART)
 image = "viptela-20.7.2-x86_64.tar.gz"
 
 # Upload image
-session.api.repository.upload_image(software_image)
+session.api.repository.upload_image(image)
 
 # Install software
 
-install_task = session.api.software.install(devices = vsmarts,
-    image= image)
+install_task = session.api.software.install(devices=vsmarts, image=image)
 
 # Check action status
 install_task.wait_for_completed()
 ```
 
 </details>
 
 <details>
     <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>
+To get all alarms:
 
 ```python
 alarms = session.api.alarms.get()
 ```
 
+To get all not viewed alarms:
+
+```python
+not_viewed_alarms = session.api.alarms.get().filter(viewed=False)
+```
+
+To get all alarms from past `n` hours:
+
+```python
+n = 24
+alarms_from_n_hours = session.api.alarms.get(from_time=n)
+```
+
+To get all critical alarms from past `n` hours:
+
+```python
+n = 48
+critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
+```
+
 </details>
 
 <details>
     <summary> <b>User operations</b> <i>(click to expand)</i></summary>
 
 ```python
 from vmngclient.api.administration import User, UsersAPI
```

