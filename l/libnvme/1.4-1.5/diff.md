# Comparing `tmp/libnvme-1.4.tar.gz` & `tmp/libnvme-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libnvme-1.4.tar", last modified: Fri Mar 31 14:06:35 2023, max compression
+gzip compressed data, was "libnvme-1.5.tar", last modified: Fri Jun 30 13:18:16 2023, max compression
```

## Comparing `libnvme-1.4.tar` & `libnvme-1.5.tar`

### file list

```diff
@@ -1,924 +1,994 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:24.944925 libnvme-1.4/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/.github/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/
--rw-rw-r--   0 runner    (1001) docker     (123)       80 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/clang.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      452 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/ubuntu-armhf.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      465 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/ubuntu-ppc64le.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/ubuntu-s390x.txt
--rw-rw-r--   0 runner    (1001) docker     (123)       81 2023-03-31 14:05:19.000000 libnvme-1.4/.github/cross/ubuntu-static.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      122 2023-03-31 14:05:19.000000 libnvme-1.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (123)    11439 2023-03-31 14:05:19.000000 libnvme-1.4/.github/workflows/build.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     1043 2023-03-31 14:05:19.000000 libnvme-1.4/.github/workflows/coverage.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     1721 2023-03-31 14:05:19.000000 libnvme-1.4/.github/workflows/release-python.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      350 2023-03-31 14:05:19.000000 libnvme-1.4/.github/workflows/release.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      130 2023-03-31 14:05:19.000000 libnvme-1.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-03-31 14:05:19.000000 libnvme-1.4/.readthedocs.yaml
--rw-rw-r--   0 runner    (1001) docker     (123)    26530 2023-03-31 14:05:19.000000 libnvme-1.4/COPYING
--rw-rw-r--   0 runner    (1001) docker     (123)     1006 2023-03-31 14:05:19.000000 libnvme-1.4/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)     5830 2023-03-31 14:05:19.000000 libnvme-1.4/README.md
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/array_size/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.440873 libnvme-1.4/ccan/ccan/array_size/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1032 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/array_size/_info
--rw-rw-r--   0 runner    (1001) docker     (123)      889 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/array_size/array_size.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/build_assert/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.440873 libnvme-1.4/ccan/ccan/build_assert/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1350 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/build_assert/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     1228 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/build_assert/build_assert.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/check_type/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.440873 libnvme-1.4/ccan/ccan/check_type/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)      841 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/check_type/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     2368 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/check_type/check_type.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/container_of/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.440873 libnvme-1.4/ccan/ccan/container_of/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1386 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/container_of/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     4278 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/container_of/container_of.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/endian/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.440873 libnvme-1.4/ccan/ccan/endian/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1419 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/endian/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     9656 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/endian/endian.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/list/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.444873 libnvme-1.4/ccan/ccan/list/LICENSE -> ../../licenses/BSD-MIT
--rw-rw-r--   0 runner    (1001) docker     (123)     1519 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/list/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     1000 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/list/list.c
--rw-rw-r--   0 runner    (1001) docker     (123)    24307 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/list/list.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/minmax/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.444873 libnvme-1.4/ccan/ccan/minmax/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1141 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/minmax/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     1266 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/minmax/minmax.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/short_types/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.444873 libnvme-1.4/ccan/ccan/short_types/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)      793 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/short_types/short_types.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/
-lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-31 14:06:35.444873 libnvme-1.4/ccan/ccan/str/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)     1355 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/_info
--rw-rw-r--   0 runner    (1001) docker     (123)     1602 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/debug.c
--rw-rw-r--   0 runner    (1001) docker     (123)      283 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/str.c
--rw-rw-r--   0 runner    (1001) docker     (123)     5958 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/str.h
--rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/ccan/str/str_debug.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/licenses/
--rw-rw-r--   0 runner    (1001) docker     (123)     1023 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/licenses/BSD-MIT
--rw-rw-r--   0 runner    (1001) docker     (123)     6383 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/licenses/CC0
--rw-rw-r--   0 runner    (1001) docker     (123)      603 2023-03-31 14:05:19.000000 libnvme-1.4/ccan/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/doc/
--rw-rw-r--   0 runner    (1001) docker     (123)      390 2023-03-31 14:05:19.000000 libnvme-1.4/doc/api.rst.in
--rw-rw-r--   0 runner    (1001) docker     (123)     1054 2023-03-31 14:05:19.000000 libnvme-1.4/doc/conf.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1060 2023-03-31 14:05:19.000000 libnvme-1.4/doc/conf.py.in
--rw-rw-r--   0 runner    (1001) docker     (123)     4123 2023-03-31 14:05:19.000000 libnvme-1.4/doc/config-schema.json
--rw-rw-r--   0 runner    (1001) docker     (123)     4123 2023-03-31 14:05:19.000000 libnvme-1.4/doc/config-schema.json.in
--rw-rw-r--   0 runner    (1001) docker     (123)      570 2023-03-31 14:05:19.000000 libnvme-1.4/doc/index.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      570 2023-03-31 14:05:19.000000 libnvme-1.4/doc/index.rst.in
--rw-rw-r--   0 runner    (1001) docker     (123)      965 2023-03-31 14:05:19.000000 libnvme-1.4/doc/installation.rst.in
--rwxrwxr-x   0 runner    (1001) docker     (123)    70557 2023-03-31 14:05:19.000000 libnvme-1.4/doc/kernel-doc
--rw-rw-r--   0 runner    (1001) docker     (123)      264 2023-03-31 14:05:19.000000 libnvme-1.4/doc/kernel-doc-check
--rwxrwxr-x   0 runner    (1001) docker     (123)      354 2023-03-31 14:05:19.000000 libnvme-1.4/doc/list-man-pages.sh
--rwxrwxr-x   0 runner    (1001) docker     (123)       47 2023-03-31 14:05:19.000000 libnvme-1.4/doc/list-pre-compiled.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/
--rw-rw-r--   0 runner    (1001) docker     (123)     3523 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_admin_opcode.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1889 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_admin_passthru.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1907 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_admin_passthru64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      655 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ae_info_css_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      954 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ae_info_error.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1141 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ae_info_notice.2
--rw-rw-r--   0 runner    (1001) docker     (123)      585 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ae_info_smart.2
--rw-rw-r--   0 runner    (1001) docker     (123)      565 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ae_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      409 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_aggregate_endurance_group_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      417 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_aggregate_predictable_lat_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      577 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ana_group_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      473 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ana_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      733 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ana_state.2
--rw-rw-r--   0 runner    (1001) docker     (123)      655 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_apst_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      573 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_boot_partition.2
--rw-rw-r--   0 runner    (1001) docker     (123)      701 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_capacity_config_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      454 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_capacity_mgmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1068 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_change_ns_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      539 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_channel_config_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      345 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmb_size.2
--rw-rw-r--   0 runner    (1001) docker     (123)      904 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      416 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_effects_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      510 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_format_mset.2
--rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_format_pi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      493 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_format_pil.2
--rw-rw-r--   0 runner    (1001) docker     (123)      955 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_format_ses.2
--rw-rw-r--   0 runner    (1001) docker     (123)     3374 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_get_log_lid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_cmd_get_log_telemetry_host_lsp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      416 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_compare.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2027 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_connect_err.2
--rw-rw-r--   0 runner    (1001) docker     (123)     4037 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_constants.2
--rw-rw-r--   0 runner    (1001) docker     (123)      385 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_copy.2
--rw-rw-r--   0 runner    (1001) docker     (123)      746 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_copy_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      756 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_copy_range_f1.2
--rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_create_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      385 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_create_root.2
--rw-rw-r--   0 runner    (1001) docker     (123)      403 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      329 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_first_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      336 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_first_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      296 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_for_each_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_for_each_ns_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      301 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_for_each_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      401 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_for_each_path_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      384 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_address.2
--rw-rw-r--   0 runner    (1001) docker     (123)      350 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      361 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_dhchap_host_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      371 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_dhchap_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      315 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_fd.2
--rw-rw-r--   0 runner    (1001) docker     (123)      330 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_firmware.2
--rw-rw-r--   0 runner    (1001) docker     (123)      359 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_host_iface.2
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_host_traddr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      305 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_model.2
--rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_name.2
--rw-rw-r--   0 runner    (1001) docker     (123)      333 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_numa_node.2
--rw-rw-r--   0 runner    (1001) docker     (123)      334 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_queue_count.2
--rw-rw-r--   0 runner    (1001) docker     (123)      325 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_serial.2
--rw-rw-r--   0 runner    (1001) docker     (123)      318 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_sqsize.2
--rw-rw-r--   0 runner    (1001) docker     (123)      337 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_state.2
--rw-rw-r--   0 runner    (1001) docker     (123)      330 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_subsysnqn.2
--rw-rw-r--   0 runner    (1001) docker     (123)      343 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      339 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_sysfs_dir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      326 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_traddr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      332 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_transport.2
--rw-rw-r--   0 runner    (1001) docker     (123)      365 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_get_trsvcid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      504 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_identify.2
--rw-rw-r--   0 runner    (1001) docker     (123)      352 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_is_discovered.2
--rw-rw-r--   0 runner    (1001) docker     (123)      486 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_is_discovery_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      352 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_is_persistent.2
--rw-rw-r--   0 runner    (1001) docker     (123)      397 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_is_unique_discovery_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2393 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_metadata_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      380 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_next_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_next_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      411 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_reset.2
--rw-rw-r--   0 runner    (1001) docker     (123)      403 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_dhchap_host_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      395 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_dhchap_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      437 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_discovered.2
--rw-rw-r--   0 runner    (1001) docker     (123)      511 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_discovery_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      438 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_persistent.2
--rw-rw-r--   0 runner    (1001) docker     (123)      546 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ctrls_filter.2
--rw-rw-r--   0 runner    (1001) docker     (123)      589 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_data_tfr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_default_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      512 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_describe_key_serial.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1035 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dev_self_test.2
--rw-rw-r--   0 runner    (1001) docker     (123)      407 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_dtype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      702 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_receive_doper.2
--rw-rw-r--   0 runner    (1001) docker     (123)      464 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_recv.2
--rw-rw-r--   0 runner    (1001) docker     (123)      624 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_recv_identify_parameters.2
--rw-rw-r--   0 runner    (1001) docker     (123)      662 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_recv_stream_allocate.2
--rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_recv_stream_parameters.2
--rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_recv_stream_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      730 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send.2
--rw-rw-r--   0 runner    (1001) docker     (123)      596 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send_doper.2
--rw-rw-r--   0 runner    (1001) docker     (123)      722 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send_id_endir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      455 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send_identify_endir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      622 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send_stream_release_identifier.2
--rw-rw-r--   0 runner    (1001) docker     (123)      559 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_send_stream_release_resource.2
--rw-rw-r--   0 runner    (1001) docker     (123)      505 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_directive_types.2
--rw-rw-r--   0 runner    (1001) docker     (123)      374 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_disconnect_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dsm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      476 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dsm_attributes.2
--rw-rw-r--   0 runner    (1001) docker     (123)      391 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dsm_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      621 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dst_stc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dump_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      360 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_dump_tree.2
--rw-rw-r--   0 runner    (1001) docker     (123)      713 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_eg_critical_warning_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      387 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_eg_event_aggregate_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      474 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_end_grp_chan_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      872 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_end_grp_config_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1471 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_endurance_group_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_errno_to_string.2
--rw-rw-r--   0 runner    (1001) docker     (123)     3984 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_error_log_page.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1894 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fabrics_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      781 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fctype.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1030 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_config_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      946 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_config_fdpa.2
--rw-rw-r--   0 runner    (1001) docker     (123)      645 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_config_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      878 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      469 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_event_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      586 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_event_realloc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      334 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_event_realloc_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_event_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      423 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_events_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      650 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_reclaim_unit_handle_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      679 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_reclaim_unit_handle_update.2
--rw-rw-r--   0 runner    (1001) docker     (123)      330 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruh_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      472 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruh_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      600 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruh_status_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      421 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruh_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruha.2
--rw-rw-r--   0 runner    (1001) docker     (123)      372 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruhu_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_ruhu_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_stats_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      481 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_supported_event_attributes.2
--rw-rw-r--   0 runner    (1001) docker     (123)      415 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fdp_supported_event_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     8677 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat.2
--rw-rw-r--   0 runner    (1001) docker     (123)      307 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_auto_pst.2
--rw-rw-r--   0 runner    (1001) docker     (123)      422 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_fdp_events_cdw11.2
--rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_host_behavior.2
--rw-rw-r--   0 runner    (1001) docker     (123)      686 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_nswpcfg_state.2
--rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_plm_window_select.2
--rw-rw-r--   0 runner    (1001) docker     (123)      610 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_resv_notify_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      498 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_feat_tmpthresh_thsel.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1855 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_features_async_event_config_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)     3957 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_features_id.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1944 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fid_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fid_supported_effects_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      451 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_firmware_slot.2
--rw-rw-r--   0 runner    (1001) docker     (123)      313 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_first_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      348 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_first_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      531 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_flush.2
--rw-rw-r--   0 runner    (1001) docker     (123)      290 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_for_each_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      372 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_for_each_host_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      316 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_for_each_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      403 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_for_each_subsystem_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      734 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_format_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_format_nvm_compln_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      496 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_format_nvm_start_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      240 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_free_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      241 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_free_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      237 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_free_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      313 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_free_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      316 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_free_tree.2
--rw-rw-r--   0 runner    (1001) docker     (123)      645 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fw_commit.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1622 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fw_commit_ca.2
--rw-rw-r--   0 runner    (1001) docker     (123)      811 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fw_commit_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1100 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fw_download.2
--rw-rw-r--   0 runner    (1001) docker     (123)      763 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_fw_download_seq.2
--rw-rw-r--   0 runner    (1001) docker     (123)      657 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_gen_dhchap_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      508 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_ana_log_len.2
--rw-rw-r--   0 runner    (1001) docker     (123)      442 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_ctrl_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      934 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_ctrl_telemetry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      729 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_directive_receive_length.2
--rw-rw-r--   0 runner    (1001) docker     (123)      742 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_discovery_args.2
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_feature_length.2
--rw-rw-r--   0 runner    (1001) docker     (123)      870 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_feature_length2.2
--rw-rw-r--   0 runner    (1001) docker     (123)      449 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features.2
--rw-rw-r--   0 runner    (1001) docker     (123)      660 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_arbitration.2
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_async_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      717 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_auto_pst.2
--rw-rw-r--   0 runner    (1001) docker     (123)      823 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_data.2
--rw-rw-r--   0 runner    (1001) docker     (123)      771 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_endurance_event_cfg.2
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_err_recovery.2
--rw-rw-r--   0 runner    (1001) docker     (123)      639 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_hctm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      778 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_host_behavior.2
--rw-rw-r--   0 runner    (1001) docker     (123)      749 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_host_id.2
--rw-rw-r--   0 runner    (1001) docker     (123)      671 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_host_mem_buf.2
--rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_iocs_profile.2
--rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_irq_coalesce.2
--rw-rw-r--   0 runner    (1001) docker     (123)      688 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_irq_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      639 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_kato.2
--rw-rw-r--   0 runner    (1001) docker     (123)      753 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_lba_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      691 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_lba_sts_interval.2
--rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_nopsc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      661 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_num_queues.2
--rw-rw-r--   0 runner    (1001) docker     (123)      775 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_plm_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      714 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_plm_window.2
--rw-rw-r--   0 runner    (1001) docker     (123)      661 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_power_mgmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      657 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_resv_mask.2
--rw-rw-r--   0 runner    (1001) docker     (123)      672 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_resv_persist.2
--rw-rw-r--   0 runner    (1001) docker     (123)      636 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_rrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      645 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_sanitize.2
--rw-rw-r--   0 runner    (1001) docker     (123)      614 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_sel.2
--rw-rw-r--   0 runner    (1001) docker     (123)      657 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_simple.2
--rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_sw_progress.2
--rw-rw-r--   0 runner    (1001) docker     (123)      670 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_temp_thresh.2
--rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_timestamp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      669 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_volatile_wc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_write_atomic.2
--rw-rw-r--   0 runner    (1001) docker     (123)      720 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_features_write_protect.2
--rw-rw-r--   0 runner    (1001) docker     (123)      867 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_host_telemetry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      645 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_lba_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      610 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_lba_status_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      417 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1105 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_ana.2
--rw-rw-r--   0 runner    (1001) docker     (123)      778 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_ana_groups.2
--rw-rw-r--   0 runner    (1001) docker     (123)      738 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_boot_partition.2
--rw-rw-r--   0 runner    (1001) docker     (123)      766 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_changed_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_cmd_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      552 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_create_telemetry_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      721 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_device_self_test.2
--rw-rw-r--   0 runner    (1001) docker     (123)      799 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_discovery.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1007 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_endurance_group.2
--rw-rw-r--   0 runner    (1001) docker     (123)      735 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_endurance_grp_evt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      830 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_error.2
--rw-rw-r--   0 runner    (1001) docker     (123)      621 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_fdp_configurations.2
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_fdp_events.2
--rw-rw-r--   0 runner    (1001) docker     (123)      573 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_fdp_stats.2
--rw-rw-r--   0 runner    (1001) docker     (123)      653 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_fid_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      784 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_fw_slot.2
--rw-rw-r--   0 runner    (1001) docker     (123)      689 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_lba_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_media_unit_stat.2
--rw-rw-r--   0 runner    (1001) docker     (123)      677 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_mi_cmd_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      589 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_page.2
--rw-rw-r--   0 runner    (1001) docker     (123)      729 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_persistent_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      793 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_predictable_lat_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_predictable_lat_nvmset.2
--rw-rw-r--   0 runner    (1001) docker     (123)      628 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_reclaim_unit_handle_usage.2
--rw-rw-r--   0 runner    (1001) docker     (123)      593 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_reservation.2
--rw-rw-r--   0 runner    (1001) docker     (123)      713 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_sanitize.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1046 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_smart.2
--rw-rw-r--   0 runner    (1001) docker     (123)      697 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_support_cap_config_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      633 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_supported_log_pages.2
--rw-rw-r--   0 runner    (1001) docker     (123)      879 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_telemetry_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      806 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_telemetry_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      764 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_log_zns_changed_zones.2
--rw-rw-r--   0 runner    (1001) docker     (123)      572 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_logical_block_size.2
--rw-rw-r--   0 runner    (1001) docker     (123)      887 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_new_host_telemetry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      463 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_ns_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      714 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_nsid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      470 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_path_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      595 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_property.2
--rw-rw-r--   0 runner    (1001) docker     (123)      493 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_get_subsys_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      501 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_hmac_alg.2
--rw-rw-r--   0 runner    (1001) docker     (123)      309 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_behavior_support.2
--rw-rw-r--   0 runner    (1001) docker     (123)      358 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_get_dhchap_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      314 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_get_hostid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      320 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_get_hostnqn.2
--rw-rw-r--   0 runner    (1001) docker     (123)      413 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_get_hostsymname.2
--rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_get_root.2
--rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_is_pdc_enabled.2
--rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_mem_buf_attrs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      614 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_metadata.2
--rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_set_dhchap_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      390 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_set_hostsymname.2
--rw-rw-r--   0 runner    (1001) docker     (123)      614 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_host_set_pdc_enabled.2
--rw-rw-r--   0 runner    (1001) docker     (123)    14784 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1482 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_anacap.2
--rw-rw-r--   0 runner    (1001) docker     (123)      387 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_apsta.2
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_avscc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1238 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_cmic.2
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_cntrltype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      581 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_cqes.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2240 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_ctratt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      523 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_dctype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      457 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_dsto.2
--rw-rw-r--   0 runner    (1001) docker     (123)      459 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_fcatt.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1347 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_fna.2
--rw-rw-r--   0 runner    (1001) docker     (123)      880 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_frmw.2
--rw-rw-r--   0 runner    (1001) docker     (123)      406 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_fuses.2
--rw-rw-r--   0 runner    (1001) docker     (123)      489 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_hctm.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1647 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_lpa.2
--rw-rw-r--   0 runner    (1001) docker     (123)      568 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_mec.2
--rw-rw-r--   0 runner    (1001) docker     (123)      706 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      681 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_nvmsr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      401 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_nvscc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      956 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_nwpc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2000 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_oacs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1247 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_oaes.2
--rw-rw-r--   0 runner    (1001) docker     (123)      405 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_ofcs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1635 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_oncs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      795 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_rpmbs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1155 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_sanicap.2
--rw-rw-r--   0 runner    (1001) docker     (123)      896 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_sgls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      581 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_sqes.2
--rw-rw-r--   0 runner    (1001) docker     (123)      606 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_vwc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1075 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ctrl_vwci.2
--rw-rw-r--   0 runner    (1001) docker     (123)      461 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_directives.2
--rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_domain_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_domain_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      411 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_endurance_group_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_independent_id_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      312 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_iocs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     7185 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1230 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_dlfeat.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1056 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_dpc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      976 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_dps.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1073 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_flbas.2
--rw-rw-r--   0 runner    (1001) docker     (123)      401 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_granularity_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      653 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_granularity_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      591 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_mc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      414 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_nmic.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1561 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_ns_rescap.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1411 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_nsfeat.2
--rw-rw-r--   0 runner    (1001) docker     (123)      399 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_nvmset_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2974 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_psd.2
--rw-rw-r--   0 runner    (1001) docker     (123)      561 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_uuid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      352 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_uuid_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      418 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_id_uuid_list_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      576 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify.2
--rw-rw-r--   0 runner    (1001) docker     (123)      917 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_active_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1114 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_active_ns_list_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      618 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_allocated_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      931 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_allocated_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1115 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_allocated_ns_list_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)     3618 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_cns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      647 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      828 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ctrl_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      867 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      843 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_domain_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_endurance_group_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      856 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_independent_identify_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      677 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_iocs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1049 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1058 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      869 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ns_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      963 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ns_csi_user_data_format.2
--rw-rw-r--   0 runner    (1001) docker     (123)      956 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ns_descs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      864 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_ns_granularity.2
--rw-rw-r--   0 runner    (1001) docker     (123)      983 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_nsid_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      954 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_nvmset_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      767 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_primary_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1125 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_secondary_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      764 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_identify_uuid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      733 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_copy_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      751 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_copy_range_f1.2
--rw-rw-r--   0 runner    (1001) docker     (123)      474 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      701 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_dsm_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      543 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_init_logging.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1001 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_insert_tls_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      450 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1149 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_control_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1785 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_dsm_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      451 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_mgmt_recv.2
--rw-rw-r--   0 runner    (1001) docker     (123)      327 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_mgmt_recv_mo.2
--rw-rw-r--   0 runner    (1001) docker     (123)      448 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_mgmt_send.2
--rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_mgmt_send_mo.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1671 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_opcode.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1874 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_passthru.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1886 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_io_passthru64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      715 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_is_64bit_reg.2
--rw-rw-r--   0 runner    (1001) docker     (123)      362 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_range_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      697 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_range_type_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      374 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_rd.2
--rw-rw-r--   0 runner    (1001) docker     (123)      484 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      499 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_status_atype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      539 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_status_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      700 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lba_status_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      531 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lbaf.2
--rw-rw-r--   0 runner    (1001) docker     (123)      749 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lbaf_rp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lbart.2
--rw-rw-r--   0 runner    (1001) docker     (123)      605 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lbas_ns_element.2
--rw-rw-r--   0 runner    (1001) docker     (123)      419 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lockdown.2
--rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_log_ana_lsp.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1108 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lookup_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      529 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lookup_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      504 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lookup_key.2
--rw-rw-r--   0 runner    (1001) docker     (123)      428 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lookup_keyring.2
--rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_lookup_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_media_unit_config_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      871 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_media_unit_stat_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      594 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_media_unit_stat_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      489 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_metadata_element_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2122 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_admin_passthru.2
--rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_format_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      575 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_fw_commit.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1143 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_fw_download.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1026 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_features_data.2
--rw-rw-r--   0 runner    (1001) docker     (123)      935 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1145 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_ana.2
--rw-rw-r--   0 runner    (1001) docker     (123)      818 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_ana_groups.2
--rw-rw-r--   0 runner    (1001) docker     (123)      779 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_boot_partition.2
--rw-rw-r--   0 runner    (1001) docker     (123)      806 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_changed_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      798 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_cmd_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      592 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      761 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_device_self_test.2
--rw-rw-r--   0 runner    (1001) docker     (123)      839 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_discovery.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1047 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_endurance_group.2
--rw-rw-r--   0 runner    (1001) docker     (123)      775 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      870 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_error.2
--rw-rw-r--   0 runner    (1001) docker     (123)      694 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      824 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_fw_slot.2
--rw-rw-r--   0 runner    (1001) docker     (123)      729 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_lba_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      671 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_media_unit_stat.2
--rw-rw-r--   0 runner    (1001) docker     (123)      718 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1027 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_page.2
--rw-rw-r--   0 runner    (1001) docker     (123)      769 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_persistent_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      833 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      684 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2
--rw-rw-r--   0 runner    (1001) docker     (123)      634 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_reservation.2
--rw-rw-r--   0 runner    (1001) docker     (123)      753 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_sanitize.2
--rw-rw-r--   0 runner    (1001) docker     (123)      833 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_simple.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1086 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_smart.2
--rw-rw-r--   0 runner    (1001) docker     (123)      738 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      673 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_supported_log_pages.2
--rw-rw-r--   0 runner    (1001) docker     (123)      919 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      846 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_telemetry_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      804 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1049 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_get_nsid_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      879 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1066 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_active_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      756 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_allocated_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1084 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_allocated_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1132 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_cns_nsid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      886 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      981 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      756 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      853 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_ns_descs.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1101 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1550 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_partial.2
--rw-rw-r--   0 runner    (1001) docker     (123)      991 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_primary_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1115 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      541 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_ns_attach.2
--rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_ns_attach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      632 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_ns_detach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1689 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_req_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      773 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_resp_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1116 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_sanitize_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      993 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_security_recv.2
--rw-rw-r--   0 runner    (1001) docker     (123)      978 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_security_send.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1703 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_admin_xfer.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1256 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_ccs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_close.2
--rw-rw-r--   0 runner    (1001) docker     (123)      260 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_close_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1905 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_cmd_supported_effects.2
--rw-rw-r--   0 runner    (1001) docker     (123)      504 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_cmd_supported_effects_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      796 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_config_id.2
--rw-rw-r--   0 runner    (1001) docker     (123)      675 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_config_smbus_freq.2
--rw-rw-r--   0 runner    (1001) docker     (123)      634 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_create_root.2
--rw-rw-r--   0 runner    (1001) docker     (123)      819 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_csts.2
--rw-rw-r--   0 runner    (1001) docker     (123)      661 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_ctrl_health_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      654 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_cwarn.2
--rw-rw-r--   0 runner    (1001) docker     (123)      964 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_dtyp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      864 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_elem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      247 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_free_root.2
--rw-rw-r--   0 runner    (1001) docker     (123)      633 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_init_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_message_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      717 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_opcode.2
--rw-rw-r--   0 runner    (1001) docker     (123)      815 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      832 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      867 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_port.2
--rw-rw-r--   0 runner    (1001) docker     (123)      741 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_subsys.2
--rw-rw-r--   0 runner    (1001) docker     (123)      706 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_req_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      602 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_resp_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_mi_subsystem_health_status_poll.2
--rw-rw-r--   0 runner    (1001) docker     (123)      707 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_msg_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_msg_resp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      608 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_nvm_ss_health_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      698 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_open_mctp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_osc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      634 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_port_pcie.2
--rw-rw-r--   0 runner    (1001) docker     (123)      678 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_port_smb.2
--rw-rw-r--   0 runner    (1001) docker     (123)      763 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_read_ctrl_info.2
--rw-rw-r--   0 runner    (1001) docker     (123)      485 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_read_nvm_ss_info.2
--rw-rw-r--   0 runner    (1001) docker     (123)      728 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_read_port_info.2
--rw-rw-r--   0 runner    (1001) docker     (123)      442 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_read_sc_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2411 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_resp_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      599 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_set_probe_enabled.2
--rw-rw-r--   0 runner    (1001) docker     (123)      653 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_status_to_string.2
--rw-rw-r--   0 runner    (1001) docker     (123)      840 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_hdr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      834 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_mr_common.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1382 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_mra.2
--rw-rw-r--   0 runner    (1001) docker     (123)      748 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_ppmra.2
--rw-rw-r--   0 runner    (1001) docker     (123)      548 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_telem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      448 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_mi_vpd_tra.2
--rw-rw-r--   0 runner    (1001) docker     (123)      675 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_attach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      677 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_detach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      319 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_filter.2
--rw-rw-r--   0 runner    (1001) docker     (123)      356 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_first_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      320 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_for_each_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      420 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_for_each_path_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_namespace_next_path.2
--rw-rw-r--   0 runner    (1001) docker     (123)      563 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nd_ns_fpi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      380 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_next_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      425 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_next_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      446 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_attach.2
--rw-rw-r--   0 runner    (1001) docker     (123)      580 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_attach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      432 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_attach_sel.2
--rw-rw-r--   0 runner    (1001) docker     (123)      487 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_compare.2
--rw-rw-r--   0 runner    (1001) docker     (123)      582 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_detach_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      276 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_flush.2
--rw-rw-r--   0 runner    (1001) docker     (123)      325 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_csi.2
--rw-rw-r--   0 runner    (1001) docker     (123)      389 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      305 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_eui64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_fd.2
--rw-rw-r--   0 runner    (1001) docker     (123)      318 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_firmware.2
--rw-rw-r--   0 runner    (1001) docker     (123)      353 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_generic_name.2
--rw-rw-r--   0 runner    (1001) docker     (123)      306 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_lba_count.2
--rw-rw-r--   0 runner    (1001) docker     (123)      295 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_lba_size.2
--rw-rw-r--   0 runner    (1001) docker     (123)      314 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_lba_util.2
--rw-rw-r--   0 runner    (1001) docker     (123)      309 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_meta_size.2
--rw-rw-r--   0 runner    (1001) docker     (123)      293 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_model.2
--rw-rw-r--   0 runner    (1001) docker     (123)      292 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_name.2
--rw-rw-r--   0 runner    (1001) docker     (123)      311 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_nguid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      271 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_nsid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      313 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_serial.2
--rw-rw-r--   0 runner    (1001) docker     (123)      336 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_subsystem.2
--rw-rw-r--   0 runner    (1001) docker     (123)      327 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_sysfs_dir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_get_uuid.2
--rw-rw-r--   0 runner    (1001) docker     (123)      714 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_id_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_id_desc_nidt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      464 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_identify.2
--rw-rw-r--   0 runner    (1001) docker     (123)      511 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_identify_descs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      261 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      776 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_metadata_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      427 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_mgmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1006 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_mgmt_create.2
--rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_mgmt_delete.2
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_mgmt_sel.2
--rw-rw-r--   0 runner    (1001) docker     (123)      496 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_read.2
--rw-rw-r--   0 runner    (1001) docker     (123)      409 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_rescan.2
--rw-rw-r--   0 runner    (1001) docker     (123)      417 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_verify.2
--rw-rw-r--   0 runner    (1001) docker     (123)      485 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_write.2
--rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_write_protect_cfg.2
--rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_write_uncorrectable.2
--rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_ns_write_zeros.2
--rw-rw-r--   0 runner    (1001) docker     (123)      497 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nss_hw_err_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      592 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvm_id_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvm_id_ns_elbaf.2
--rw-rw-r--   0 runner    (1001) docker     (123)      615 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvm_identify_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      591 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvmeset_pl_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      944 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvmset_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)      954 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvmset_pl_events.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1213 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_nvmset_predictable_lat_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      479 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_open.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1795 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_passthru_cmd.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1910 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_passthru_cmd64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      368 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_path_get_ana_state.2
--rw-rw-r--   0 runner    (1001) docker     (123)      331 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_path_get_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      319 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_path_get_name.2
--rw-rw-r--   0 runner    (1001) docker     (123)      319 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_path_get_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      348 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_path_get_sysfs_dir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_paths_filter.2
--rw-rw-r--   0 runner    (1001) docker     (123)      839 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_persistent_event_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1352 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_persistent_event_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1673 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_persistent_event_types.2
--rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_pevent_log_action.2
--rw-rw-r--   0 runner    (1001) docker     (123)      624 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_plm_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      373 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_pmr_size.2
--rw-rw-r--   0 runner    (1001) docker     (123)      401 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_pmr_throughput.2
--rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_power_on_reset_info_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1550 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_primary_ctrl_cap.2
--rw-rw-r--   0 runner    (1001) docker     (123)      811 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_psd_flags.2
--rw-rw-r--   0 runner    (1001) docker     (123)      312 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_psd_power_scale.2
--rw-rw-r--   0 runner    (1001) docker     (123)      566 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_psd_ps.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1179 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_psd_workload.2
--rw-rw-r--   0 runner    (1001) docker     (123)      401 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_read.2
--rw-rw-r--   0 runner    (1001) docker     (123)      501 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_read_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      366 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_refresh_topology.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2546 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_register_offsets.2
--rw-rw-r--   0 runner    (1001) docker     (123)      518 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_registered_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      597 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_registered_ctrl_ext.2
--rw-rw-r--   0 runner    (1001) docker     (123)      256 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_rescan_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      625 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_acquire.2
--rw-rw-r--   0 runner    (1001) docker     (123)      639 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_cptpl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      604 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_notification_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      771 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_notify_rnlpt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      530 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_racqa.2
--rw-rw-r--   0 runner    (1001) docker     (123)      566 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_register.2
--rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_release.2
--rw-rw-r--   0 runner    (1001) docker     (123)      686 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_report.2
--rw-rw-r--   0 runner    (1001) docker     (123)      586 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_rrega.2
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_rrela.2
--rw-rw-r--   0 runner    (1001) docker     (123)      930 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_rtype.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1042 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_resv_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      509 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_compln_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)     4689 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_log_page.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1022 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_nvm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      741 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_sanact.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2814 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_sstat.2
--rw-rw-r--   0 runner    (1001) docker     (123)      425 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_sanitize_start_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      293 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan.2
--rw-rw-r--   0 runner    (1001) docker     (123)      430 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_ctrl_namespace_paths.2
--rw-rw-r--   0 runner    (1001) docker     (123)      411 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_ctrl_namespaces.2
--rw-rw-r--   0 runner    (1001) docker     (123)      309 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_ctrls.2
--rw-rw-r--   0 runner    (1001) docker     (123)      352 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_namespace.2
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_subsystem_namespaces.2
--rw-rw-r--   0 runner    (1001) docker     (123)      331 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_subsystems.2
--rw-rw-r--   0 runner    (1001) docker     (123)      546 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_scan_topology.2
--rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_secondary_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      464 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_secondary_ctrl_list.2
--rw-rw-r--   0 runner    (1001) docker     (123)      464 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_security_receive.2
--rw-rw-r--   0 runner    (1001) docker     (123)      893 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_security_send.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1532 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_self_test_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_feature_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features.2
--rw-rw-r--   0 runner    (1001) docker     (123)      809 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_arbitration.2
--rw-rw-r--   0 runner    (1001) docker     (123)      657 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_async_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      762 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_auto_pst.2
--rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_data.2
--rw-rw-r--   0 runner    (1001) docker     (123)      806 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_endurance_evt_cfg.2
--rw-rw-r--   0 runner    (1001) docker     (123)      810 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_err_recovery.2
--rw-rw-r--   0 runner    (1001) docker     (123)      711 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_hctm.2
--rw-rw-r--   0 runner    (1001) docker     (123)      622 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_host_behavior.2
--rw-rw-r--   0 runner    (1001) docker     (123)      635 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_host_id.2
--rw-rw-r--   0 runner    (1001) docker     (123)      706 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_irq_coalesce.2
--rw-rw-r--   0 runner    (1001) docker     (123)      688 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_irq_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      798 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_lba_range.2
--rw-rw-r--   0 runner    (1001) docker     (123)      777 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_lba_sts_interval.2
--rw-rw-r--   0 runner    (1001) docker     (123)      675 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_nopsc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      819 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_plm_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)      730 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_plm_window.2
--rw-rw-r--   0 runner    (1001) docker     (123)      683 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_power_mgmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      675 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_resv_mask.2
--rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_resv_persist.2
--rw-rw-r--   0 runner    (1001) docker     (123)      686 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_rrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      643 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_sanitize.2
--rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_simple.2
--rw-rw-r--   0 runner    (1001) docker     (123)      676 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_sw_progress.2
--rw-rw-r--   0 runner    (1001) docker     (123)      818 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_temp_thresh.2
--rw-rw-r--   0 runner    (1001) docker     (123)      595 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_timestamp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      654 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_volatile_wc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_write_atomic.2
--rw-rw-r--   0 runner    (1001) docker     (123)      687 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_features_write_protect.2
--rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_keyring.2
--rw-rw-r--   0 runner    (1001) docker     (123)      594 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_set_property.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1472 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_smart_crit.2
--rw-rw-r--   0 runner    (1001) docker     (123)      871 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_smart_egcw.2
--rw-rw-r--   0 runner    (1001) docker     (123)     9364 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_smart_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      793 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_st_code.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1109 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_st_curr_op.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2751 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_st_result.2
--rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_st_valid_diag_info.2
--rw-rw-r--   0 runner    (1001) docker     (123)      357 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_code.2
--rw-rw-r--   0 runner    (1001) docker     (123)      387 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_code_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      518 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_equals.2
--rw-rw-r--   0 runner    (1001) docker     (123)    26826 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_field.2
--rw-rw-r--   0 runner    (1001) docker     (123)      366 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_get_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      429 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_get_value.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2073 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_result.2
--rw-rw-r--   0 runner    (1001) docker     (123)      539 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_to_errno.2
--rw-rw-r--   0 runner    (1001) docker     (123)      553 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_to_string.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1071 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_status_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      893 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_streams_directive_params.2
--rw-rw-r--   0 runner    (1001) docker     (123)      380 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_streams_directive_status.2
--rw-rw-r--   0 runner    (1001) docker     (123)      690 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_submit_admin_passthru.2
--rw-rw-r--   0 runner    (1001) docker     (123)      710 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_submit_admin_passthru64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_submit_io_passthru.2
--rw-rw-r--   0 runner    (1001) docker     (123)      686 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_submit_io_passthru64.2
--rw-rw-r--   0 runner    (1001) docker     (123)      307 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsys_filter.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1296 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsys_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      357 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_first_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      364 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_first_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      332 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_for_each_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      432 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_for_each_ctrl_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      326 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_for_each_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_for_each_ns_safe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      334 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_get_host.2
--rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_get_name.2
--rw-rw-r--   0 runner    (1001) docker     (123)      325 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_get_nqn.2
--rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_get_sysfs_dir.2
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_get_type.2
--rw-rw-r--   0 runner    (1001) docker     (123)      461 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_lookup_namespace.2
--rw-rw-r--   0 runner    (1001) docker     (123)      440 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_next_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      427 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_next_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      443 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_subsystem_reset.2
--rw-rw-r--   0 runner    (1001) docker     (123)      575 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_supported_cap_config_list_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      407 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_supported_log_pages.2
--rw-rw-r--   0 runner    (1001) docker     (123)      509 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_telemetry_da.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2627 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_telemetry_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_thermal_exc_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      422 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_time_stamp_change_event.2
--rw-rw-r--   0 runner    (1001) docker     (123)      414 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_timestamp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      250 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_unlink_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      384 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_update_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1769 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_uring_cmd.2
--rw-rw-r--   0 runner    (1001) docker     (123)      605 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_verify.2
--rw-rw-r--   0 runner    (1001) docker     (123)      373 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_version.2
--rw-rw-r--   0 runner    (1001) docker     (123)      731 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_virt_mgmt_act.2
--rw-rw-r--   0 runner    (1001) docker     (123)      405 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_virt_mgmt_rt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      839 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_virtual_mgmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      406 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_write.2
--rw-rw-r--   0 runner    (1001) docker     (123)      788 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_write_uncorrectable.2
--rw-rw-r--   0 runner    (1001) docker     (123)      705 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_write_zeros.2
--rw-rw-r--   0 runner    (1001) docker     (123)      430 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_append.2
--rw-rw-r--   0 runner    (1001) docker     (123)      438 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_changed_zone_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      699 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_desc.2
--rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_id_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1499 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_id_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      518 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_identify_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      570 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_identify_ns.2
--rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_lbafe.2
--rw-rw-r--   0 runner    (1001) docker     (123)      457 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_mgmt_recv.2
--rw-rw-r--   0 runner    (1001) docker     (123)      454 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_mgmt_send.2
--rw-rw-r--   0 runner    (1001) docker     (123)      447 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_recv_action.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1254 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_report_options.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1007 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_report_zones.2
--rw-rw-r--   0 runner    (1001) docker     (123)      803 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_send_action.2
--rw-rw-r--   0 runner    (1001) docker     (123)      593 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_za.2
--rw-rw-r--   0 runner    (1001) docker     (123)      783 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_zs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zns_zt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      443 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvme_zone_report.2
--rw-rw-r--   0 runner    (1001) docker     (123)      718 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_add_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      841 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_addr_family.2
--rw-rw-r--   0 runner    (1001) docker     (123)      364 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_adrfam_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_cms_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_connect_data.2
--rw-rw-r--   0 runner    (1001) docker     (123)      700 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_connect_disc_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)      361 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_default_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1154 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_dim_data.2
--rw-rw-r--   0 runner    (1001) docker     (123)      422 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_dim_entfmt.2
--rw-rw-r--   0 runner    (1001) docker     (123)      465 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_dim_etype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      429 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_dim_tas.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1330 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_disc_eflags.2
--rw-rw-r--   0 runner    (1001) docker     (123)     3358 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_disc_log_entry.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1155 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_discovery_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      357 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_eflags_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      442 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_exat_len.2
--rw-rw-r--   0 runner    (1001) docker     (123)      344 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_exattype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_ext_attr.2
--rw-rw-r--   0 runner    (1001) docker     (123)     1509 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_ext_die.2
--rw-rw-r--   0 runner    (1001) docker     (123)      736 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_get_discovery_log.2
--rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_get_discovery_wargs.2
--rw-rw-r--   0 runner    (1001) docker     (123)      492 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_hostid_from_file.2
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_hostnqn_from_file.2
--rw-rw-r--   0 runner    (1001) docker     (123)      338 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_hostnqn_generate.2
--rw-rw-r--   0 runner    (1001) docker     (123)      670 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_log_discovery_lid_support.2
--rw-rw-r--   0 runner    (1001) docker     (123)      608 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_log_discovery_lsp.2
--rw-rw-r--   0 runner    (1001) docker     (123)      380 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_prtype_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      384 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_qptype_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      348 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_rdma_cms.2
--rw-rw-r--   0 runner    (1001) docker     (123)      694 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_rdma_prtype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      436 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_rdma_qptype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      781 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_register_ctrl.2
--rw-rw-r--   0 runner    (1001) docker     (123)      364 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_sectype_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      371 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_subtype_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_tcp_sectype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      574 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_treq.2
--rw-rw-r--   0 runner    (1001) docker     (123)      358 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_treq_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      734 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_trtype.2
--rw-rw-r--   0 runner    (1001) docker     (123)      364 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_trtype_str.2
--rw-rw-r--   0 runner    (1001) docker     (123)      540 2023-03-31 14:05:19.000000 libnvme-1.4/doc/man/nvmf_update_config.2
--rw-rw-r--   0 runner    (1001) docker     (123)     2911 2023-03-31 14:05:19.000000 libnvme-1.4/doc/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)     2763 2023-03-31 14:05:19.000000 libnvme-1.4/doc/mi.rst.in
--rw-rw-r--   0 runner    (1001) docker     (123)       37 2023-03-31 14:05:19.000000 libnvme-1.4/doc/quickstart.rst.in
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/
--rw-rw-r--   0 runner    (1001) docker     (123)     9987 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/fabrics.rst
--rw-rw-r--   0 runner    (1001) docker     (123)     2133 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/filters.rst
--rw-rw-r--   0 runner    (1001) docker     (123)   119194 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/ioctl.rst
--rw-rw-r--   0 runner    (1001) docker     (123)     9201 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/linux.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      449 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/log.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      928 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)    79131 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/mi.rst
--rw-rw-r--   0 runner    (1001) docker     (123)    35577 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/tree.rst
--rw-rw-r--   0 runner    (1001) docker     (123)   223460 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/types.rst
--rw-rw-r--   0 runner    (1001) docker     (123)    12297 2023-03-31 14:05:19.000000 libnvme-1.4/doc/rst/util.rst
--rwxrwxr-x   0 runner    (1001) docker     (123)      939 2023-03-31 14:05:19.000000 libnvme-1.4/doc/update-docs.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/examples/
--rw-rw-r--   0 runner    (1001) docker     (123)     2631 2023-03-31 14:05:19.000000 libnvme-1.4/examples/discover-loop.c
--rw-rw-r--   0 runner    (1001) docker     (123)     1948 2023-03-31 14:05:19.000000 libnvme-1.4/examples/discover-loop.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3090 2023-03-31 14:05:19.000000 libnvme-1.4/examples/display-columnar.c
--rw-rw-r--   0 runner    (1001) docker     (123)     1869 2023-03-31 14:05:19.000000 libnvme-1.4/examples/display-tree.c
--rw-rw-r--   0 runner    (1001) docker     (123)     1085 2023-03-31 14:05:19.000000 libnvme-1.4/examples/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)     4906 2023-03-31 14:05:19.000000 libnvme-1.4/examples/mi-conf.c
--rw-rw-r--   0 runner    (1001) docker     (123)    18346 2023-03-31 14:05:19.000000 libnvme-1.4/examples/mi-mctp.c
--rw-rw-r--   0 runner    (1001) docker     (123)     3306 2023-03-31 14:05:19.000000 libnvme-1.4/examples/telemetry-listen.c
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/internal/
--rw-rw-r--   0 runner    (1001) docker     (123)      521 2023-03-31 14:05:19.000000 libnvme-1.4/internal/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/
--rw-rw-r--   0 runner    (1001) docker     (123)       40 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)     2146 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/README.md
--rw-rw-r--   0 runner    (1001) docker     (123)      231 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2720 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)    21220 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/nvme.i
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/tests/
--rwxrwxr-x   0 runner    (1001) docker     (123)      393 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/tests/create-ctrl-obj.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      958 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme/tests/gc.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1313 2023-03-31 14:05:19.000000 libnvme-1.4/libnvme.spec.in
--rwxrwxr-x   0 runner    (1001) docker     (123)      613 2023-03-31 14:05:19.000000 libnvme-1.4/meson-vcs-tag.sh
--rw-rw-r--   0 runner    (1001) docker     (123)     8199 2023-03-31 14:05:19.000000 libnvme-1.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)      998 2023-03-31 14:05:19.000000 libnvme-1.4/meson_options.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      930 2023-03-31 14:05:19.000000 libnvme-1.4/pyproject.toml
--rwxrwxr-x   0 runner    (1001) docker     (123)     2003 2023-03-31 14:05:19.000000 libnvme-1.4/release.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/src/
--rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-03-31 14:05:19.000000 libnvme-1.4/src/libnvme-mi.h
--rw-rw-r--   0 runner    (1001) docker     (123)     1227 2023-03-31 14:05:19.000000 libnvme-1.4/src/libnvme-mi.map
--rw-rw-r--   0 runner    (1001) docker     (123)      586 2023-03-31 14:05:19.000000 libnvme-1.4/src/libnvme.h
--rw-rw-r--   0 runner    (1001) docker     (123)     9511 2023-03-31 14:05:19.000000 libnvme-1.4/src/libnvme.map
--rw-rw-r--   0 runner    (1001) docker     (123)     3255 2023-03-31 14:05:19.000000 libnvme-1.4/src/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/
--rw-rw-r--   0 runner    (1001) docker     (123)    27945 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/api-types.h
--rw-rw-r--   0 runner    (1001) docker     (123)      138 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/cleanup.c
--rw-rw-r--   0 runner    (1001) docker     (123)      395 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/cleanup.h
--rw-rw-r--   0 runner    (1001) docker     (123)    38514 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/fabrics.c
--rw-rw-r--   0 runner    (1001) docker     (123)     9717 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/fabrics.h
--rw-rw-r--   0 runner    (1001) docker     (123)     2473 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/filters.c
--rw-rw-r--   0 runner    (1001) docker     (123)     2216 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/filters.h
--rw-rw-r--   0 runner    (1001) docker     (123)    55507 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/ioctl.c
--rw-rw-r--   0 runner    (1001) docker     (123)   130477 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/ioctl.h
--rw-rw-r--   0 runner    (1001) docker     (123)    17913 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/json.c
--rw-rw-r--   0 runner    (1001) docker     (123)    18165 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/linux.c
--rw-rw-r--   0 runner    (1001) docker     (123)     8856 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/linux.h
--rw-rw-r--   0 runner    (1001) docker     (123)     1914 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/log.c
--rw-rw-r--   0 runner    (1001) docker     (123)      768 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/log.h
--rw-rw-r--   0 runner    (1001) docker     (123)    18805 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/mi-mctp.c
--rw-rw-r--   0 runner    (1001) docker     (123)    39668 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/mi.c
--rw-rw-r--   0 runner    (1001) docker     (123)    88765 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/mi.h
--rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/no-json.c
--rw-rw-r--   0 runner    (1001) docker     (123)     5437 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/private.h
--rw-rw-r--   0 runner    (1001) docker     (123)    42052 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/tree.c
--rw-rw-r--   0 runner    (1001) docker     (123)    34050 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/tree.h
--rw-rw-r--   0 runner    (1001) docker     (123)   276813 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/types.h
--rw-rw-r--   0 runner    (1001) docker     (123)    35984 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/util.c
--rw-rw-r--   0 runner    (1001) docker     (123)    20225 2023-03-31 14:05:19.000000 libnvme-1.4/src/nvme/util.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (123)      124 2023-03-31 14:05:19.000000 libnvme-1.4/subprojects/dbus.wrap
--rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-03-31 14:05:19.000000 libnvme-1.4/subprojects/json-c.wrap
--rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-03-31 14:05:19.000000 libnvme-1.4/subprojects/openssl.wrap
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:05:19.000000 libnvme-1.4/test/
--rw-rw-r--   0 runner    (1001) docker     (123)     1490 2023-03-31 14:05:19.000000 libnvme-1.4/test/cpp.cc
--rw-rw-r--   0 runner    (1001) docker     (123)     1520 2023-03-31 14:05:19.000000 libnvme-1.4/test/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)    16732 2023-03-31 14:05:19.000000 libnvme-1.4/test/mi-mctp.c
--rw-rw-r--   0 runner    (1001) docker     (123)    43381 2023-03-31 14:05:19.000000 libnvme-1.4/test/mi.c
--rw-rw-r--   0 runner    (1001) docker     (123)     8522 2023-03-31 14:05:19.000000 libnvme-1.4/test/register.c
--rw-rw-r--   0 runner    (1001) docker     (123)    12728 2023-03-31 14:05:19.000000 libnvme-1.4/test/test.c
--rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-03-31 14:05:19.000000 libnvme-1.4/test/tree.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1083 2023-03-31 14:05:19.000000 libnvme-1.4/test/utils.c
--rw-rw-r--   0 runner    (1001) docker     (123)      455 2023-03-31 14:05:19.000000 libnvme-1.4/test/utils.h
--rw-rw-r--   0 runner    (1001) docker     (123)     2648 2023-03-31 14:05:19.000000 libnvme-1.4/test/uuid.c
--rw-rw-r--   0 runner    (1001) docker     (123)     1997 2023-03-31 14:05:19.000000 libnvme-1.4/test/zns.c
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-03-31 14:06:35.900871 libnvme-1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:04.797947 libnvme-1.5/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/.github/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/.github/cross/
+-rw-rw-r--   0 runner    (1001) docker     (123)      452 2023-06-30 13:17:07.000000 libnvme-1.5/.github/cross/ubuntu-cross-armhf.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      465 2023-06-30 13:17:07.000000 libnvme-1.5/.github/cross/ubuntu-cross-ppc64le.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-06-30 13:17:07.000000 libnvme-1.5/.github/cross/ubuntu-cross-s390x.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      122 2023-06-30 13:17:07.000000 libnvme-1.5/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3592 2023-06-30 13:17:07.000000 libnvme-1.5/.github/workflows/build.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1043 2023-06-30 13:17:07.000000 libnvme-1.5/.github/workflows/coverage.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1840 2023-06-30 13:17:07.000000 libnvme-1.5/.github/workflows/release-python.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      350 2023-06-30 13:17:07.000000 libnvme-1.5/.github/workflows/release.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      130 2023-06-30 13:17:07.000000 libnvme-1.5/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-06-30 13:17:07.000000 libnvme-1.5/.readthedocs.yaml
+-rw-rw-r--   0 runner    (1001) docker     (123)    26530 2023-06-30 13:17:07.000000 libnvme-1.5/COPYING
+-rw-rw-r--   0 runner    (1001) docker     (123)     1006 2023-06-30 13:17:07.000000 libnvme-1.5/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)     6536 2023-06-30 13:17:07.000000 libnvme-1.5/README.md
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/array_size/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.509817 libnvme-1.5/ccan/ccan/array_size/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1032 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/array_size/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)      889 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/array_size/array_size.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/build_assert/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.509817 libnvme-1.5/ccan/ccan/build_assert/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1350 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/build_assert/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     1228 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/build_assert/build_assert.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/check_type/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.509817 libnvme-1.5/ccan/ccan/check_type/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)      841 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/check_type/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     2368 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/check_type/check_type.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/container_of/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.509817 libnvme-1.5/ccan/ccan/container_of/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1386 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/container_of/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     4278 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/container_of/container_of.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/endian/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.509817 libnvme-1.5/ccan/ccan/endian/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1419 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/endian/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     9656 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/endian/endian.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/list/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.513817 libnvme-1.5/ccan/ccan/list/LICENSE -> ../../licenses/BSD-MIT
+-rw-rw-r--   0 runner    (1001) docker     (123)     1519 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/list/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     1000 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/list/list.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    24307 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/list/list.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/minmax/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.513817 libnvme-1.5/ccan/ccan/minmax/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1141 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/minmax/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     1266 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/minmax/minmax.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/short_types/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.513817 libnvme-1.5/ccan/ccan/short_types/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)      793 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/short_types/short_types.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/
+lrwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-06-30 13:18:16.513817 libnvme-1.5/ccan/ccan/str/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)     1355 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/_info
+-rw-rw-r--   0 runner    (1001) docker     (123)     1602 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/debug.c
+-rw-rw-r--   0 runner    (1001) docker     (123)      283 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/str.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     5958 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/str.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/ccan/str/str_debug.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/licenses/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1023 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/licenses/BSD-MIT
+-rw-rw-r--   0 runner    (1001) docker     (123)     6383 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/licenses/CC0
+-rw-rw-r--   0 runner    (1001) docker     (123)      603 2023-06-30 13:17:07.000000 libnvme-1.5/ccan/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/doc/
+-rw-rw-r--   0 runner    (1001) docker     (123)      390 2023-06-30 13:17:07.000000 libnvme-1.5/doc/api.rst.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     1054 2023-06-30 13:17:07.000000 libnvme-1.5/doc/conf.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1060 2023-06-30 13:17:07.000000 libnvme-1.5/doc/conf.py.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     4226 2023-06-30 13:17:07.000000 libnvme-1.5/doc/config-schema.json
+-rw-rw-r--   0 runner    (1001) docker     (123)     4226 2023-06-30 13:17:07.000000 libnvme-1.5/doc/config-schema.json.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      570 2023-06-30 13:17:07.000000 libnvme-1.5/doc/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      570 2023-06-30 13:17:07.000000 libnvme-1.5/doc/index.rst.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      965 2023-06-30 13:17:07.000000 libnvme-1.5/doc/installation.rst.in
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/
+-rw-rw-r--   0 runner    (1001) docker     (123)     5411 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_control.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_control_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1568 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_desc_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2320 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_discovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      379 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_discovery_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2981 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_header.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      422 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_heap_obj.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1097 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_hfi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      343 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_hfi_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     4747 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_hfi_info_tcp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1031 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_hfi_info_tcp_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      912 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2238 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_host_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1063 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      813 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_discovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      596 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_hfi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2265 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_hfi_info_tcp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      908 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      606 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_nid_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1104 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_primary_admin_host_flag.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      340 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_security.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2346 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_info_subsystem_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3604 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_security.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     5119 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_security_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      497 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_security_secret_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     5478 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_ssns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1809 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_ssns_ext_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_ssns_ext_info_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     4073 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_ssns_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1509 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_ssns_trflags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nbft_trtype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3522 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_admin_opcode.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1888 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_admin_passthru.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1906 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_admin_passthru64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      654 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ae_info_css_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      953 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ae_info_error.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1140 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ae_info_notice.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      584 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ae_info_smart.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      564 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ae_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      408 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_aggregate_endurance_group_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      416 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_aggregate_predictable_lat_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      576 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ana_group_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      472 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ana_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      732 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ana_state.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      654 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_apst_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      572 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_boot_partition.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      700 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_capacity_config_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_capacity_mgmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1067 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_change_ns_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      538 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_channel_config_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      344 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmb_size.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      903 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      415 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_effects_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      509 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_format_mset.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      655 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_format_pi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      492 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_format_pil.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      954 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_format_ses.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3373 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_get_log_lid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      493 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_cmd_get_log_telemetry_host_lsp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      415 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_compare.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2264 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_connect_err.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     4036 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_constants.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      384 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_copy.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      745 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_copy_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_copy_range_f1.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      816 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_create_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      384 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_create_root.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      402 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      328 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_first_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      335 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_first_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      295 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_for_each_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_for_each_ns_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      300 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_for_each_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      400 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_for_each_path_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_address.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      349 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      360 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_dhchap_host_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      370 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_dhchap_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      314 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_fd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      329 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_firmware.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      358 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_host_iface.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      368 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_host_traddr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_model.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_name.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      332 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_numa_node.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_phy_slot.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      333 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_queue_count.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_serial.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      317 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_sqsize.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      336 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_state.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      329 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_subsysnqn.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      342 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      338 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_sysfs_dir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      325 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_traddr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      331 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_transport.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      364 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_get_trsvcid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      503 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_identify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      351 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_is_discovered.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      485 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_is_discovery_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      351 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_is_persistent.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      396 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_is_unique_discovery_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      368 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2392 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_metadata_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      379 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_next_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      423 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_next_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      410 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_reset.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      402 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_dhchap_host_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_dhchap_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      436 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_discovered.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      510 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_discovery_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      437 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_persistent.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ctrls_filter.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      588 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_data_tfr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      452 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_default_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      511 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_describe_key_serial.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1034 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dev_self_test.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      406 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_dtype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      701 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_receive_doper.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      463 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_recv.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      623 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_recv_identify_parameters.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      661 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_recv_stream_allocate.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      637 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_recv_stream_parameters.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      681 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_recv_stream_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      729 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      595 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send_doper.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      721 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send_id_endir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      454 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send_identify_endir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      621 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send_stream_release_identifier.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      558 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_send_stream_release_resource.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      504 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_directive_types.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      373 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_disconnect_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      754 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dsm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      475 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dsm_attributes.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      390 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dsm_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      620 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dst_stc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dump_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      359 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_dump_tree.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      712 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_eg_critical_warning_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_eg_event_aggregate_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      473 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_end_grp_chan_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      871 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_end_grp_config_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1470 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_endurance_group_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      385 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_errno_to_string.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3983 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_error_log_page.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1893 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fabrics_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      780 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fctype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1029 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_config_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      945 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_config_fdpa.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_config_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      877 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      468 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_event_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      585 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_event_realloc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      333 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_event_realloc_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      816 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_event_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      422 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_events_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      649 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_reclaim_unit_handle_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      678 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_reclaim_unit_handle_update.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      329 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruh_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      471 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruh_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      599 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruh_status_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      420 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruh_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruha.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      371 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruhu_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      443 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_ruhu_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_stats_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      480 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_supported_event_attributes.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      414 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fdp_supported_event_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     8676 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      306 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_auto_pst.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      421 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_fdp_events_cdw11.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      362 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_host_behavior.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      685 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_nswpcfg_state.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_plm_window_select.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      609 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_resv_notify_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      497 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_feat_tmpthresh_thsel.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1854 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_features_async_event_config_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3956 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_features_id.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1943 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fid_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fid_supported_effects_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      450 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_firmware_slot.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_first_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_first_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      530 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_flush.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      289 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_for_each_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      371 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_for_each_host_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      315 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_for_each_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      402 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_for_each_subsystem_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      733 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_format_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_format_nvm_compln_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      495 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_format_nvm_start_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      239 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_free_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      240 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_free_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      236 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_free_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_free_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      315 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_free_tree.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fw_commit.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1621 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fw_commit_ca.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      810 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fw_commit_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1099 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fw_download.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      762 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_fw_download_seq.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_gen_dhchap_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      507 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_ana_log_len.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      441 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      476 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_ctrl_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      933 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_ctrl_telemetry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      728 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_directive_receive_length.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      741 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_discovery_args.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_feature_length.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      869 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_feature_length2.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      448 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      659 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_arbitration.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_async_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      716 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_auto_pst.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      822 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_data.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      770 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_endurance_event_cfg.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_err_recovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_hctm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      777 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_host_behavior.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      748 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_host_id.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      670 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_host_mem_buf.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      664 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_iocs_profile.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      664 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_irq_coalesce.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      687 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_irq_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_kato.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      752 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_lba_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      690 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_lba_sts_interval.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      651 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_nopsc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      660 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_num_queues.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_plm_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      713 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_plm_window.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      660 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_power_mgmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_resv_mask.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      671 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_resv_persist.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      635 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_rrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_sanitize.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      613 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_sel.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_simple.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_sw_progress.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      669 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_temp_thresh.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      629 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_timestamp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      668 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_volatile_wc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      664 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_write_atomic.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      719 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_features_write_protect.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      866 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_host_telemetry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      644 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_lba_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      609 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_lba_status_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      416 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1104 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_ana.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      777 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_ana_groups.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      737 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_boot_partition.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_changed_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      757 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_cmd_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      551 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_create_telemetry_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      720 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_device_self_test.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      798 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_discovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1006 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_endurance_group.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      734 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_endurance_grp_evt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      829 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_error.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      620 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_fdp_configurations.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_fdp_events.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      572 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_fdp_stats.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_fid_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      783 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_fw_slot.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      688 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_lba_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      629 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_media_unit_stat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      676 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_mi_cmd_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      588 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_page.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      728 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_persistent_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      792 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_predictable_lat_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      643 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_predictable_lat_nvmset.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      627 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_reclaim_unit_handle_usage.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      592 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_reservation.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      712 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_sanitize.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1045 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_smart.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      696 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_support_cap_config_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      632 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_supported_log_pages.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      878 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_telemetry_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      805 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_telemetry_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      763 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_log_zns_changed_zones.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_logical_block_size.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      886 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_new_host_telemetry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      462 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_ns_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      713 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_nsid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      469 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_path_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      594 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_property.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      492 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_get_subsys_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      500 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_hmac_alg.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      308 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_behavior_support.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      357 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_get_dhchap_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      313 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_get_hostid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      319 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_get_hostnqn.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      412 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_get_hostsymname.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      323 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_get_root.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      532 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_is_pdc_enabled.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_mem_buf_attrs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      613 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_metadata.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_set_dhchap_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      389 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_set_hostsymname.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      613 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_host_set_pdc_enabled.2
+-rw-rw-r--   0 runner    (1001) docker     (123)    14783 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1481 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_anacap.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_apsta.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      433 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_avscc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1237 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_cmic.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      493 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_cntrltype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      580 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_cqes.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2239 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_ctratt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_dctype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      456 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_dsto.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      458 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_fcatt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1346 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_fna.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      879 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_frmw.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      405 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_fuses.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      488 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_hctm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1646 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_lpa.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      567 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_mec.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      705 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      680 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_nvmsr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      400 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_nvscc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      955 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_nwpc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1999 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_oacs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1246 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_oaes.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      404 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_ofcs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1634 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_oncs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      794 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_rpmbs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1154 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_sanicap.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      895 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_sgls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      580 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_sqes.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      605 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_vwc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1074 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ctrl_vwci.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      460 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_directives.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      651 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_domain_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      443 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_domain_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      410 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_endurance_group_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1017 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_independent_id_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      311 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_iocs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     7184 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      387 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1229 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_dlfeat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1055 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_dpc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      975 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_dps.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1072 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_flbas.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      400 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_granularity_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_granularity_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      590 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_mc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      413 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_nmic.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1560 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_ns_rescap.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1410 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_nsfeat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      398 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_nvmset_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2973 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_psd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      560 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_uuid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      351 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_uuid_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      417 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_id_uuid_list_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      575 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      916 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_active_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1113 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_active_ns_list_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      617 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_allocated_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      930 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_allocated_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1114 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_allocated_ns_list_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3617 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_cns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      646 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      827 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ctrl_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      866 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      842 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_domain_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      637 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_endurance_group_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      855 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_independent_identify_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      676 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_iocs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1048 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1057 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      868 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ns_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      962 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ns_csi_user_data_format.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      955 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ns_descs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      863 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_ns_granularity.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      982 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_nsid_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      953 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_nvmset_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      766 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_primary_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1124 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_secondary_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      763 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_identify_uuid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      732 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_copy_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      750 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_copy_range_f1.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      473 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      700 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      816 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_dsm_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      542 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_init_logging.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1000 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_insert_tls_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      449 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1148 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_control_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1784 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_dsm_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      450 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_mgmt_recv.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      326 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_mgmt_recv_mo.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      447 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_mgmt_send.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      323 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_mgmt_send_mo.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1670 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_opcode.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1873 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_passthru.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1885 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_io_passthru64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      714 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_is_64bit_reg.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      361 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_range_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      696 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_range_type_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      373 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_rd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      483 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      498 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_status_atype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      538 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_status_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      699 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lba_status_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      530 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lbaf.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      748 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lbaf_rp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      746 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lbart.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      604 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lbas_ns_element.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      418 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lockdown.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      392 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_log_ana_lsp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1107 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lookup_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      528 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lookup_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      503 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lookup_key.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      427 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lookup_keyring.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      630 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_lookup_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      433 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_media_unit_config_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      870 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_media_unit_stat_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      593 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_media_unit_stat_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      488 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_metadata_element_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2121 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_admin_passthru.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      655 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_format_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      574 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_fw_commit.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1142 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_fw_download.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1025 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_features_data.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      934 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1144 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_ana.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_ana_groups.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      778 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_boot_partition.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      805 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_changed_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      797 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_cmd_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      591 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      760 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_device_self_test.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      838 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_discovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1046 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_endurance_group.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      774 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      869 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_error.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      693 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      823 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_fw_slot.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      728 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_lba_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      670 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_media_unit_stat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      717 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1026 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_page.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      768 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_persistent_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      832 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      683 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      633 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_reservation.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      752 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_sanitize.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      832 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_simple.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1085 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_smart.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      737 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      672 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_supported_log_pages.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      918 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      845 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_telemetry_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      803 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1048 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_get_nsid_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      878 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1065 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_active_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_allocated_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1083 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_allocated_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1131 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_cns_nsid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      885 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      980 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      755 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      852 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_ns_descs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1100 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1549 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_partial.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      990 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_primary_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1114 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      540 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_ns_attach.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      629 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_ns_attach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_ns_detach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1688 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_req_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      772 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_resp_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1115 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_sanitize_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      992 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_security_recv.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      977 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_security_send.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1702 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_admin_xfer.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1255 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_ccs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_close.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      259 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_close_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1904 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_cmd_supported_effects.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      503 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_cmd_supported_effects_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      795 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_config_id.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_config_smbus_freq.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      633 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_create_root.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      818 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_csts.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      660 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_ctrl_health_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      563 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_ctrl_id.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      653 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_cwarn.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      963 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_dtyp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      863 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_elem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      246 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_free_root.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      632 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_init_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      673 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_message_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      716 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_opcode.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      814 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      831 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      866 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_port.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      740 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_subsys.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      705 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_req_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      601 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_resp_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1011 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_mi_subsystem_health_status_poll.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      706 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_msg_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      655 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_msg_resp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      607 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_nvm_ss_health_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      697 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_open_mctp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_osc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      633 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_port_pcie.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      677 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_port_smb.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      762 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_read_ctrl_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      484 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_read_nvm_ss_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      727 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_read_port_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      441 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_read_sc_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2410 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_resp_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      598 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_set_probe_enabled.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      652 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_status_to_string.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      839 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_hdr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      833 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_mr_common.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1381 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_mra.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_ppmra.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      547 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_telem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      447 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_mi_vpd_tra.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_attach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      676 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_detach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      318 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_filter.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      355 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_first_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      319 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_for_each_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      419 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_for_each_path_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_namespace_next_path.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      276 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nbft_free.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      528 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nbft_read.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      562 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nd_ns_fpi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      379 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_next_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_next_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_attach.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      579 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_attach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      431 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_attach_sel.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      486 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_compare.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      581 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_detach_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_flush.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_csi.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      304 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_eui64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_fd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      317 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_firmware.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      352 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_generic_name.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      305 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_lba_count.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_lba_size.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      313 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_lba_util.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      308 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_meta_size.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      292 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_model.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      291 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_name.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      310 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_nguid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      270 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_nsid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      312 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_serial.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      335 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_subsystem.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      326 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_sysfs_dir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      381 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_get_uuid.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      713 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_id_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      816 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_id_desc_nidt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      463 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_identify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      510 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_identify_descs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      260 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      775 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_metadata_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      426 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_mgmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1142 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_mgmt_create.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      651 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_mgmt_delete.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2926 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_mgmt_host_sw_specified.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_mgmt_sel.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      495 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_read.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      408 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_rescan.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      416 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_verify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      484 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_write.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      651 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_write_protect_cfg.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_write_uncorrectable.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_ns_write_zeros.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      496 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nss_hw_err_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      591 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvm_id_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      544 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvm_id_ns_elbaf.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      614 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvm_identify_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      590 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvmeset_pl_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      943 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvmset_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      953 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvmset_pl_events.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1212 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_nvmset_predictable_lat_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_open.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1794 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_passthru_cmd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1909 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_passthru_cmd64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      367 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_path_get_ana_state.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      330 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_path_get_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      318 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_path_get_name.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      318 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_path_get_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_path_get_sysfs_dir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      297 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_paths_filter.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      838 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_persistent_event_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1351 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_persistent_event_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1672 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_persistent_event_types.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      521 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_pevent_log_action.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      623 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_plm_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      372 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_pmr_size.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      400 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_pmr_throughput.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      754 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_power_on_reset_info_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1549 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_primary_ctrl_cap.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      810 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_psd_flags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      311 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_psd_power_scale.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      565 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_psd_ps.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1178 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_psd_workload.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      400 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_read.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      500 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_read_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      365 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_refresh_topology.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2545 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_register_offsets.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      517 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_registered_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      596 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_registered_ctrl_ext.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_rescan_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      624 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_acquire.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      638 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_cptpl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      603 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_notification_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      770 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_notify_rnlpt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      529 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_racqa.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      565 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_register.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      452 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_release.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      685 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_report.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      585 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_rrega.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_rrela.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      929 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_rtype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1041 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_resv_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      508 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_compln_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     4688 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_log_page.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1021 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_nvm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      740 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_sanact.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2813 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_sstat.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_sanitize_start_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      292 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      429 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_ctrl_namespace_paths.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      410 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_ctrl_namespaces.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      308 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_ctrls.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      351 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_namespace.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      433 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_subsystem_namespaces.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      330 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_subsystems.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_scan_topology.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      754 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_secondary_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      463 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_secondary_ctrl_list.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      463 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_security_receive.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      892 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_security_send.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1531 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_self_test_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      368 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_feature_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      443 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      808 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_arbitration.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      656 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_async_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      761 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_auto_pst.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      939 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_data.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      805 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_endurance_evt_cfg.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      809 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_err_recovery.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      710 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_hctm.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      621 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_host_behavior.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      634 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_host_id.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      705 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_irq_coalesce.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      687 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_irq_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      797 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_lba_range.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      776 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_lba_sts_interval.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_nopsc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      818 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_plm_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      729 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_plm_window.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_power_mgmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      674 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_resv_mask.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      673 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_resv_persist.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      685 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_rrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      642 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_sanitize.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      773 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_simple.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      675 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_sw_progress.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      817 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_temp_thresh.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      594 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_timestamp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      653 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_volatile_wc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      643 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_write_atomic.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      686 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_features_write_protect.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      444 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_keyring.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      593 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_set_property.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1471 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_smart_crit.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      870 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_smart_egcw.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     9363 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_smart_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      792 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_st_code.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1108 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_st_curr_op.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2750 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_st_result.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      856 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_st_valid_diag_info.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      356 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_code.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_code_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      517 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_equals.2
+-rw-rw-r--   0 runner    (1001) docker     (123)    27290 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_field.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      365 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_get_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      428 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_get_value.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2072 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_result.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      538 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_to_errno.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      552 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_to_string.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1070 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_status_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      892 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_streams_directive_params.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      379 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_streams_directive_status.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      689 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_submit_admin_passthru.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      709 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_submit_admin_passthru64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_submit_io_passthru.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      685 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_submit_io_passthru64.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      306 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsys_filter.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1295 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsys_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      356 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_first_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_first_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      331 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_for_each_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      431 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_for_each_ctrl_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      325 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_for_each_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      423 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_for_each_ns_safe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      389 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_application.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      333 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_host.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      346 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_name.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_nqn.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      381 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_sysfs_dir.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_get_type.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      460 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_lookup_namespace.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      439 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_next_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      426 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_next_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      442 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_reset.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      441 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_subsystem_set_application.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      574 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_supported_cap_config_list_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      406 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_supported_log_pages.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      508 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_telemetry_da.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     2626 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_telemetry_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      362 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_thermal_exc_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      421 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_time_stamp_change_event.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      413 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_timestamp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      249 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_unlink_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_update_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1768 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_uring_cmd.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      604 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_verify.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      372 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_version.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      730 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_virt_mgmt_act.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      404 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_virt_mgmt_rt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      838 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_virtual_mgmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      405 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_write.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      787 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_write_uncorrectable.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      704 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_write_zeros.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      429 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_append.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      437 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_changed_zone_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      698 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_desc.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      392 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_id_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1498 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_id_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      517 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_identify_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      569 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_identify_ns.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      382 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_lbafe.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      456 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_mgmt_recv.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_mgmt_send.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      446 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_recv_action.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1253 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_report_options.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1006 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_report_zones.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      802 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_send_action.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      592 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_za.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      782 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_zs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      293 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zns_zt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      442 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvme_zone_report.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      717 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_add_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      840 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_addr_family.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_adrfam_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_cms_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_connect_data.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      699 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_connect_disc_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      360 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_default_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1153 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_dim_data.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      421 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_dim_entfmt.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      464 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_dim_etype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      428 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_dim_tas.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1329 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_disc_eflags.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3357 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_disc_log_entry.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1154 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_discovery_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      356 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_eflags_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      441 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_exat_len.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      343 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_exattype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      532 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_ext_attr.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     1508 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_ext_die.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      735 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_get_discovery_log.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      800 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_get_discovery_wargs.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      491 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_hostid_from_file.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      493 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_hostnqn_from_file.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      337 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_hostnqn_generate.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      669 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_log_discovery_lid_support.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      607 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_log_discovery_lsp.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      379 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_prtype_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      383 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_qptype_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_rdma_cms.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      693 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_rdma_prtype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_rdma_qptype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      780 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_register_ctrl.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_sectype_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      370 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_subtype_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      637 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_tcp_sectype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      573 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_treq.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      357 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_treq_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      733 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_trtype.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      363 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_trtype_str.2
+-rw-rw-r--   0 runner    (1001) docker     (123)      539 2023-06-30 13:17:07.000000 libnvme-1.5/doc/man/nvmf_update_config.2
+-rw-rw-r--   0 runner    (1001) docker     (123)     3076 2023-06-30 13:17:07.000000 libnvme-1.5/doc/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     2763 2023-06-30 13:17:07.000000 libnvme-1.5/doc/mi.rst.in
+-rw-rw-r--   0 runner    (1001) docker     (123)       37 2023-06-30 13:17:07.000000 libnvme-1.5/doc/quickstart.rst.in
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/
+-rw-rw-r--   0 runner    (1001) docker     (123)     9987 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/fabrics.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     2133 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/filters.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)   119357 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/ioctl.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     9201 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/linux.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      449 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/log.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)    79751 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/mi.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)    50791 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/nbft.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)    36921 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/tree.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)   226455 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/types.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)    12743 2023-06-30 13:17:07.000000 libnvme-1.5/doc/rst/util.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/examples/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2631 2023-06-30 13:17:07.000000 libnvme-1.5/examples/discover-loop.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     1952 2023-06-30 13:17:07.000000 libnvme-1.5/examples/discover-loop.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3090 2023-06-30 13:17:07.000000 libnvme-1.5/examples/display-columnar.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     1869 2023-06-30 13:17:07.000000 libnvme-1.5/examples/display-tree.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     1085 2023-06-30 13:17:07.000000 libnvme-1.5/examples/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     4906 2023-06-30 13:17:07.000000 libnvme-1.5/examples/mi-conf.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    18345 2023-06-30 13:17:07.000000 libnvme-1.5/examples/mi-mctp.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     3306 2023-06-30 13:17:07.000000 libnvme-1.5/examples/telemetry-listen.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/internal/
+-rw-rw-r--   0 runner    (1001) docker     (123)      521 2023-06-30 13:17:07.000000 libnvme-1.5/internal/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/
+-rw-rw-r--   0 runner    (1001) docker     (123)       40 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)     2146 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      231 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)    30479 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/nvme.i
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1017 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/tests/NBFT
+-rwxrwxr-x   0 runner    (1001) docker     (123)      393 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/tests/create-ctrl-obj.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      958 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/tests/gc.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     3468 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme/tests/test-nbft.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1313 2023-06-30 13:17:07.000000 libnvme-1.5/libnvme.spec.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     8580 2023-06-30 13:17:07.000000 libnvme-1.5/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      998 2023-06-30 13:17:07.000000 libnvme-1.5/meson_options.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      930 2023-06-30 13:17:07.000000 libnvme-1.5/pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/
+-rwxrwxr-x   0 runner    (1001) docker     (123)     5108 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/build.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)    70557 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/kernel-doc
+-rwxrwxr-x   0 runner    (1001) docker     (123)      264 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/kernel-doc-check
+-rwxrwxr-x   0 runner    (1001) docker     (123)      354 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/list-man-pages.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)       47 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/list-pre-compiled.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)      613 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/meson-vcs-tag.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)     3195 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/release.sh
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1002 2023-06-30 13:17:07.000000 libnvme-1.5/scripts/update-docs.sh
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/src/
+-rw-rw-r--   0 runner    (1001) docker     (123)      394 2023-06-30 13:17:07.000000 libnvme-1.5/src/libnvme-mi.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1276 2023-06-30 13:17:07.000000 libnvme-1.5/src/libnvme-mi.map
+-rw-rw-r--   0 runner    (1001) docker     (123)      609 2023-06-30 13:17:07.000000 libnvme-1.5/src/libnvme.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     9745 2023-06-30 13:17:07.000000 libnvme-1.5/src/libnvme.map
+-rw-rw-r--   0 runner    (1001) docker     (123)     3297 2023-06-30 13:17:07.000000 libnvme-1.5/src/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/
+-rw-rw-r--   0 runner    (1001) docker     (123)    28102 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/api-types.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      138 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/cleanup.c
+-rw-rw-r--   0 runner    (1001) docker     (123)      395 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/cleanup.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    44982 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/fabrics.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     9717 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/fabrics.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2473 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/filters.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     2216 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/filters.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    55763 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/ioctl.c
+-rw-rw-r--   0 runner    (1001) docker     (123)   130706 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/ioctl.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    18287 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/json.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    18165 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/linux.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     8856 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/linux.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1914 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/log.c
+-rw-rw-r--   0 runner    (1001) docker     (123)      768 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/log.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    18805 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/mi-mctp.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    40118 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/mi.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    89314 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/mi.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    21041 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/nbft.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    55759 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/nbft.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      445 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/no-json.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     6091 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/private.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    45034 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/tree.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    35246 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/tree.h
+-rw-rw-r--   0 runner    (1001) docker     (123)   280862 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/types.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    38243 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/util.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    20680 2023-06-30 13:17:07.000000 libnvme-1.5/src/nvme/util.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (123)      124 2023-06-30 13:17:07.000000 libnvme-1.5/subprojects/dbus.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-30 13:17:07.000000 libnvme-1.5/subprojects/json-c.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      631 2023-06-30 13:17:07.000000 libnvme-1.5/subprojects/openssl.wrap
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/test/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1490 2023-06-30 13:17:07.000000 libnvme-1.5/test/cpp.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1919 2023-06-30 13:17:07.000000 libnvme-1.5/test/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)    16732 2023-06-30 13:17:07.000000 libnvme-1.5/test/mi-mctp.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    43480 2023-06-30 13:17:07.000000 libnvme-1.5/test/mi.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/
+-rw-rw-r--   0 runner    (1001) docker     (123)      847 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/README
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1590 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-auto-ipv6
+-rw-rw-r--   0 runner    (1001) docker     (123)     1795 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-dhcp-ipv4
+-rw-rw-r--   0 runner    (1001) docker     (123)     1555 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-dhcp-ipv6
+-rw-rw-r--   0 runner    (1001) docker     (123)     1565 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-rhpoc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1564 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-static-ipv4
+-rw-rw-r--   0 runner    (1001) docker     (123)     1778 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-static-ipv4-discovery
+-rw-rw-r--   0 runner    (1001) docker     (123)     1564 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/diffs/NBFT-static-ipv6
+-rwxrwxr-x   0 runner    (1001) docker     (123)      101 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/gen-nbft-diffs.sh.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     1683 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/meson.build
+-rwxrwxr-x   0 runner    (1001) docker     (123)      130 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/nbft-dump-diff.sh.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     5100 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/nbft-dump.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/
+-rw-rw-r--   0 runner    (1001) docker     (123)      721 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-auto-ipv6
+-rw-rw-r--   0 runner    (1001) docker     (123)      825 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-dhcp-ipv4
+-rw-rw-r--   0 runner    (1001) docker     (123)      725 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-dhcp-ipv6
+-rw-rw-r--   0 runner    (1001) docker     (123)      724 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-rhpoc
+-rw-rw-r--   0 runner    (1001) docker     (123)      725 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-static-ipv4
+-rw-rw-r--   0 runner    (1001) docker     (123)      825 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-static-ipv4-discovery
+-rw-rw-r--   0 runner    (1001) docker     (123)      721 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables/NBFT-static-ipv6
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables_bad/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1103 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables_bad/NBFT-bad-oldspec
+-rw-rw-r--   0 runner    (1001) docker     (123)      512 2023-06-30 13:17:07.000000 libnvme-1.5/test/nbft/tables_bad/NBFT-random-noise
+-rw-rw-r--   0 runner    (1001) docker     (123)     8522 2023-06-30 13:17:07.000000 libnvme-1.5/test/register.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     3718 2023-06-30 13:17:07.000000 libnvme-1.5/test/test-util.c
+-rw-rw-r--   0 runner    (1001) docker     (123)    12728 2023-06-30 13:17:07.000000 libnvme-1.5/test/test.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     6841 2023-06-30 13:17:07.000000 libnvme-1.5/test/tree.c
+-rw-rw-r--   0 runner    (1001) docker     (123)      453 2023-06-30 13:17:07.000000 libnvme-1.5/test/tree.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1083 2023-06-30 13:17:07.000000 libnvme-1.5/test/utils.c
+-rw-rw-r--   0 runner    (1001) docker     (123)      455 2023-06-30 13:17:07.000000 libnvme-1.5/test/utils.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2648 2023-06-30 13:17:07.000000 libnvme-1.5/test/uuid.c
+-rw-rw-r--   0 runner    (1001) docker     (123)     1997 2023-06-30 13:17:07.000000 libnvme-1.5/test/zns.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-30 13:18:17.013818 libnvme-1.5/PKG-INFO
```

### Comparing `libnvme-1.4/.github/workflows/coverage.yml` & `libnvme-1.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/.github/workflows/release-python.yml` & `libnvme-1.5/.github/workflows/release-python.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,17 @@
   workflow_dispatch:
 
 jobs:
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
+      - name: install libraries
+        run: sudo apt-get install gcc pkg-config libjson-c-dev libssl-dev python3-dev
+
       - uses: actions/checkout@v3
 
       - name: Build sdist
         run: pipx run build --sdist
 
       - uses: actions/upload-artifact@v3
         with:
```

### Comparing `libnvme-1.4/COPYING` & `libnvme-1.5/COPYING`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/Makefile` & `libnvme-1.5/Makefile`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/README.md` & `libnvme-1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 This is the libnvme development C library. libnvme provides type
 definitions for NVMe specification structures, enumerations, and bit
 fields, helper functions to construct, dispatch, and decode commands
 and payloads, and utilities to connect, scan, and manage nvme devices
 on a Linux system.
 
 The public specification is the authority to resolve any protocol
-discrepencies with this library. For more info on NVM Express, please
+discrepancies with this library. For more info on NVM Express, please
 see:
 
   https://nvmexpress.org
 
 Subscribe to linux-nvme@lists.infradead.org for linux-nvme related
 discussions and development for both kernel and userspace. The list is
 archived here:
@@ -32,142 +32,133 @@
 is currently licensed LGPL-2.1-or-later, see COPYING for more
 information.
 
 Keith Busch 2020-02-06
 
 ------
 
-# Building with meson
+# Dependency
 
-## What is the meson build system?
+libnvme depends on minimum Linux kernel version v4.15, which
+introduced the /sys/class/nvme-subsystem.
 
-Here's an excerpt from the meson web site: *Meson is **an open source
-build system** meant to be both extremely fast, and, even more
-importantly, as user friendly as possible. The main design point of
-Meson is that every moment a developer spends writing or debugging
-build definitions is a second wasted.*
+# Build from source
+## Prerequisite
 
-Several well-known projects such as `systemd` and `Gnome` use meson as
-their build system. A summary of projects using meson can be found
-[here](https://mesonbuild.com/Users.html). For more info on meson,
-please consult the following sites:
+A minimal build depends on a set of build tools
 
-**Wiki page**: https://en.wikipedia.org/wiki/Meson_(software)
+  - gcc
+  - ninja
+  - meson
 
-**meson documentation**: https://mesonbuild.com/
+Not all feature will be present with such configuration, e.g.
+the fabrics part of the library wont support authentication or
+TLS over the nvme-tcp transport.
 
-**meson repo**: https://github.com/mesonbuild/meson
+To enable the optional features install following libraries
 
-## Dependency
+`/etc/nvme/config.json`` support:
+  - json-c (recommend)
 
-libnvme depends on minimum Linux kernel version v4.15, which
-introduced the /sys/class/nvme-subsystem.
+Authentication and TLS over nvme-tcp:
+  - openssl
+  - keyutils
 
-## Prerequisite
+End point discovery for MI
+  - libdbus
 
-First, install meson.
+Python bindings
+  - Python 3 interpreter
+  - Python 3 development libraries
 
-**Debian / Ubuntu**:
+## Minimal on embedded builds
 
-```bash
-sudo apt-get install meson
-```
+The reference implemention of the Meson specification is in Python 3. Installing
+or porting this dependency is not really feasible for embedded project. Though
+there are two project which implement the Ninja and the Meson API in pure C99
 
-**Fedora / Red Hat**:
+  - samurai: https://github.com/michaelforney/samurai.git
+  - muon: https://git.sr.ht/~lattis/muon
 
-```bash
-sudo dnf install meson
-```
+See the CI [build](.github/workflows/build.yml) for an example how to use it.
 
 ## To compile libnvme
 
-Using meson is similar to projects that use a `configure` script before running `make`.
-
 To `configure` the project:
 
 ```
 meson setup .build
 ```
 
 Which will default to build a shared library. To configure for static libraries call
 
 ```
-meson setup .build --default-library=static
+meson setup --default-library=static .build
 ```
 
 One nice feature of meson is that it doesn't mix build artifacts
 (e.g. `*.o`, `*.so`, etc.) with source code. In the above example,
 "`.build`" is the name of the directory where the build configuration
 as well as all the build artifacts will be saved. This directory can
 be named anything as long as it's not an existing source directory. To
 completely "clean" all the build artifacts, one need only delete the
 `.build` directory.
 
 To compile:
 
 ```
-cd .build
-ninja
-```
-
-Or:
-
-```
-ninja -C .build
+meson -C .build
 ```
 
 ## To install libnvme
 
 To install `libnvme`:
 
 ```
-cd .build
-meson install
+meson install -C .build
 ```
 
 ## To run unit tests
 
 To run unit tests:
 
 ```
-cd .build
-meson test
-```
-
-## To clean after a build
-
-To perform the equivalent of a `make clean` without deleting the build configuration.
-
-```
-cd .build
-ninja -t clean
-```
-
-Or:
-
-```
-ninja -C .build -t clean
+meson test -C .build
 ```
 
 ## To purge everything
 
 To completely clean all build artifacts, including the build configuration.
 
 ```
 rm -rf .build
 ```
 
 ## Supported build options
 
 A few build options can be specified on the command line when invoking meson.
 
-| Option | Values [default]          | Description                                                  |
-| ------ | ------------------------- | ------------------------------------------------------------ |
-| man    | true, [false]             | Instruct meson to configure the project to build the `libnvme` documentation. <br />Example: `meson .build -Dman=true` |
+| Option      | Values [default]          | Description                                                  |
+| ----------- | ------------------------- | ------------------------------------------------------------ |
+| version-tag | none                      | Overwrite the git version string in the binary               |
+| htmldir     | none                      | Installation directory for the HTML documentation            |
+| rstdir      | none                      | Installation directory for the RST documentation             |
+| docs        | [false], html, man, rst, all | Install documentation                                     |
+| docs-build  | [false], true             | Enable build documentation                                   |
 | python | [auto], enabled, disabled | Whether to build the Python bindings. When set to `auto`, the default, meson will check for the presence of the  tools and libraries (e.g. `swig`) required to build the Python bindings. If found, meson will configure the project to build the Python bindings. If a tool or library is missing, then the Python bindings won't be built. Setting this to `enabled`, forces the Python bindings to be built. When set to `disabled`, meson will configure the project to not build the Python bindings.<br />Example: `meson setup .build -Dpython=disabled` |
+| openssl     | [auto], enabled, disabled | Enables OpenSSL dependend features (e.g. authentication), adds build dependency on OpenSSL |
+| libdbus     | auto, enabled, [disabled] | Enables D-Bus dependend features (libnvme-mi: End point discovery), adds build dependency on libdbus |
+| json-c      | [auto], enabled, disabled | (recommended) Enables JSON-C dependend features (e.g. config.json parsing), adds build depdency on json-c |
+| keyutils    | [auto], enabled, disabled | Enables keyutils dependend features (e.g. TLS over TCP), adds build dependency on keyutils |
+
+See the full configuration options with
+
+```bash
+meson configure .build
+```
 
 ### Changing the build options from the command-line (i.e. w/o modifying any files)
 
 To configure a build for debugging purposes (i.e. optimization turned
 off and debug symbols enabled):
 
 ```bash
@@ -179,16 +170,9 @@
 ```bash
 meson setup .build -Db_sanitize=address
 ```
 
 This option adds `-fsanitize=address` to the gcc options. Note that when using the sanitize feature, the library `libasan.so` must be available and must be the very first library loaded when running an executable. Ensuring that `libasan.so` gets loaded first can be achieved with the `LD_PRELOAD` environment variable as follows: 
 
 ```
-meson setup .build -Db_sanitize=address && LD_PRELOAD=/lib64/libasan.so.6 ninja -C .build test 
-```
-
-To list configuration options that are available and possible values:
-
-```bash
-meson configure .build
+meson setup .build -Db_sanitize=address && LD_PRELOAD=/lib64/libasan.so.6 ninja -C .build test
 ```
-
```

### Comparing `libnvme-1.4/ccan/ccan/array_size/_info` & `libnvme-1.5/ccan/ccan/array_size/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/array_size/array_size.h` & `libnvme-1.5/ccan/ccan/array_size/array_size.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/build_assert/_info` & `libnvme-1.5/ccan/ccan/build_assert/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/build_assert/build_assert.h` & `libnvme-1.5/ccan/ccan/build_assert/build_assert.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/check_type/_info` & `libnvme-1.5/ccan/ccan/check_type/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/check_type/check_type.h` & `libnvme-1.5/ccan/ccan/check_type/check_type.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/container_of/_info` & `libnvme-1.5/ccan/ccan/container_of/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/container_of/container_of.h` & `libnvme-1.5/ccan/ccan/container_of/container_of.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/endian/_info` & `libnvme-1.5/ccan/ccan/endian/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/endian/endian.h` & `libnvme-1.5/ccan/ccan/endian/endian.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/list/_info` & `libnvme-1.5/ccan/ccan/list/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/list/list.c` & `libnvme-1.5/ccan/ccan/list/list.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/list/list.h` & `libnvme-1.5/ccan/ccan/list/list.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/minmax/_info` & `libnvme-1.5/ccan/ccan/minmax/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/minmax/minmax.h` & `libnvme-1.5/ccan/ccan/minmax/minmax.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/short_types/short_types.h` & `libnvme-1.5/ccan/ccan/short_types/short_types.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/str/_info` & `libnvme-1.5/ccan/ccan/str/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/str/debug.c` & `libnvme-1.5/ccan/ccan/str/debug.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/str/str.h` & `libnvme-1.5/ccan/ccan/str/str.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/ccan/str/str_debug.h` & `libnvme-1.5/ccan/ccan/str/str_debug.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/licenses/BSD-MIT` & `libnvme-1.5/ccan/licenses/BSD-MIT`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/licenses/CC0` & `libnvme-1.5/ccan/licenses/CC0`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/ccan/meson.build` & `libnvme-1.5/ccan/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/conf.py` & `libnvme-1.5/doc/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'libnvme'
 copyright = '2020, Keith Busch'
 author = 'Keith Busch <kbusch@kernel.org>'
 master_doc = 'index'
 
-release = '1.4'
+release = '1.5'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `libnvme-1.4/doc/conf.py.in` & `libnvme-1.5/doc/conf.py.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/config-schema.json` & `libnvme-1.5/doc/config-schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539683%*

 * *Differences: {"'$defs'": "{'subsystem': {'properties': {'application': OrderedDict([('description', 'Program "*

 * *            "managing this subsystem'), ('type', 'string')])}}}"}*

```diff
@@ -144,14 +144,18 @@
                 "transport"
             ],
             "type": "object"
         },
         "subsystem": {
             "description": "NVMe subsystem properties",
             "properties": {
+                "application": {
+                    "description": "Program managing this subsystem",
+                    "type": "string"
+                },
                 "nqn": {
                     "description": "Subsystem NQN",
                     "maxLength": 223,
                     "type": "string"
                 },
                 "ports": {
                     "description": "Array of NVMe subsystem ports",
```

### Comparing `libnvme-1.4/doc/config-schema.json.in` & `libnvme-1.5/doc/config-schema.json.in`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539683%*

 * *Differences: {"'$defs'": "{'subsystem': {'properties': {'application': OrderedDict([('description', 'Program "*

 * *            "managing this subsystem'), ('type', 'string')])}}}"}*

```diff
@@ -144,14 +144,18 @@
                 "transport"
             ],
             "type": "object"
         },
         "subsystem": {
             "description": "NVMe subsystem properties",
             "properties": {
+                "application": {
+                    "description": "Program managing this subsystem",
+                    "type": "string"
+                },
                 "nqn": {
                     "description": "Subsystem NQN",
                     "maxLength": 223,
                     "type": "string"
                 },
                 "ports": {
                     "description": "Array of NVMe subsystem ports",
```

### Comparing `libnvme-1.4/doc/index.rst` & `libnvme-1.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/index.rst.in` & `libnvme-1.5/doc/index.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/installation.rst.in` & `libnvme-1.5/doc/installation.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/kernel-doc` & `libnvme-1.5/scripts/kernel-doc`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/man/nvme_admin_opcode.2` & `libnvme-1.5/doc/man/nvme_admin_opcode.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_admin_opcode" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_admin_opcode" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_admin_opcode \- Known NVMe admin opcodes
 .SH SYNOPSIS
 enum nvme_admin_opcode {
 .br
 .BI "    nvme_admin_delete_sq"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_admin_passthru.2` & `libnvme-1.5/doc/man/nvme_admin_passthru.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_admin_passthru" 9 "nvme_admin_passthru" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_admin_passthru" 9 "nvme_admin_passthru" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_admin_passthru \- Submit an nvme passthrough command
 .SH SYNOPSIS
 .B "int" nvme_admin_passthru
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_admin_passthru64.2` & `libnvme-1.5/doc/man/nvme_io_passthru64.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_admin_passthru64" 9 "nvme_admin_passthru64" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_io_passthru64" 9 "nvme_io_passthru64" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_admin_passthru64 \- Submit a 64-bit nvme passthrough command
+nvme_io_passthru64 \- Submit an nvme io passthrough command
 .SH SYNOPSIS
-.B "int" nvme_admin_passthru64
+.B "int" nvme_io_passthru64
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_admin_passthru64\fP. This sets up and
-submits a \fIstruct nvme_passthru_cmd64\fP.
+Parameterized form of \fBnvme_submit_io_passthru64\fP. This sets up and submits
+a \fIstruct nvme_passthru_cmd64\fP.
 
-Known values for \fIopcode\fP are defined in \fIenum nvme_admin_opcode\fP.
+Known values for \fIopcode\fP are defined in \fIenum nvme_io_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_ae_info_css_nvm.2` & `libnvme-1.5/doc/man/nvme_ae_info_css_nvm.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_css_nvm" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_css_nvm" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_css_nvm \- Asynchronous Event Information - I/O Command Specific Status
 .SH SYNOPSIS
 enum nvme_ae_info_css_nvm {
 .br
 .BI "    NVME_AER_CSS_NVM_RESERVATION"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ae_info_error.2` & `libnvme-1.5/doc/man/nvme_ae_info_error.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_error" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_error" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_error \- Asynchronous Event Information - Error Status
 .SH SYNOPSIS
 enum nvme_ae_info_error {
 .br
 .BI "    NVME_AER_ERROR_INVALID_DB_REG"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ae_info_notice.2` & `libnvme-1.5/doc/man/nvme_ae_info_notice.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_notice" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_notice" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_notice \- Asynchronous Event Information - Notice
 .SH SYNOPSIS
 enum nvme_ae_info_notice {
 .br
 .BI "    NVME_AER_NOTICE_NS_CHANGED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ae_info_smart.2` & `libnvme-1.5/doc/man/nvme_ae_info_smart.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_smart" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_smart" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_smart \- Asynchronous Event Information - SMART / Health Status
 .SH SYNOPSIS
 enum nvme_ae_info_smart {
 .br
 .BI "    NVME_AER_SMART_SUBSYSTEM_RELIABILITY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ae_type.2` & `libnvme-1.5/doc/man/nvme_ae_type.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_type \- Asynchronous Event Type
 .SH SYNOPSIS
 enum nvme_ae_type {
 .br
 .BI "    NVME_AER_ERROR"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ana_group_desc.2` & `libnvme-1.5/doc/man/nvme_ana_group_desc.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_ana_group_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_ana_group_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_ana_group_desc \- ANA Group Descriptor
 .SH SYNOPSIS
 struct nvme_ana_group_desc {
 .br
 .BI "    __le32 grpid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_ana_state.2` & `libnvme-1.5/doc/man/nvme_ana_state.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ana_state" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ana_state" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ana_state \- ANA Group Descriptor - Asymmetric Namespace Access State
 .SH SYNOPSIS
 enum nvme_ana_state {
 .br
 .BI "    NVME_ANA_STATE_OPTIMIZED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_apst_entry.2` & `libnvme-1.5/doc/man/nvme_apst_entry.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_apst_entry" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_apst_entry" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_apst_entry \- Autonomous Power State Transition
 .SH SYNOPSIS
 enum nvme_apst_entry {
 .br
 .BI "    NVME_APST_ENTRY_ITPS_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_boot_partition.2` & `libnvme-1.5/doc/man/nvme_boot_partition.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_boot_partition" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_boot_partition" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_boot_partition \- Boot Partition Log
 .SH SYNOPSIS
 struct nvme_boot_partition {
 .br
 .BI "    __u8 lid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_capacity_config_desc.2` & `libnvme-1.5/doc/man/nvme_capacity_config_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_capacity_config_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_capacity_config_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_capacity_config_desc \- Capacity Configuration structure definitions
 .SH SYNOPSIS
 struct nvme_capacity_config_desc {
 .br
 .BI "    __le16 cap_config_id;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_change_ns_event.2` & `libnvme-1.5/doc/man/nvme_change_ns_event.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_change_ns_event" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_change_ns_event" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_change_ns_event \- Change Namespace Event Data
 .SH SYNOPSIS
 struct nvme_change_ns_event {
 .br
 .BI "    __le32 nsmgt_cdw10;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_channel_config_desc.2` & `libnvme-1.5/doc/man/nvme_channel_config_desc.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_channel_config_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_channel_config_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_channel_config_desc \- Channel Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_channel_config_desc {
 .br
 .BI "    __le16 chanid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_cmd_effects.2` & `libnvme-1.5/doc/man/nvme_cmd_effects.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_effects" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_effects" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_effects \- Commands Supported and Effects
 .SH SYNOPSIS
 enum nvme_cmd_effects {
 .br
 .BI "    NVME_CMD_EFFECTS_CSUPP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_cmd_format_pi.2` & `libnvme-1.5/doc/man/nvme_cmd_format_pi.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_format_pi" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_format_pi" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_format_pi \- Format NVM - Protection Information
 .SH SYNOPSIS
 enum nvme_cmd_format_pi {
 .br
 .BI "    NVME_FORMAT_PI_DISABLE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_cmd_format_ses.2` & `libnvme-1.5/doc/man/nvme_cmd_format_ses.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_format_ses" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_format_ses" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_format_ses \- Format NVM - Secure Erase Settings
 .SH SYNOPSIS
 enum nvme_cmd_format_ses {
 .br
 .BI "    NVME_FORMAT_SES_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_cmd_get_log_lid.2` & `libnvme-1.5/doc/man/nvme_cmd_get_log_lid.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_get_log_lid" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_get_log_lid" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_get_log_lid \- Get Log Page -Log Page Identifiers
 .SH SYNOPSIS
 enum nvme_cmd_get_log_lid {
 .br
 .BI "    NVME_LOG_LID_SUPPORTED_LOG_PAGES"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_connect_err.2` & `libnvme-1.5/doc/man/nvme_connect_err.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_connect_err" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_connect_err" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_connect_err \- nvme connect error codes
 .SH SYNOPSIS
 enum nvme_connect_err {
 .br
 .BI "    ENVME_CONNECT_RESOLVE"
 , 
@@ -69,14 +69,22 @@
 .br
 .br
 .BI "    ENVME_CONNECT_OPNOTSUPP"
 , 
 .br
 .br
 .BI "    ENVME_CONNECT_CONNREFUSED"
+, 
+.br
+.br
+.BI "    ENVME_CONNECT_ADDRNOTAVAIL"
+, 
+.br
+.br
+.BI "    ENVME_CONNECT_IGNORED"
 
 };
 .SH Constants
 .IP "ENVME_CONNECT_RESOLVE" 12
 failed to resolve host
 .IP "ENVME_CONNECT_ADDRFAM" 12
 unrecognized address family
@@ -108,7 +116,11 @@
 hostnqn already in use
 .IP "ENVME_CONNECT_NODEV" 12
 invalid interface
 .IP "ENVME_CONNECT_OPNOTSUPP" 12
 not supported
 .IP "ENVME_CONNECT_CONNREFUSED" 12
 connection refused
+.IP "ENVME_CONNECT_ADDRNOTAVAIL" 12
+cannot assign requested address
+.IP "ENVME_CONNECT_IGNORED" 12
+connect attempt is ignored due to configuration
```

### Comparing `libnvme-1.4/doc/man/nvme_constants.2` & `libnvme-1.5/doc/man/nvme_constants.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_constants" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_constants" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_constants \- A place to stash various constant nvme values
 .SH SYNOPSIS
 enum nvme_constants {
 .br
 .BI "    NVME_NSID_ALL"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_copy_range.2` & `libnvme-1.5/doc/man/nvme_copy_range.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range \- Copy - Source Range Entries Descriptor Format
 .SH SYNOPSIS
 struct nvme_copy_range {
 .br
 .BI "    __u8 rsvd0[8];"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_copy_range_f1.2` & `libnvme-1.5/doc/man/nvme_copy_range_f1.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range_f1" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range_f1" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range_f1 \- Copy - Source Range Entries Descriptor Format 1h
 .SH SYNOPSIS
 struct nvme_copy_range_f1 {
 .br
 .BI "    __u8 rsvd0[8];"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_create_ctrl.2` & `libnvme-1.5/doc/man/nvme_create_ctrl.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_create_ctrl" 9 "nvme_create_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_create_ctrl" 9 "nvme_create_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_create_ctrl \- Allocate an unconnected NVMe controller
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvme_create_ctrl
 .BI "(nvme_root_t r "  ","
 .BI "const char *subsysnqn "  ","
 .BI "const char *transport "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_ctrl_metadata_type.2` & `libnvme-1.5/doc/man/nvme_ctrl_metadata_type.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ctrl_metadata_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ctrl_metadata_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ctrl_metadata_type \- Controller Metadata Element Types
 .SH SYNOPSIS
 enum nvme_ctrl_metadata_type {
 .br
 .BI "    NVME_CTRL_METADATA_OS_CTRL_NAME"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2` & `libnvme-1.5/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_set_unique_discovery_ctrl" 9 "nvme_ctrl_set_unique_discovery_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_ctrl_set_unique_discovery_ctrl" 9 "nvme_ctrl_set_unique_discovery_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_set_unique_discovery_ctrl \- Set the 'unique_discovery_ctrl' flag
 .SH SYNOPSIS
 .B "void" nvme_ctrl_set_unique_discovery_ctrl
 .BI "(nvme_ctrl_t c "  ","
 .BI "bool unique "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_data_tfr.2` & `libnvme-1.5/doc/man/nvme_data_tfr.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_data_tfr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_data_tfr" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_data_tfr \- Data transfer direction of the command
 .SH SYNOPSIS
 enum nvme_data_tfr {
 .br
 .BI "    NVME_DATA_TFR_NO_DATA_TFR"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_dev_self_test.2` & `libnvme-1.5/doc/man/nvme_dev_self_test.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_dev_self_test" 9 "nvme_dev_self_test" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_dev_self_test" 9 "nvme_dev_self_test" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_dev_self_test \- Start or abort a self test
 .SH SYNOPSIS
 .B "int" nvme_dev_self_test
 .BI "(struct nvme_dev_self_test_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_receive_doper.2` & `libnvme-1.5/doc/man/nvme_directive_receive_doper.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_directive_receive_doper" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_directive_receive_doper" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_directive_receive_doper \- Directive Receive Directive Operation
 .SH SYNOPSIS
 enum nvme_directive_receive_doper {
 .br
 .BI "    NVME_DIRECTIVE_RECEIVE_IDENTIFY_DOPER_PARAM"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_recv_identify_parameters.2` & `libnvme-1.5/doc/man/nvme_directive_recv_identify_parameters.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_identify_parameters" 9 "nvme_directive_recv_identify_parameters" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_identify_parameters" 9 "nvme_directive_recv_identify_parameters" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_identify_parameters \- Directive receive identifier parameters
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_identify_parameters
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_directives *id "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_recv_stream_allocate.2` & `libnvme-1.5/doc/man/nvme_directive_recv_stream_allocate.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_allocate" 9 "nvme_directive_recv_stream_allocate" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_allocate" 9 "nvme_directive_recv_stream_allocate" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_allocate \- Directive receive stream allocate
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_allocate
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 nsr "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_recv_stream_parameters.2` & `libnvme-1.5/doc/man/nvme_directive_recv_stream_parameters.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_parameters" 9 "nvme_directive_recv_stream_parameters" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_parameters" 9 "nvme_directive_recv_stream_parameters" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_parameters \- Directive receive stream parameters
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_parameters
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_streams_directive_params *parms "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_recv_stream_status.2` & `libnvme-1.5/doc/man/nvme_directive_recv_stream_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_status" 9 "nvme_directive_recv_stream_status" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_status" 9 "nvme_directive_recv_stream_status" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_status \- Directive receive stream status
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_status
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "unsigned int nr_entries "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_send.2` & `libnvme-1.5/doc/man/nvme_directive_send_stream_release_resource.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-.TH "nvme_directive_send" 9 "nvme_directive_send" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_send_stream_release_resource" 9 "nvme_directive_send_stream_release_resource" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_directive_send \- Send directive command
+nvme_directive_send_stream_release_resource \- Directive Send Stream release resources
 .SH SYNOPSIS
-.B "int" nvme_directive_send
-.BI "(struct nvme_directive_send_args *args "  ");"
+.B "int" nvme_directive_send_stream_release_resource
+.BI "(int fd "  ","
+.BI "__u32 nsid "  ");"
 .SH ARGUMENTS
-.IP "args" 12
-\fIstruct nvme_directive_send_args\fP argument structure
-.SH "DESCRIPTION"
-Directives is a mechanism to enable host and NVM subsystem or controller
-information exchange. The Directive Send command transfers data related to a
-specific Directive Type from the host to the controller.
-
-See the NVMe specification for more information.
+.IP "fd" 12
+File descriptor of nvme device
+.IP "nsid" 12
+Namespace ID
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_send_doper.2` & `libnvme-1.5/doc/man/nvme_directive_send_doper.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_directive_send_doper" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_directive_send_doper" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_directive_send_doper \- Directive Send Directive Operation
 .SH SYNOPSIS
 enum nvme_directive_send_doper {
 .br
 .BI "    NVME_DIRECTIVE_SEND_IDENTIFY_DOPER_ENDIR"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_directive_send_id_endir.2` & `libnvme-1.5/doc/man/nvme_directive_send_id_endir.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_send_id_endir" 9 "nvme_directive_send_id_endir" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_directive_send_id_endir" 9 "nvme_directive_send_id_endir" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_send_id_endir \- Directive Send Enable Directive
 .SH SYNOPSIS
 .B "int" nvme_directive_send_id_endir
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool endir "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_dsm.2` & `libnvme-1.5/doc/man/nvme_dsm.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_dsm" 9 "nvme_dsm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_dsm" 9 "nvme_dsm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_dsm \- Send an nvme data set management command
 .SH SYNOPSIS
 .B "int" nvme_dsm
 .BI "(struct nvme_dsm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_dst_stc.2` & `libnvme-1.5/doc/man/nvme_dst_stc.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_dst_stc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_dst_stc" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_dst_stc \- Action taken by the Device Self-test command
 .SH SYNOPSIS
 enum nvme_dst_stc {
 .br
 .BI "    NVME_DST_STC_SHORT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_eg_critical_warning_flags.2` & `libnvme-1.5/doc/man/nvme_eg_critical_warning_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_eg_critical_warning_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_eg_critical_warning_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_eg_critical_warning_flags \- Endurance Group Information Log - Critical Warning
 .SH SYNOPSIS
 enum nvme_eg_critical_warning_flags {
 .br
 .BI "    NVME_EG_CRITICAL_WARNING_SPARE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_end_grp_config_desc.2` & `libnvme-1.5/doc/man/nvme_end_grp_config_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_end_grp_config_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_end_grp_config_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_end_grp_config_desc \- Endurance Group Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_end_grp_config_desc {
 .br
 .BI "    __le16 endgid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_endurance_group_log.2` & `libnvme-1.5/doc/man/nvme_endurance_group_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_endurance_group_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_endurance_group_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_endurance_group_log \- Endurance Group Information Log
 .SH SYNOPSIS
 struct nvme_endurance_group_log {
 .br
 .BI "    __u8 critical_warning;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_error_log_page.2` & `libnvme-1.5/doc/man/nvme_error_log_page.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_error_log_page" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_error_log_page" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_error_log_page \- Error Information Log Entry (Log Identifier 01h)
 .SH SYNOPSIS
 struct nvme_error_log_page {
 .br
 .BI "    __le64 error_count;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fabrics_config.2` & `libnvme-1.5/doc/man/nvme_fabrics_config.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fabrics_config" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fabrics_config" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fabrics_config \- Defines all linux nvme fabrics initiator options
 .SH SYNOPSIS
 struct nvme_fabrics_config {
 .br
 .BI "    char *host_traddr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fctype.2` & `libnvme-1.5/doc/man/nvme_fctype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fctype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fctype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fctype \- Fabrics Command Types
 .SH SYNOPSIS
 enum nvme_fctype {
 .br
 .BI "    nvme_fabrics_type_property_set"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_config_desc.2` & `libnvme-1.5/doc/man/nvme_fdp_config_desc.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_config_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_config_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_config_desc \- FDP Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_fdp_config_desc {
 .br
 .BI "    __le16 size;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_config_fdpa.2` & `libnvme-1.5/doc/man/nvme_fdp_config_fdpa.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_config_fdpa" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_config_fdpa" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_config_fdpa \- FDP Attributes
 .SH SYNOPSIS
 enum nvme_fdp_config_fdpa {
 .br
 .BI "    NVME_FDP_CONFIG_FDPA_RGIF_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_config_log.2` & `libnvme-1.5/doc/man/nvme_fdp_config_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_config_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_config_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_config_log \- FDP Configurations Log Page
 .SH SYNOPSIS
 struct nvme_fdp_config_log {
 .br
 .BI "    __le16 n;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_event.2` & `libnvme-1.5/doc/man/nvme_fdp_event.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_event" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_event" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_event \- FDP Event
 .SH SYNOPSIS
 struct nvme_fdp_event {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_event_realloc.2` & `libnvme-1.5/doc/man/nvme_fdp_event_realloc.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_event_realloc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_event_realloc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_event_realloc \- Media Reallocated Event Type Specific Information
 .SH SYNOPSIS
 struct nvme_fdp_event_realloc {
 .br
 .BI "    __u8 flags;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_event_type.2` & `libnvme-1.5/doc/man/nvme_fdp_event_type.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_event_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_event_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_event_type \- FDP Event Types
 .SH SYNOPSIS
 enum nvme_fdp_event_type {
 .br
 .BI "    NVME_FDP_EVENT_RUNFW"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_reclaim_unit_handle_status.2` & `libnvme-1.5/doc/man/nvme_fdp_reclaim_unit_handle_status.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fdp_reclaim_unit_handle_status" 9 "nvme_fdp_reclaim_unit_handle_status" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_fdp_reclaim_unit_handle_status" 9 "nvme_fdp_reclaim_unit_handle_status" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_fdp_reclaim_unit_handle_status \- Get reclaim unit handle status
 .SH SYNOPSIS
 .B "int" nvme_fdp_reclaim_unit_handle_status
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 data_len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_reclaim_unit_handle_update.2` & `libnvme-1.5/doc/man/nvme_fdp_reclaim_unit_handle_update.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fdp_reclaim_unit_handle_update" 9 "nvme_fdp_reclaim_unit_handle_update" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_fdp_reclaim_unit_handle_update" 9 "nvme_fdp_reclaim_unit_handle_update" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_fdp_reclaim_unit_handle_update \- Update a list of reclaim unit handles
 .SH SYNOPSIS
 .B "int" nvme_fdp_reclaim_unit_handle_update
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "unsigned int npids "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_ruh_status_desc.2` & `libnvme-1.5/doc/man/nvme_fdp_ruh_status_desc.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_ruh_status_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_ruh_status_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_ruh_status_desc \- Reclaim Unit Handle Status Descriptor
 .SH SYNOPSIS
 struct nvme_fdp_ruh_status_desc {
 .br
 .BI "    __le16 pid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fdp_ruha.2` & `libnvme-1.5/doc/man/nvme_fdp_ruha.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_ruha" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_ruha" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_ruha \- Reclaim Unit Handle Attributes
 .SH SYNOPSIS
 enum nvme_fdp_ruha {
 .br
 .BI "    NVME_FDP_RUHA_HOST_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_feat.2` & `libnvme-1.5/doc/man/nvme_feat.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_feat \- Features Access Shifts/Masks values
 .SH SYNOPSIS
 enum nvme_feat {
 .br
 .BI "    NVME_FEAT_ARBITRATION_BURST_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_feat_nswpcfg_state.2` & `libnvme-1.5/doc/man/nvme_feat_nswpcfg_state.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat_nswpcfg_state" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat_nswpcfg_state" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_feat_nswpcfg_state \- Write Protection - Write Protection State
 .SH SYNOPSIS
 enum nvme_feat_nswpcfg_state {
 .br
 .BI "    NVME_FEAT_NS_NO_WRITE_PROTECT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_feat_resv_notify_flags.2` & `libnvme-1.5/doc/man/nvme_feat_resv_notify_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat_resv_notify_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat_resv_notify_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_feat_resv_notify_flags \- Reservation Notification Configuration
 .SH SYNOPSIS
 enum nvme_feat_resv_notify_flags {
 .br
 .BI "    NVME_FEAT_RESV_NOTIFY_REGPRE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_features_async_event_config_flags.2` & `libnvme-1.5/doc/man/nvme_features_async_event_config_flags.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_features_async_event_config_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_features_async_event_config_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_features_async_event_config_flags \- Asynchronous Event Configuration configuration flags
 .SH SYNOPSIS
 enum nvme_features_async_event_config_flags {
 .br
 .BI "    NVME_FEATURE_AENCFG_SMART_CRIT_SPARE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_features_id.2` & `libnvme-1.5/doc/man/nvme_features_id.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_features_id" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_features_id" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_features_id \- Features - Feature Identifiers
 .SH SYNOPSIS
 enum nvme_features_id {
 .br
 .BI "    NVME_FEAT_FID_ARBITRATION"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_fid_supported_effects.2` & `libnvme-1.5/doc/man/nvme_fid_supported_effects.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fid_supported_effects" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fid_supported_effects" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fid_supported_effects \- FID Supported and Effects Data Structure definitions
 .SH SYNOPSIS
 enum nvme_fid_supported_effects {
 .br
 .BI "    NVME_FID_SUPPORTED_EFFECTS_FSUPP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_flush.2` & `libnvme-1.5/doc/man/nvme_flush.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_flush" 9 "nvme_flush" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_flush" 9 "nvme_flush" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_flush \- Send an nvme flush command
 .SH SYNOPSIS
 .B "int" nvme_flush
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_format_nvm.2` & `libnvme-1.5/doc/man/nvme_format_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_format_nvm" 9 "nvme_format_nvm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_format_nvm" 9 "nvme_format_nvm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_format_nvm \- Format nvme namespace(s)
 .SH SYNOPSIS
 .B "int" nvme_format_nvm
 .BI "(struct nvme_format_nvm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_format_nvm_compln_event.2` & `libnvme-1.5/doc/man/nvme_format_nvm_compln_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_format_nvm_compln_event" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_format_nvm_compln_event" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_format_nvm_compln_event \- Format NVM Completion Event Data
 .SH SYNOPSIS
 struct nvme_format_nvm_compln_event {
 .br
 .BI "    __le32 nsid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fw_commit.2` & `libnvme-1.5/doc/man/nvme_fw_commit.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_commit" 9 "nvme_fw_commit" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_fw_commit" 9 "nvme_fw_commit" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_commit \- Commit firmware using the specified action
 .SH SYNOPSIS
 .B "int" nvme_fw_commit
 .BI "(struct nvme_fw_commit_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_fw_commit_ca.2` & `libnvme-1.5/doc/man/nvme_fw_commit_ca.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fw_commit_ca" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fw_commit_ca" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_fw_commit_ca \- Firmware Commit - Commit Action
 .SH SYNOPSIS
 enum nvme_fw_commit_ca {
 .br
 .BI "    NVME_FW_COMMIT_CA_REPLACE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_fw_commit_event.2` & `libnvme-1.5/doc/man/nvme_fw_commit_event.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fw_commit_event" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fw_commit_event" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_fw_commit_event \- Firmware Commit Event Data
 .SH SYNOPSIS
 struct nvme_fw_commit_event {
 .br
 .BI "    __le64 old_fw_rev;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_fw_download.2` & `libnvme-1.5/doc/man/nvme_fw_download.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_download" 9 "nvme_fw_download" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_fw_download" 9 "nvme_fw_download" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_download \- Download part or all of a firmware image to the controller
 .SH SYNOPSIS
 .B "int" nvme_fw_download
 .BI "(struct nvme_fw_download_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_fw_download_seq.2` & `libnvme-1.5/doc/man/nvme_fw_download_seq.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_download_seq" 9 "nvme_fw_download_seq" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_fw_download_seq" 9 "nvme_fw_download_seq" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_download_seq \- Firmware download sequence
 .SH SYNOPSIS
 .B "int" nvme_fw_download_seq
 .BI "(int fd "  ","
 .BI "__u32 size "  ","
 .BI "__u32 xfer "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_gen_dhchap_key.2` & `libnvme-1.5/doc/man/nvme_gen_dhchap_key.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_gen_dhchap_key" 9 "nvme_gen_dhchap_key" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_gen_dhchap_key" 9 "nvme_gen_dhchap_key" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_gen_dhchap_key \- DH-HMAC-CHAP key generation
 .SH SYNOPSIS
 .B "int" nvme_gen_dhchap_key
 .BI "(char *hostnqn "  ","
 .BI "enum nvme_hmac_alg hmac "  ","
 .BI "unsigned int key_len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_ctrl_telemetry.2` & `libnvme-1.5/doc/man/nvme_get_ctrl_telemetry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_ctrl_telemetry" 9 "nvme_get_ctrl_telemetry" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_ctrl_telemetry" 9 "nvme_get_ctrl_telemetry" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_ctrl_telemetry \- Get controller telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_ctrl_telemetry
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_telemetry_log **log "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_directive_receive_length.2` & `libnvme-1.5/doc/man/nvme_get_directive_receive_length.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_directive_receive_length" 9 "nvme_get_directive_receive_length" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_directive_receive_length" 9 "nvme_get_directive_receive_length" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_directive_receive_length \- Get directive receive length
 .SH SYNOPSIS
 .B "int" nvme_get_directive_receive_length
 .BI "(enum nvme_directive_dtype dtype "  ","
 .BI "enum nvme_directive_receive_doper doper "  ","
 .BI "__u32 *len "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_discovery_args.2` & `libnvme-1.5/doc/man/nvme_get_discovery_args.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_get_discovery_args" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_get_discovery_args" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_get_discovery_args \- Arguments for nvmf_get_discovery_wargs()
 .SH SYNOPSIS
 struct nvme_get_discovery_args {
 .br
 .BI "    nvme_ctrl_t c;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_get_feature_length.2` & `libnvme-1.5/doc/man/nvme_get_feature_length.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_feature_length" 9 "nvme_get_feature_length" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_feature_length" 9 "nvme_get_feature_length" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_feature_length \- Retreive the command payload length for a specific feature identifier
 .SH SYNOPSIS
 .B "int" nvme_get_feature_length
 .BI "(int fid "  ","
 .BI "__u32 cdw11 "  ","
 .BI "__u32 *len "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_feature_length2.2` & `libnvme-1.5/doc/man/nvme_get_feature_length2.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_feature_length2" 9 "nvme_get_feature_length2" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_feature_length2" 9 "nvme_get_feature_length2" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_feature_length2 \- Retreive the command payload length for a specific feature identifier
 .SH SYNOPSIS
 .B "int" nvme_get_feature_length2
 .BI "(int fid "  ","
 .BI "__u32 cdw11 "  ","
 .BI "enum nvme_data_tfr dir "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_arbitration.2` & `libnvme-1.5/doc/man/nvme_get_features_arbitration.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_arbitration" 9 "nvme_get_features_arbitration" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_arbitration" 9 "nvme_get_features_arbitration" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_arbitration \- Get arbitration feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_arbitration
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_async_event.2` & `libnvme-1.5/doc/man/nvme_get_features_async_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_async_event" 9 "nvme_get_features_async_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_async_event" 9 "nvme_get_features_async_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_async_event \- Get asynchronous event feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_async_event
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_auto_pst.2` & `libnvme-1.5/doc/man/nvme_get_features_auto_pst.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_auto_pst" 9 "nvme_get_features_auto_pst" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_auto_pst" 9 "nvme_get_features_auto_pst" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_auto_pst \- Get autonomous power state feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_auto_pst
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_feat_auto_pst *apst "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_data.2` & `libnvme-1.5/doc/man/nvme_get_features_data.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_data" 9 "nvme_get_features_data" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_data" 9 "nvme_get_features_data" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_data \- Helper function for @nvme_get_features()
 .SH SYNOPSIS
 .B "int" nvme_get_features_data
 .BI "(int fd "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_endurance_event_cfg.2` & `libnvme-1.5/doc/man/nvme_get_features_endurance_event_cfg.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_endurance_event_cfg" 9 "nvme_get_features_endurance_event_cfg" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_endurance_event_cfg" 9 "nvme_get_features_endurance_event_cfg" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_endurance_event_cfg \- Get endurance event config feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_endurance_event_cfg
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u16 endgid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_err_recovery.2` & `libnvme-1.5/doc/man/nvme_get_features_err_recovery.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_err_recovery" 9 "nvme_get_features_err_recovery" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_err_recovery" 9 "nvme_get_features_err_recovery" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_err_recovery \- Get error recovery feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_err_recovery
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_hctm.2` & `libnvme-1.5/doc/man/nvme_get_features_nopsc.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_hctm" 9 "nvme_get_features_hctm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_nopsc" 9 "nvme_get_features_nopsc" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_hctm \- Get thermal management feature
+nvme_get_features_nopsc \- Get non-operational power state feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_hctm
+.B "int" nvme_get_features_nopsc
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_host_behavior.2` & `libnvme-1.5/doc/man/nvme_get_features_host_behavior.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_behavior" 9 "nvme_get_features_host_behavior" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_behavior" 9 "nvme_get_features_host_behavior" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_behavior \- Get host behavior feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_behavior
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_feat_host_behavior *data "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_host_id.2` & `libnvme-1.5/doc/man/nvme_get_features_host_id.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_id" 9 "nvme_get_features_host_id" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_id" 9 "nvme_get_features_host_id" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_id \- Get host id feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_id
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "bool exhid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_host_mem_buf.2` & `libnvme-1.5/doc/man/nvme_get_features_host_mem_buf.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_mem_buf" 9 "nvme_get_features_host_mem_buf" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_mem_buf" 9 "nvme_get_features_host_mem_buf" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_mem_buf \- Get host memory buffer feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_mem_buf
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_iocs_profile.2` & `libnvme-1.5/doc/man/nvme_get_features_write_protect.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-.TH "nvme_get_features_iocs_profile" 9 "nvme_get_features_iocs_profile" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_write_protect" 9 "nvme_get_features_write_protect" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_iocs_profile \- Get IOCS profile feature
+nvme_get_features_write_protect \- Get write protect feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_iocs_profile
+.B "int" nvme_get_features_write_protect
 .BI "(int fd "  ","
+.BI "__u32 nsid "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
+.IP "nsid" 12
+Namespace ID
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_irq_coalesce.2` & `libnvme-1.5/doc/man/nvme_get_features_irq_coalesce.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_irq_coalesce" 9 "nvme_get_features_irq_coalesce" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_irq_coalesce" 9 "nvme_get_features_irq_coalesce" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_irq_coalesce \- Get IRQ coalesce feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_irq_coalesce
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_irq_config.2` & `libnvme-1.5/doc/man/nvme_get_features_irq_config.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_irq_config" 9 "nvme_get_features_irq_config" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_irq_config" 9 "nvme_get_features_irq_config" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_irq_config \- Get IRQ config feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_irq_config
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u16 iv "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_kato.2` & `libnvme-1.5/doc/man/nvme_get_features_kato.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_kato" 9 "nvme_get_features_kato" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_kato" 9 "nvme_get_features_kato" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_kato \- Get keep alive timeout feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_kato
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_lba_range.2` & `libnvme-1.5/doc/man/nvme_set_features_lba_range.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-.TH "nvme_get_features_lba_range" 9 "nvme_get_features_lba_range" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_lba_range" 9 "nvme_set_features_lba_range" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_lba_range \- Get LBA range feature
+nvme_set_features_lba_range \- Set LBA range feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_lba_range
+.B "int" nvme_set_features_lba_range
 .BI "(int fd "  ","
-.BI "enum nvme_get_features_sel sel "  ","
+.BI "__u32 nsid "  ","
+.BI "__u32 nr_ranges "  ","
+.BI "bool save "  ","
 .BI "struct nvme_lba_range_type *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "sel" 12
-Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "nsid" 12
+Namespace ID
+.IP "nr_ranges" 12
+Number of ranges in \fIdata\fP
+.IP "save" 12
+Save value across power states
 .IP "data" 12
-User address of feature data, if applicable
+User address of feature data
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_lba_sts_interval.2` & `libnvme-1.5/doc/man/nvme_get_features_lba_sts_interval.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_lba_sts_interval" 9 "nvme_get_features_lba_sts_interval" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_lba_sts_interval" 9 "nvme_get_features_lba_sts_interval" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_lba_sts_interval \- Get LBA status information feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_lba_sts_interval
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_nopsc.2` & `libnvme-1.5/doc/man/nvme_get_features_hctm.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_nopsc" 9 "nvme_get_features_nopsc" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_hctm" 9 "nvme_get_features_hctm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_nopsc \- Get non-operational power state feature
+nvme_get_features_hctm \- Get thermal management feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_nopsc
+.B "int" nvme_get_features_hctm
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_num_queues.2` & `libnvme-1.5/doc/man/nvme_get_features_num_queues.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_num_queues" 9 "nvme_get_features_num_queues" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_num_queues" 9 "nvme_get_features_num_queues" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_num_queues \- Get number of queues feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_num_queues
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_plm_config.2` & `libnvme-1.5/doc/man/nvme_get_features_plm_config.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_plm_config" 9 "nvme_get_features_plm_config" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_plm_config" 9 "nvme_get_features_plm_config" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_plm_config \- Get predictable latency feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_plm_config
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u16 nvmsetid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_plm_window.2` & `libnvme-1.5/doc/man/nvme_set_features_sw_progress.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-.TH "nvme_get_features_plm_window" 9 "nvme_get_features_plm_window" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_sw_progress" 9 "nvme_set_features_sw_progress" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_plm_window \- Get window select feature
+nvme_set_features_sw_progress \- Set pre-boot software load count feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_plm_window
+.B "int" nvme_set_features_sw_progress
 .BI "(int fd "  ","
-.BI "enum nvme_get_features_sel sel "  ","
-.BI "__u16 nvmsetid "  ","
+.BI "__u8 pbslc "  ","
+.BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "sel" 12
-Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
-.IP "nvmsetid" 12
-NVM set id
+.IP "pbslc" 12
+Pre-boot Software Load Count
+.IP "save" 12
+Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_power_mgmt.2` & `libnvme-1.5/doc/man/nvme_get_features_power_mgmt.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_power_mgmt" 9 "nvme_get_features_power_mgmt" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_power_mgmt" 9 "nvme_get_features_power_mgmt" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_power_mgmt \- Get power management feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_power_mgmt
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_resv_mask.2` & `libnvme-1.5/doc/man/nvme_get_features_iocs_profile.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_resv_mask" 9 "nvme_get_features_resv_mask" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_iocs_profile" 9 "nvme_get_features_iocs_profile" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_resv_mask \- Get reservation mask feature
+nvme_get_features_iocs_profile \- Get IOCS profile feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_resv_mask
+.B "int" nvme_get_features_iocs_profile
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_resv_persist.2` & `libnvme-1.5/doc/man/nvme_get_features_resv_persist.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_resv_persist" 9 "nvme_get_features_resv_persist" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_persist" 9 "nvme_get_features_resv_persist" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_resv_persist \- Get reservation persist feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_resv_persist
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_rrl.2` & `libnvme-1.5/doc/man/nvme_get_features_resv_mask.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_rrl" 9 "nvme_get_features_rrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_mask" 9 "nvme_get_features_resv_mask" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_rrl \- Get read recovery level feature
+nvme_get_features_resv_mask \- Get reservation mask feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_rrl
+.B "int" nvme_get_features_resv_mask
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_sanitize.2` & `libnvme-1.5/doc/man/nvme_get_features_rrl.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_sanitize" 9 "nvme_get_features_sanitize" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_rrl" 9 "nvme_get_features_rrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_sanitize \- Get sanitize feature
+nvme_get_features_rrl \- Get read recovery level feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_sanitize
+.B "int" nvme_get_features_rrl
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_sel.2` & `libnvme-1.5/doc/man/nvme_get_features_sel.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_get_features_sel" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_get_features_sel" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_get_features_sel \- Get Features - Select
 .SH SYNOPSIS
 enum nvme_get_features_sel {
 .br
 .BI "    NVME_GET_FEATURES_SEL_CURRENT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_simple.2` & `libnvme-1.5/doc/man/nvme_get_features_simple.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_simple" 9 "nvme_get_features_simple" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_simple" 9 "nvme_get_features_simple" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_simple \- Helper function for @nvme_get_features()
 .SH SYNOPSIS
 .B "int" nvme_get_features_simple
 .BI "(int fd "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_sw_progress.2` & `libnvme-1.5/doc/man/nvme_get_features_sw_progress.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_sw_progress" 9 "nvme_get_features_sw_progress" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_sw_progress" 9 "nvme_get_features_sw_progress" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_sw_progress \- Get software progress feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_sw_progress
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_temp_thresh.2` & `libnvme-1.5/doc/man/nvme_get_features_volatile_wc.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_temp_thresh" 9 "nvme_get_features_temp_thresh" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_volatile_wc" 9 "nvme_get_features_volatile_wc" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_temp_thresh \- Get temperature threshold feature
+nvme_get_features_volatile_wc \- Get volatile write cache feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_temp_thresh
+.B "int" nvme_get_features_volatile_wc
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_timestamp.2` & `libnvme-1.5/doc/man/nvme_get_features_timestamp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_timestamp" 9 "nvme_get_features_timestamp" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_timestamp" 9 "nvme_get_features_timestamp" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_timestamp \- Get timestamp feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_timestamp
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_timestamp *ts "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_volatile_wc.2` & `libnvme-1.5/doc/man/nvme_get_features_plm_window.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-.TH "nvme_get_features_volatile_wc" 9 "nvme_get_features_volatile_wc" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_plm_window" 9 "nvme_get_features_plm_window" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_volatile_wc \- Get volatile write cache feature
+nvme_get_features_plm_window \- Get window select feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_volatile_wc
+.B "int" nvme_get_features_plm_window
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
+.BI "__u16 nvmsetid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "nvmsetid" 12
+NVM set id
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_write_atomic.2` & `libnvme-1.5/doc/man/nvme_get_features_write_atomic.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_write_atomic" 9 "nvme_get_features_write_atomic" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_write_atomic" 9 "nvme_get_features_write_atomic" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_write_atomic \- Get write atomic feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_write_atomic
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_features_write_protect.2` & `libnvme-1.5/doc/man/nvme_get_features_lba_range.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-.TH "nvme_get_features_write_protect" 9 "nvme_get_features_write_protect" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_lba_range" 9 "nvme_get_features_lba_range" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_write_protect \- Get write protect feature
+nvme_get_features_lba_range \- Get LBA range feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_write_protect
+.B "int" nvme_get_features_lba_range
 .BI "(int fd "  ","
-.BI "__u32 nsid "  ","
 .BI "enum nvme_get_features_sel sel "  ","
+.BI "struct nvme_lba_range_type *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "nsid" 12
-Namespace ID
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "data" 12
+User address of feature data, if applicable
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_host_telemetry.2` & `libnvme-1.5/doc/man/nvme_get_host_telemetry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_host_telemetry" 9 "nvme_get_host_telemetry" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_host_telemetry" 9 "nvme_get_host_telemetry" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_host_telemetry \- Get host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_host_telemetry
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log **log "  ","
 .BI "enum nvme_telemetry_da da "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_lba_status.2` & `libnvme-1.5/doc/man/nvme_get_lba_status.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_lba_status" 9 "nvme_get_lba_status" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_lba_status" 9 "nvme_get_lba_status" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_lba_status \- Retrieve information on possibly unrecoverable LBAs
 .SH SYNOPSIS
 .B "int" nvme_get_lba_status
 .BI "(struct nvme_get_lba_status_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_lba_status_log.2` & `libnvme-1.5/doc/man/nvme_get_lba_status_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_lba_status_log" 9 "nvme_get_lba_status_log" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_lba_status_log" 9 "nvme_get_lba_status_log" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_lba_status_log \- Retrieve the LBA Status log page
 .SH SYNOPSIS
 .B "int" nvme_get_lba_status_log
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_lba_status_log **log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_ana.2` & `libnvme-1.5/doc/man/nvme_get_log_ana.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_ana" 9 "nvme_get_log_ana" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_ana" 9 "nvme_get_log_ana" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_ana \- Retrieve Asymmetric Namespace Access log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_ana
 .BI "(int fd "  ","
 .BI "enum nvme_log_ana_lsp lsp "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_ana_groups.2` & `libnvme-1.5/doc/man/nvme_get_log_ana_groups.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_ana_groups" 9 "nvme_get_log_ana_groups" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_ana_groups" 9 "nvme_get_log_ana_groups" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_ana_groups \- Retrieve Asymmetric Namespace Access groups only log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_ana_groups
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_boot_partition.2` & `libnvme-1.5/doc/man/nvme_get_log_boot_partition.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_boot_partition" 9 "nvme_get_log_boot_partition" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_boot_partition" 9 "nvme_get_log_boot_partition" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_boot_partition \- Retrieve Boot Partition
 .SH SYNOPSIS
 .B "int" nvme_get_log_boot_partition
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u8 lsp "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_changed_ns_list.2` & `libnvme-1.5/doc/man/nvme_get_log_changed_ns_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_changed_ns_list" 9 "nvme_get_log_changed_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_changed_ns_list" 9 "nvme_get_log_changed_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_changed_ns_list \- Retrieve namespace changed list
 .SH SYNOPSIS
 .B "int" nvme_get_log_changed_ns_list
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_ns_list *ns_log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_create_telemetry_host.2` & `libnvme-1.5/doc/man/nvme_get_log_create_telemetry_host.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_create_telemetry_host" 9 "nvme_get_log_create_telemetry_host" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_create_telemetry_host" 9 "nvme_get_log_create_telemetry_host" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_create_telemetry_host \- Create host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_log_create_telemetry_host
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_device_self_test.2` & `libnvme-1.5/doc/man/nvme_get_log_device_self_test.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_device_self_test" 9 "nvme_get_log_device_self_test" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_device_self_test" 9 "nvme_get_log_device_self_test" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_device_self_test \- Retrieve the device self test log
 .SH SYNOPSIS
 .B "int" nvme_get_log_device_self_test
 .BI "(int fd "  ","
 .BI "struct nvme_self_test_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_discovery.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_discovery.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.TH "nvme_get_log_discovery" 9 "nvme_get_log_discovery" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_discovery" 9 "nvme_mi_admin_get_log_discovery" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_discovery \- Retrieve Discovery log page
+nvme_mi_admin_get_log_discovery \- Retrieve Discovery log page
 .SH SYNOPSIS
-.B "int" nvme_get_log_discovery
-.BI "(int fd "  ","
+.B "int" nvme_mi_admin_get_log_discovery
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
 .BI "__u32 len "  ","
 .BI "void *log "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
+.IP "ctrl" 12
+Controller to query
 .IP "rae" 12
 Retain asynchronous events
 .IP "offset" 12
 Offset of this log to retrieve
 .IP "len" 12
 The allocated size for this portion of the log
 .IP "log" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_endurance_group.2` & `libnvme-1.5/doc/man/nvme_get_log_endurance_group.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_endurance_group" 9 "nvme_get_log_endurance_group" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_endurance_group" 9 "nvme_get_log_endurance_group" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_endurance_group \- Get Endurance Group log
 .SH SYNOPSIS
 .B "int" nvme_get_log_endurance_group
 .BI "(int fd "  ","
 .BI "__u16 endgid "  ","
 .BI "struct nvme_endurance_group_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_endurance_grp_evt.2` & `libnvme-1.5/doc/man/nvme_get_log_endurance_grp_evt.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_endurance_grp_evt" 9 "nvme_get_log_endurance_grp_evt" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_endurance_grp_evt" 9 "nvme_get_log_endurance_grp_evt" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_endurance_grp_evt \- Retrieve Rotational Media Information
 .SH SYNOPSIS
 .B "int" nvme_get_log_endurance_grp_evt
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_error.2` & `libnvme-1.5/doc/man/nvme_get_log_error.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_error" 9 "nvme_get_log_error" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_error" 9 "nvme_get_log_error" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_error \- Retrieve nvme error log
 .SH SYNOPSIS
 .B "int" nvme_get_log_error
 .BI "(int fd "  ","
 .BI "unsigned int nr_entries "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_fdp_configurations.2` & `libnvme-1.5/doc/man/nvme_get_log_fdp_configurations.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fdp_configurations" 9 "nvme_get_log_fdp_configurations" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_fdp_configurations" 9 "nvme_get_log_fdp_configurations" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fdp_configurations \- Get list of Flexible Data Placement configurations
 .SH SYNOPSIS
 .B "int" nvme_get_log_fdp_configurations
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_fdp_events.2` & `libnvme-1.5/doc/man/nvme_get_log_fdp_events.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fdp_events" 9 "nvme_get_log_fdp_events" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_fdp_events" 9 "nvme_get_log_fdp_events" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fdp_events \- Get Flexible Data Placement events
 .SH SYNOPSIS
 .B "int" nvme_get_log_fdp_events
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "bool host_events "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_fdp_stats.2` & `libnvme-1.5/doc/man/nvme_get_log_fdp_stats.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fdp_stats" 9 "nvme_get_log_fdp_stats" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_fdp_stats" 9 "nvme_get_log_fdp_stats" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fdp_stats \- Get Flexible Data Placement statistics
 .SH SYNOPSIS
 .B "int" nvme_get_log_fdp_stats
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_fid_supported_effects.2` & `libnvme-1.5/doc/man/nvme_get_log_mi_cmd_supported_effects.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH "nvme_get_log_fid_supported_effects" 9 "nvme_get_log_fid_supported_effects" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_mi_cmd_supported_effects" 9 "nvme_get_log_mi_cmd_supported_effects" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_fid_supported_effects \- Retrieve Feature Identifiers Supported and Effects
+nvme_get_log_mi_cmd_supported_effects \- displays the MI Commands Supported by the controller
 .SH SYNOPSIS
-.B "int" nvme_get_log_fid_supported_effects
+.B "int" nvme_get_log_mi_cmd_supported_effects
 .BI "(int fd "  ","
 .BI "bool rae "  ","
-.BI "struct nvme_fid_supported_effects_log *log "  ");"
+.BI "struct nvme_mi_cmd_supported_effects_log *log "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "rae" 12
 Retain asynchronous events
 .IP "log" 12
-FID Supported and Effects data structure
+MI Command Supported and Effects data structure
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_fw_slot.2` & `libnvme-1.5/doc/man/nvme_get_log_fw_slot.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fw_slot" 9 "nvme_get_log_fw_slot" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_fw_slot" 9 "nvme_get_log_fw_slot" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fw_slot \- Retrieves the controller firmware log
 .SH SYNOPSIS
 .B "int" nvme_get_log_fw_slot
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_firmware_slot *fw_log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_lba_status.2` & `libnvme-1.5/doc/man/nvme_get_log_lba_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_lba_status" 9 "nvme_get_log_lba_status" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_lba_status" 9 "nvme_get_log_lba_status" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_lba_status \- Retrieve LBA Status
 .SH SYNOPSIS
 .B "int" nvme_get_log_lba_status
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_media_unit_stat.2` & `libnvme-1.5/doc/man/nvme_get_log_media_unit_stat.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_media_unit_stat" 9 "nvme_get_log_media_unit_stat" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_media_unit_stat" 9 "nvme_get_log_media_unit_stat" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_media_unit_stat \- Retrieve Media Unit Status
 .SH SYNOPSIS
 .B "int" nvme_get_log_media_unit_stat
 .BI "(int fd "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_media_unit_stat_log *mus "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_mi_cmd_supported_effects.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_supported_log_pages.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH "nvme_get_log_mi_cmd_supported_effects" 9 "nvme_get_log_mi_cmd_supported_effects" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_supported_log_pages" 9 "nvme_mi_admin_get_log_supported_log_pages" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_mi_cmd_supported_effects \- displays the MI Commands Supported by the controller
+nvme_mi_admin_get_log_supported_log_pages \- Retrieve nmve supported log pages
 .SH SYNOPSIS
-.B "int" nvme_get_log_mi_cmd_supported_effects
-.BI "(int fd "  ","
+.B "int" nvme_mi_admin_get_log_supported_log_pages
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
-.BI "struct nvme_mi_cmd_supported_effects_log *log "  ");"
+.BI "struct nvme_supported_log_pages *log "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
+.IP "ctrl" 12
+Controller to query
 .IP "rae" 12
 Retain asynchronous events
 .IP "log" 12
-MI Command Supported and Effects data structure
+Array of LID supported and Effects data structures
 .SH "RETURN"
 The nvme command status if a response was received (see
-\fIenum nvme_status_field\fP) or -1 with errno set otherwise
+\fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_page.2` & `libnvme-1.5/doc/man/nvme_get_log_page.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_page" 9 "nvme_get_log_page" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_page" 9 "nvme_get_log_page" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_page \- Get log page data
 .SH SYNOPSIS
 .B "int" nvme_get_log_page
 .BI "(int fd "  ","
 .BI "__u32 xfer_len "  ","
 .BI "struct nvme_get_log_args *args "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_persistent_event.2` & `libnvme-1.5/doc/man/nvme_get_log_persistent_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_persistent_event" 9 "nvme_get_log_persistent_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_persistent_event" 9 "nvme_get_log_persistent_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_persistent_event \- Retrieve Persistent Event Log
 .SH SYNOPSIS
 .B "int" nvme_get_log_persistent_event
 .BI "(int fd "  ","
 .BI "enum nvme_pevent_log_action action "  ","
 .BI "__u32 size "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_predictable_lat_event.2` & `libnvme-1.5/doc/man/nvme_get_log_predictable_lat_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_predictable_lat_event" 9 "nvme_get_log_predictable_lat_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_predictable_lat_event" 9 "nvme_get_log_predictable_lat_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_predictable_lat_event \- Retrieve Predictable Latency Event Aggregate Log Page
 .SH SYNOPSIS
 .B "int" nvme_get_log_predictable_lat_event
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_predictable_lat_nvmset.2` & `libnvme-1.5/doc/man/nvme_get_log_predictable_lat_nvmset.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_predictable_lat_nvmset" 9 "nvme_get_log_predictable_lat_nvmset" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_predictable_lat_nvmset" 9 "nvme_get_log_predictable_lat_nvmset" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_predictable_lat_nvmset \- Predictable Latency Per NVM Set
 .SH SYNOPSIS
 .B "int" nvme_get_log_predictable_lat_nvmset
 .BI "(int fd "  ","
 .BI "__u16 nvmsetid "  ","
 .BI "struct nvme_nvmset_predictable_lat_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_reclaim_unit_handle_usage.2` & `libnvme-1.5/doc/man/nvme_get_log_reclaim_unit_handle_usage.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_reclaim_unit_handle_usage" 9 "nvme_get_log_reclaim_unit_handle_usage" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_reclaim_unit_handle_usage" 9 "nvme_get_log_reclaim_unit_handle_usage" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_reclaim_unit_handle_usage \- Get reclaim unit handle usage
 .SH SYNOPSIS
 .B "int" nvme_get_log_reclaim_unit_handle_usage
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_reservation.2` & `libnvme-1.5/doc/man/nvme_get_log_reservation.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_reservation" 9 "nvme_get_log_reservation" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_reservation" 9 "nvme_get_log_reservation" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_reservation \- Retrieve Reservation Notification
 .SH SYNOPSIS
 .B "int" nvme_get_log_reservation
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_resv_notification_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_sanitize.2` & `libnvme-1.5/doc/man/nvme_get_log_sanitize.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_sanitize" 9 "nvme_get_log_sanitize" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_sanitize" 9 "nvme_get_log_sanitize" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_sanitize \- Retrieve Sanitize Status
 .SH SYNOPSIS
 .B "int" nvme_get_log_sanitize
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_sanitize_log_page *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_smart.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_smart.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-.TH "nvme_get_log_smart" 9 "nvme_get_log_smart" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_smart" 9 "nvme_mi_admin_get_log_smart" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_smart \- Retrieve nvme smart log
+nvme_mi_admin_get_log_smart \- Retrieve nvme smart log
 .SH SYNOPSIS
-.B "int" nvme_get_log_smart
-.BI "(int fd "  ","
+.B "int" nvme_mi_admin_get_log_smart
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_smart_log *smart_log "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
+.IP "ctrl" 12
+Controller to query
 .IP "nsid" 12
 Optional namespace identifier
 .IP "rae" 12
 Retain asynchronous events
 .IP "smart_log" 12
 User address to store the smart log
 .SH "DESCRIPTION"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_support_cap_config_list.2` & `libnvme-1.5/doc/man/nvme_get_log_support_cap_config_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_support_cap_config_list" 9 "nvme_get_log_support_cap_config_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_support_cap_config_list" 9 "nvme_get_log_support_cap_config_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_support_cap_config_list \- Retrieve Supported Capacity Configuration List
 .SH SYNOPSIS
 .B "int" nvme_get_log_support_cap_config_list
 .BI "(int fd "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_supported_cap_config_list_log *cap "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_supported_log_pages.2` & `libnvme-1.5/doc/man/nvme_get_log_supported_log_pages.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_supported_log_pages" 9 "nvme_get_log_supported_log_pages" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_supported_log_pages" 9 "nvme_get_log_supported_log_pages" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_supported_log_pages \- Retrieve nmve supported log pages
 .SH SYNOPSIS
 .B "int" nvme_get_log_supported_log_pages
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_supported_log_pages *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_telemetry_ctrl.2` & `libnvme-1.5/doc/man/nvme_get_log_telemetry_ctrl.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_telemetry_ctrl" 9 "nvme_get_log_telemetry_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_telemetry_ctrl" 9 "nvme_get_log_telemetry_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_telemetry_ctrl \- Get Telemetry Controller-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_telemetry_ctrl
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_telemetry_host.2` & `libnvme-1.5/doc/man/nvme_get_log_telemetry_host.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_telemetry_host" 9 "nvme_get_log_telemetry_host" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_telemetry_host" 9 "nvme_get_log_telemetry_host" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_telemetry_host \- Get Telemetry Host-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_telemetry_host
 .BI "(int fd "  ","
 .BI "__u64 offset "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_log_zns_changed_zones.2` & `libnvme-1.5/doc/man/nvme_get_log_zns_changed_zones.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_zns_changed_zones" 9 "nvme_get_log_zns_changed_zones" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_zns_changed_zones" 9 "nvme_get_log_zns_changed_zones" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_zns_changed_zones \- Retrieve list of zones that have changed
 .SH SYNOPSIS
 .B "int" nvme_get_log_zns_changed_zones
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_logical_block_size.2` & `libnvme-1.5/doc/man/nvme_get_logical_block_size.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_logical_block_size" 9 "nvme_get_logical_block_size" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_logical_block_size" 9 "nvme_get_logical_block_size" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_logical_block_size \- Retrieve block size
 .SH SYNOPSIS
 .B "int" nvme_get_logical_block_size
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "int *blksize "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_get_new_host_telemetry.2` & `libnvme-1.5/doc/man/nvme_get_new_host_telemetry.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_new_host_telemetry" 9 "nvme_get_new_host_telemetry" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_new_host_telemetry" 9 "nvme_get_new_host_telemetry" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_new_host_telemetry \- Get new host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_new_host_telemetry
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log **log "  ","
 .BI "enum nvme_telemetry_da da "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_get_nsid.2` & `libnvme-1.5/doc/man/nvme_get_nsid.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_nsid" 9 "nvme_get_nsid" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_nsid" 9 "nvme_get_nsid" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_nsid \- Retrieve the NSID from a namespace file descriptor
 .SH SYNOPSIS
 .B "int" nvme_get_nsid
 .BI "(int fd "  ","
 .BI "__u32 *nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_get_property.2` & `libnvme-1.5/doc/man/nvme_get_property.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_property" 9 "nvme_get_property" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_property" 9 "nvme_get_property" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_property \- Get a controller property
 .SH SYNOPSIS
 .B "int" nvme_get_property
 .BI "(struct nvme_get_property_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_host_is_pdc_enabled.2` & `libnvme-1.5/doc/man/nvme_host_is_pdc_enabled.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_host_is_pdc_enabled" 9 "nvme_host_is_pdc_enabled" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_host_is_pdc_enabled" 9 "nvme_host_is_pdc_enabled" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_host_is_pdc_enabled \- Is Persistenct Discovery Controller enabled
 .SH SYNOPSIS
 .B "bool" nvme_host_is_pdc_enabled
 .BI "(nvme_host_t h "  ","
 .BI "bool fallback "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_host_mem_buf_attrs.2` & `libnvme-1.5/doc/man/nvme_host_mem_buf_attrs.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_host_mem_buf_attrs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_host_mem_buf_attrs" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_host_mem_buf_attrs \- Host Memory Buffer - Attributes Data Structure
 .SH SYNOPSIS
 struct nvme_host_mem_buf_attrs {
 .br
 .BI "    __le32 hsize;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_host_metadata.2` & `libnvme-1.5/doc/man/nvme_host_metadata.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_host_metadata" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_host_metadata" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_host_metadata \- Host Metadata Data Structure
 .SH SYNOPSIS
 struct nvme_host_metadata {
 .br
 .BI "    __u8 ndesc;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_host_set_pdc_enabled.2` & `libnvme-1.5/doc/man/nvme_host_set_pdc_enabled.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_host_set_pdc_enabled" 9 "nvme_host_set_pdc_enabled" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_host_set_pdc_enabled" 9 "nvme_host_set_pdc_enabled" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_host_set_pdc_enabled \- Set Persistent Discovery Controller flag
 .SH SYNOPSIS
 .B "void" nvme_host_set_pdc_enabled
 .BI "(nvme_host_t h "  ","
 .BI "bool enabled "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl.2` & `libnvme-1.5/doc/man/nvme_id_ctrl.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ctrl" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ctrl" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ctrl \- Identify Controller data structure
 .SH SYNOPSIS
 struct nvme_id_ctrl {
 .br
 .BI "    __le16 vid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_anacap.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_anacap.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_anacap" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_anacap" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_anacap \- This field indicates the capabilities associated with Asymmetric Namespace Access Reporting.
 .SH SYNOPSIS
 enum nvme_id_ctrl_anacap {
 .br
 .BI "    NVME_CTRL_ANACAP_OPT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_cmic.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_cmic.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_cmic" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_cmic" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_cmic \- Controller Multipath IO and Namespace Sharing Capabilities of the controller and NVM subsystem.
 .SH SYNOPSIS
 enum nvme_id_ctrl_cmic {
 .br
 .BI "    NVME_CTRL_CMIC_MULTI_PORT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_cqes.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_cqes.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_cqes" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_cqes" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_cqes \- Defines the required and maximum Completion Queue entry size when using the NVM Command Set.
 .SH SYNOPSIS
 enum nvme_id_ctrl_cqes {
 .br
 .BI "    NVME_CTRL_CQES_MIN"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_ctratt.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_ctratt.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_ctratt" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_ctratt" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_ctratt \- Controller attributes
 .SH SYNOPSIS
 enum nvme_id_ctrl_ctratt {
 .br
 .BI "    NVME_CTRL_CTRATT_128_ID"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_dctype.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_dctype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_dctype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_dctype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_dctype \- Discovery Controller types
 .SH SYNOPSIS
 enum nvme_id_ctrl_dctype {
 .br
 .BI "    NVME_CTRL_DCTYPE_NOT_REPORTED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_fna.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_fna.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_fna" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_fna" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_fna \- This field indicates attributes for the Format NVM command.
 .SH SYNOPSIS
 enum nvme_id_ctrl_fna {
 .br
 .BI "    NVME_CTRL_FNA_FMT_ALL_NAMESPACES"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_frmw.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_frmw.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_frmw" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_frmw" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_frmw \- Flags and values indicates capabilities regarding firmware updates from &struct nvme_id_ctrl.frmw.
 .SH SYNOPSIS
 enum nvme_id_ctrl_frmw {
 .br
 .BI "    NVME_CTRL_FRMW_1ST_RO"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_lpa.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_lpa.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_lpa" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_lpa" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_lpa \- Flags indicating optional attributes for log pages that are accessed via the Get Log Page command.
 .SH SYNOPSIS
 enum nvme_id_ctrl_lpa {
 .br
 .BI "    NVME_CTRL_LPA_SMART_PER_NS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_mec.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_mec.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_mec" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_mec" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_mec \- Flags indicating the capabilities of the Management Endpoint in the Controller, &struct nvme_id_ctrl.mec.
 .SH SYNOPSIS
 enum nvme_id_ctrl_mec {
 .br
 .BI "    NVME_CTRL_MEC_SMBUSME"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_nvm.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ctrl_nvm" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ctrl_nvm" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ctrl_nvm \- I/O Command Set Specific Identify Controller data structure
 .SH SYNOPSIS
 struct nvme_id_ctrl_nvm {
 .br
 .BI "    __u8 vsl;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_nvmsr.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_nvmsr.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_nvmsr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_nvmsr" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_nvmsr \- This field reports information associated with the NVM Subsystem, see &struct nvme_id_ctrl.nvmsr.
 .SH SYNOPSIS
 enum nvme_id_ctrl_nvmsr {
 .br
 .BI "    NVME_CTRL_NVMSR_NVMESD"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_nwpc.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_nwpc.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_nwpc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_nwpc" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_nwpc \- This field indicates the optional namespace write protection capabilities supported by the controller.
 .SH SYNOPSIS
 enum nvme_id_ctrl_nwpc {
 .br
 .BI "    NVME_CTRL_NWPC_WRITE_PROTECT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_oacs.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_oacs.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oacs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oacs" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oacs \- Flags indicating the optional Admin commands and features supported by the controller, see &struct nvme_id_ctrl.oacs.
 .SH SYNOPSIS
 enum nvme_id_ctrl_oacs {
 .br
 .BI "    NVME_CTRL_OACS_SECURITY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_oaes.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_oaes.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oaes" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oaes" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oaes \- Optional Asynchronous Events Supported
 .SH SYNOPSIS
 enum nvme_id_ctrl_oaes {
 .br
 .BI "    NVME_CTRL_OAES_NA"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_oncs.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_oncs.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oncs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oncs" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oncs \- This field indicates the optional NVM commands and features supported by the controller.
 .SH SYNOPSIS
 enum nvme_id_ctrl_oncs {
 .br
 .BI "    NVME_CTRL_ONCS_COMPARE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_rpmbs.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_rpmbs.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_rpmbs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_rpmbs" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_rpmbs \- This field indicates if the controller supports one or more Replay Protected Memory Blocks, from &struct nvme_id_ctrl.rpmbs.
 .SH SYNOPSIS
 enum nvme_id_ctrl_rpmbs {
 .br
 .BI "    NVME_CTRL_RPMBS_NR_UNITS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_sanicap.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_sanicap.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sanicap" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sanicap" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sanicap \- Indicates attributes for sanitize operations.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sanicap {
 .br
 .BI "    NVME_CTRL_SANICAP_CES"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_sgls.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_sgls.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sgls" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sgls" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sgls \- This field indicates if SGLs are supported for the NVM Command Set and the particular SGL types supported.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sgls {
 .br
 .BI "    NVME_CTRL_SGLS_SUPPORTED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_sqes.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_sqes.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sqes" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sqes" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sqes \- Defines the required and maximum Submission Queue entry size when using the NVM Command Set.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sqes {
 .br
 .BI "    NVME_CTRL_SQES_MIN"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_vwc.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_vwc.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_vwc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_vwc" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_vwc \- Volatile write cache
 .SH SYNOPSIS
 enum nvme_id_ctrl_vwc {
 .br
 .BI "    NVME_CTRL_VWC_PRESENT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ctrl_vwci.2` & `libnvme-1.5/doc/man/nvme_id_ctrl_vwci.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_vwci" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_vwci" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_vwci \- This field indicates information about remaining number of times that VPD contents are able to be updated using the VPD Write command, see &struct nvme_id_ctrl.vwci.
 .SH SYNOPSIS
 enum nvme_id_ctrl_vwci {
 .br
 .BI "    NVME_CTRL_VWCI_VWCR"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_domain_attr.2` & `libnvme-1.5/doc/man/nvme_id_domain_attr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_domain_attr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_domain_attr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_domain_attr \- Domain Attributes Entry
 .SH SYNOPSIS
 struct nvme_id_domain_attr {
 .br
 .BI "    __le16 dom_id;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_independent_id_ns.2` & `libnvme-1.5/doc/man/nvme_id_independent_id_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_independent_id_ns" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_independent_id_ns" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_independent_id_ns \- Identify - I/O Command Set Independent Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_id_independent_id_ns {
 .br
 .BI "    __u8 nsfeat;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns.2` & `libnvme-1.5/doc/man/nvme_id_ns.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ns" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ns" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ns \- Identify Namespace data structure
 .SH SYNOPSIS
 struct nvme_id_ns {
 .br
 .BI "    __le64 nsze;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_dlfeat.2` & `libnvme-1.5/doc/man/nvme_id_ns_dlfeat.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dlfeat" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dlfeat" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dlfeat \- This field indicates information about features that affect deallocating logical blocks for this namespace.
 .SH SYNOPSIS
 enum nvme_id_ns_dlfeat {
 .br
 .BI "    NVME_NS_DLFEAT_RB"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_dpc.2` & `libnvme-1.5/doc/man/nvme_id_ns_dpc.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dpc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dpc" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dpc \- This field indicates the capabilities for the end-to-end data protection feature.
 .SH SYNOPSIS
 enum nvme_id_ns_dpc {
 .br
 .BI "    NVME_NS_DPC_PI_TYPE1"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_dps.2` & `libnvme-1.5/doc/man/nvme_id_ns_dps.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dps" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dps" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dps \- This field indicates the Type settings for the end-to-end data protection feature.
 .SH SYNOPSIS
 enum nvme_id_ns_dps {
 .br
 .BI "    NVME_NS_DPS_PI_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_flbas.2` & `libnvme-1.5/doc/man/nvme_id_ns_flbas.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_flbas" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_flbas" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_flbas \- This field indicates the LBA data size & metadata size combination that the namespace has been formatted with
 .SH SYNOPSIS
 enum nvme_id_ns_flbas {
 .br
 .BI "    NVME_NS_FLBAS_LOWER_MASK"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_granularity_list.2` & `libnvme-1.5/doc/man/nvme_id_ns_granularity_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ns_granularity_list" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ns_granularity_list" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ns_granularity_list \- Namespace Granularity List
 .SH SYNOPSIS
 struct nvme_id_ns_granularity_list {
 .br
 .BI "    __le32 attributes;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_mc.2` & `libnvme-1.5/doc/man/nvme_id_ns_mc.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_mc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_mc" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_mc \- This field indicates the capabilities for metadata.
 .SH SYNOPSIS
 enum nvme_id_ns_mc {
 .br
 .BI "    NVME_NS_MC_EXTENDED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_ns_rescap.2` & `libnvme-1.5/doc/man/nvme_id_ns_rescap.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_rescap" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_rescap" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_rescap \- This field indicates the reservation capabilities of the namespace.
 .SH SYNOPSIS
 enum nvme_id_ns_rescap {
 .br
 .BI "    NVME_NS_RESCAP_PTPL"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_nsfeat.2` & `libnvme-1.5/doc/man/nvme_id_nsfeat.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_nsfeat" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_nsfeat" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_nsfeat \- This field defines features of the namespace.
 .SH SYNOPSIS
 enum nvme_id_nsfeat {
 .br
 .BI "    NVME_NS_FEAT_THIN"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_id_psd.2` & `libnvme-1.5/doc/man/nvme_id_psd.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_psd" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_psd" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_id_psd \- Power Management data structure
 .SH SYNOPSIS
 struct nvme_id_psd {
 .br
 .BI "    __le16 mp;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_id_uuid.2` & `libnvme-1.5/doc/man/nvme_id_uuid.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_uuid" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_uuid" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_id_uuid \- Identifier Association
 .SH SYNOPSIS
 enum nvme_id_uuid {
 .br
 .BI "    NVME_ID_UUID_HDR_ASSOCIATION_MASK"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_identify.2` & `libnvme-1.5/doc/man/nvme_identify.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify" 9 "nvme_identify" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify" 9 "nvme_identify" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify \- Send the NVMe Identify command
 .SH SYNOPSIS
 .B "int" nvme_identify
 .BI "(struct nvme_identify_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_active_ns_list.2` & `libnvme-1.5/doc/man/nvme_identify_active_ns_list.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_active_ns_list" 9 "nvme_identify_active_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_active_ns_list" 9 "nvme_identify_active_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_active_ns_list \- Retrieves active namespaces id list
 .SH SYNOPSIS
 .B "int" nvme_identify_active_ns_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_active_ns_list_csi.2` & `libnvme-1.5/doc/man/nvme_identify_active_ns_list_csi.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_active_ns_list_csi" 9 "nvme_identify_active_ns_list_csi" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_active_ns_list_csi" 9 "nvme_identify_active_ns_list_csi" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_active_ns_list_csi \- Active namespace ID list associated with a specified I/O command set
 .SH SYNOPSIS
 .B "int" nvme_identify_active_ns_list_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "enum nvme_csi csi "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_allocated_ns.2` & `libnvme-1.5/doc/man/nvme_identify_allocated_ns.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns" 9 "nvme_identify_allocated_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns" 9 "nvme_identify_allocated_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns \- Same as nvme_identify_ns, but only for allocated namespaces
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_allocated_ns_list.2` & `libnvme-1.5/doc/man/nvme_identify_allocated_ns_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns_list" 9 "nvme_identify_allocated_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns_list" 9 "nvme_identify_allocated_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns_list \- Retrieves allocated namespace id list
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_allocated_ns_list_csi.2` & `libnvme-1.5/doc/man/nvme_identify_allocated_ns_list_csi.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns_list_csi" 9 "nvme_identify_allocated_ns_list_csi" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns_list_csi" 9 "nvme_identify_allocated_ns_list_csi" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns_list_csi \- Allocated namespace ID list associated with a specified I/O command set
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns_list_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "enum nvme_csi csi "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_cns.2` & `libnvme-1.5/doc/man/nvme_identify_cns.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_identify_cns" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_identify_cns" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_identify_cns \- Identify - CNS Values
 .SH SYNOPSIS
 enum nvme_identify_cns {
 .br
 .BI "    NVME_IDENTIFY_CNS_NS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ctrl.2` & `libnvme-1.5/doc/man/nvme_identify_ctrl.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl" 9 "nvme_identify_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl" 9 "nvme_identify_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl \- Retrieves nvme identify controller
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ctrl_csi.2` & `libnvme-1.5/doc/man/nvme_identify_ctrl_csi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl_csi" 9 "nvme_identify_ctrl_csi" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl_csi" 9 "nvme_identify_ctrl_csi" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl_csi \- I/O command set specific Identify Controller data
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl_csi
 .BI "(int fd "  ","
 .BI "enum nvme_csi csi "  ","
 .BI "void *data "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_identify_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl_list" 9 "nvme_identify_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl_list" 9 "nvme_identify_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl_list \- Retrieves identify controller list
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl_list
 .BI "(int fd "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_ctrl_list *cntlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_domain_list.2` & `libnvme-1.5/doc/man/nvme_identify_domain_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_domain_list" 9 "nvme_identify_domain_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_domain_list" 9 "nvme_identify_domain_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_domain_list \- Domain list data
 .SH SYNOPSIS
 .B "int" nvme_identify_domain_list
 .BI "(int fd "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_id_domain_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_endurance_group_list.2` & `libnvme-1.5/doc/man/nvme_identify_endurance_group_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_endurance_group_list" 9 "nvme_identify_endurance_group_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_endurance_group_list" 9 "nvme_identify_endurance_group_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_endurance_group_list \- Endurance group list data
 .SH SYNOPSIS
 .B "int" nvme_identify_endurance_group_list
 .BI "(int fd "  ","
 .BI "__u16 endgrp_id "  ","
 .BI "struct nvme_id_endurance_group_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_independent_identify_ns.2` & `libnvme-1.5/doc/man/nvme_identify_independent_identify_ns.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_independent_identify_ns" 9 "nvme_identify_independent_identify_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_independent_identify_ns" 9 "nvme_identify_independent_identify_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_independent_identify_ns \- I/O command set independent Identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_identify_independent_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_independent_id_ns *ns "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_iocs.2` & `libnvme-1.5/doc/man/nvme_identify_iocs.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_iocs" 9 "nvme_identify_iocs" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_iocs" 9 "nvme_identify_iocs" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_iocs \- I/O command set data structure
 .SH SYNOPSIS
 .B "int" nvme_identify_iocs
 .BI "(int fd "  ","
 .BI "__u16 cntlid "  ","
 .BI "struct nvme_id_iocs *iocs "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2` & `libnvme-1.5/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_iocs_ns_csi_user_data_format" 9 "nvme_identify_iocs_ns_csi_user_data_format" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_iocs_ns_csi_user_data_format" 9 "nvme_identify_iocs_ns_csi_user_data_format" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_iocs_ns_csi_user_data_format \- Identify I/O command set namespace data structure
 .SH SYNOPSIS
 .B "int" nvme_identify_iocs_ns_csi_user_data_format
 .BI "(int fd "  ","
 .BI "__u16 user_data_format "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ns.2` & `libnvme-1.5/doc/man/nvme_identify_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns" 9 "nvme_identify_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ns" 9 "nvme_identify_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns \- Retrieves nvme identify namespace
 .SH SYNOPSIS
 .B "int" nvme_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ns_csi.2` & `libnvme-1.5/doc/man/nvme_identify_ns_csi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_csi" 9 "nvme_identify_ns_csi" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_csi" 9 "nvme_identify_ns_csi" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_csi \- I/O command set specific identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ns_csi_user_data_format.2` & `libnvme-1.5/doc/man/nvme_identify_ns_csi_user_data_format.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_csi_user_data_format" 9 "nvme_identify_ns_csi_user_data_format" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_csi_user_data_format" 9 "nvme_identify_ns_csi_user_data_format" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_csi_user_data_format \- Identify namespace user data format
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_csi_user_data_format
 .BI "(int fd "  ","
 .BI "__u16 user_data_format "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ns_descs.2` & `libnvme-1.5/doc/man/nvme_identify_ns_descs.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_descs" 9 "nvme_identify_ns_descs" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_descs" 9 "nvme_identify_ns_descs" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_descs \- Retrieves namespace descriptor list
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_descs
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_id_desc *descs "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_ns_granularity.2` & `libnvme-1.5/doc/man/nvme_identify_ns_granularity.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_granularity" 9 "nvme_identify_ns_granularity" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_granularity" 9 "nvme_identify_ns_granularity" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_granularity \- Retrieves namespace granularity identification
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_granularity
 .BI "(int fd "  ","
 .BI "struct nvme_id_ns_granularity_list *gr_list "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_nsid_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_identify_nsid_ctrl_list.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_nsid_ctrl_list" 9 "nvme_identify_nsid_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_nsid_ctrl_list" 9 "nvme_identify_nsid_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_nsid_ctrl_list \- Retrieves controller list attached to an nsid
 .SH SYNOPSIS
 .B "int" nvme_identify_nsid_ctrl_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 cntid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_nvmset_list.2` & `libnvme-1.5/doc/man/nvme_identify_nvmset_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_nvmset_list" 9 "nvme_identify_nvmset_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_nvmset_list" 9 "nvme_identify_nvmset_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_nvmset_list \- Retrieves NVM Set List
 .SH SYNOPSIS
 .B "int" nvme_identify_nvmset_list
 .BI "(int fd "  ","
 .BI "__u16 nvmsetid "  ","
 .BI "struct nvme_id_nvmset_list *nvmset "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_primary_ctrl.2` & `libnvme-1.5/doc/man/nvme_identify_primary_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_primary_ctrl" 9 "nvme_identify_primary_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_primary_ctrl" 9 "nvme_identify_primary_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_primary_ctrl \- Retrieve NVMe Primary Controller identification
 .SH SYNOPSIS
 .B "int" nvme_identify_primary_ctrl
 .BI "(int fd "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_primary_ctrl_cap *cap "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_secondary_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_identify_secondary_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_secondary_ctrl_list" 9 "nvme_identify_secondary_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_secondary_ctrl_list" 9 "nvme_identify_secondary_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_secondary_ctrl_list \- Retrieves secondary controller list
 .SH SYNOPSIS
 .B "int" nvme_identify_secondary_ctrl_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 cntid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_identify_uuid.2` & `libnvme-1.5/doc/man/nvme_identify_uuid.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_uuid" 9 "nvme_identify_uuid" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_identify_uuid" 9 "nvme_identify_uuid" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_uuid \- Retrieves device's UUIDs
 .SH SYNOPSIS
 .B "int" nvme_identify_uuid
 .BI "(int fd "  ","
 .BI "struct nvme_id_uuid_list *uuid_list "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_init_copy_range.2` & `libnvme-1.5/doc/man/nvme_init_copy_range.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range" 9 "nvme_init_copy_range" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range" 9 "nvme_init_copy_range" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range \- Constructs a copy range structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range
 .BI "(struct nvme_copy_range *copy "  ","
 .BI "__u16 *nlbs "  ","
 .BI "__u64 *slbas "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_init_copy_range_f1.2` & `libnvme-1.5/doc/man/nvme_init_copy_range_f1.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range_f1" 9 "nvme_init_copy_range_f1" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range_f1" 9 "nvme_init_copy_range_f1" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range_f1 \- Constructs a copy range f1 structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range_f1
 .BI "(struct nvme_copy_range_f1 *copy "  ","
 .BI "__u16 *nlbs "  ","
 .BI "__u64 *slbas "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_init_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_init_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_ctrl_list" 9 "nvme_init_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_init_ctrl_list" 9 "nvme_init_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_ctrl_list \- Initialize an nvme_ctrl_list structure from an array.
 .SH SYNOPSIS
 .B "void" nvme_init_ctrl_list
 .BI "(struct nvme_ctrl_list *cntlist "  ","
 .BI "__u16 num_ctrls "  ","
 .BI "__u16 *ctrlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_init_dsm_range.2` & `libnvme-1.5/doc/man/nvme_init_dsm_range.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_dsm_range" 9 "nvme_init_dsm_range" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_init_dsm_range" 9 "nvme_init_dsm_range" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_dsm_range \- Constructs a data set range structure
 .SH SYNOPSIS
 .B "void" nvme_init_dsm_range
 .BI "(struct nvme_dsm_range *dsm "  ","
 .BI "__u32 *ctx_attrs "  ","
 .BI "__u32 *llbas "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_init_logging.2` & `libnvme-1.5/doc/man/nvme_init_logging.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_logging" 9 "nvme_init_logging" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_init_logging" 9 "nvme_init_logging" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_logging \- Initialize logging
 .SH SYNOPSIS
 .B "void" nvme_init_logging
 .BI "(nvme_root_t r "  ","
 .BI "int lvl "  ","
 .BI "bool log_pid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_insert_tls_key.2` & `libnvme-1.5/doc/man/nvme_insert_tls_key.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_insert_tls_key" 9 "nvme_insert_tls_key" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_insert_tls_key" 9 "nvme_insert_tls_key" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_insert_tls_key \- Derive and insert TLS key
 .SH SYNOPSIS
 .B "long" nvme_insert_tls_key
 .BI "(const char *keyring "  ","
 .BI "const char *key_type "  ","
 .BI "const char *hostnqn "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_io_control_flags.2` & `libnvme-1.5/doc/man/nvme_io_control_flags.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_control_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_control_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_io_control_flags \- I/O control flags
 .SH SYNOPSIS
 enum nvme_io_control_flags {
 .br
 .BI "    NVME_IO_DTYPE_STREAMS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_io_dsm_flags.2` & `libnvme-1.5/doc/man/nvme_io_dsm_flags.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_dsm_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_dsm_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_io_dsm_flags \- Dataset Management flags
 .SH SYNOPSIS
 enum nvme_io_dsm_flags {
 .br
 .BI "    NVME_IO_DSM_FREQ_UNSPEC"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_io_opcode.2` & `libnvme-1.5/doc/man/nvme_io_opcode.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_opcode" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_opcode" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_io_opcode \- Opcodes for I/O Commands
 .SH SYNOPSIS
 enum nvme_io_opcode {
 .br
 .BI "    nvme_cmd_flush"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_io_passthru.2` & `libnvme-1.5/doc/man/nvme_io_passthru.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_io_passthru" 9 "nvme_io_passthru" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_io_passthru" 9 "nvme_io_passthru" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_io_passthru \- Submit an nvme io passthrough command
 .SH SYNOPSIS
 .B "int" nvme_io_passthru
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_io_passthru64.2` & `libnvme-1.5/doc/man/nvme_admin_passthru64.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_io_passthru64" 9 "nvme_io_passthru64" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_admin_passthru64" 9 "nvme_admin_passthru64" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_io_passthru64 \- Submit an nvme io passthrough command
+nvme_admin_passthru64 \- Submit a 64-bit nvme passthrough command
 .SH SYNOPSIS
-.B "int" nvme_io_passthru64
+.B "int" nvme_admin_passthru64
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_io_passthru64\fP. This sets up and submits
-a \fIstruct nvme_passthru_cmd64\fP.
+Parameterized form of \fBnvme_submit_admin_passthru64\fP. This sets up and
+submits a \fIstruct nvme_passthru_cmd64\fP.
 
-Known values for \fIopcode\fP are defined in \fIenum nvme_io_opcode\fP.
+Known values for \fIopcode\fP are defined in \fIenum nvme_admin_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_is_64bit_reg.2` & `libnvme-1.5/doc/man/nvme_is_64bit_reg.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_is_64bit_reg" 9 "nvme_is_64bit_reg" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_is_64bit_reg" 9 "nvme_is_64bit_reg" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_is_64bit_reg \- Checks if offset of the controller register is a know 64bit value.
 .SH SYNOPSIS
 .B "bool" nvme_is_64bit_reg
 .BI "(__u32 offset "  ");"
 .SH ARGUMENTS
 .IP "offset" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_lba_range_type_entry.2` & `libnvme-1.5/doc/man/nvme_lba_range_type_entry.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_range_type_entry" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_range_type_entry" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_range_type_entry \- LBA Range Type - Data Structure Entry
 .SH SYNOPSIS
 struct nvme_lba_range_type_entry {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_lba_status_desc.2` & `libnvme-1.5/doc/man/nvme_lba_status_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_status_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_status_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_status_desc \- LBA Status Descriptor Entry
 .SH SYNOPSIS
 struct nvme_lba_status_desc {
 .br
 .BI "    __le64 dslba;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_lba_status_log.2` & `libnvme-1.5/doc/man/nvme_lba_status_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_status_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_status_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_status_log \- LBA Status Information Log
 .SH SYNOPSIS
 struct nvme_lba_status_log {
 .br
 .BI "    __le32 lslplen;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_lbaf.2` & `libnvme-1.5/doc/man/nvme_lbaf.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lbaf" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lbaf" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_lbaf \- LBA Format Data Structure
 .SH SYNOPSIS
 struct nvme_lbaf {
 .br
 .BI "    __le16 ms;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_lbaf_rp.2` & `libnvme-1.5/doc/man/nvme_lbaf_rp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_lbaf_rp" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_lbaf_rp" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_lbaf_rp \- This field indicates the relative performance of the LBA format indicated relative to other LBA formats supported by the controller.
 .SH SYNOPSIS
 enum nvme_lbaf_rp {
 .br
 .BI "    NVME_LBAF_RP_BEST"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_lbart.2` & `libnvme-1.5/doc/man/nvme_lbart.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_lbart" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_lbart" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_lbart \- LBA Range Type - Data Structure Entry
 .SH SYNOPSIS
 enum nvme_lbart {
 .br
 .BI "    NVME_LBART_TYPE_GP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_lbas_ns_element.2` & `libnvme-1.5/doc/man/nvme_mi_nvm_ss_health_status.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-.TH "libnvme" 9 "struct nvme_lbas_ns_element" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_nvm_ss_health_status" "June 2023" "API Manual" LINUX
 .SH NAME
-struct nvme_lbas_ns_element \- LBA Status Log Namespace Element
+struct nvme_mi_nvm_ss_health_status \- Subsystem Management Data Structure
 .SH SYNOPSIS
-struct nvme_lbas_ns_element {
+struct nvme_mi_nvm_ss_health_status {
 .br
-.BI "    __le32 neid;"
+.BI "    __u8 nss;"
 .br
-.BI "    __le32 nlrd;"
+.BI "    __u8 sw;"
 .br
-.BI "    __u8 ratype;"
+.BI "    __u8 ctemp;"
 .br
-.BI "    __u8 rsvd8[7];"
+.BI "    __u8 pdlu;"
 .br
-.BI "    struct nvme_lba_rd lba_rd[];"
+.BI "    __le16 ccs;"
+.br
+.BI "    __u8 rsvd8[2];"
 .br
 .BI "
 };
 .br
 
 .SH Members
-.IP "neid" 12
-Namespace Element Identifier
-.IP "nlrd" 12
-Number of LBA Range Descriptors
-.IP "ratype" 12
-Recommended Action Type. see \fIenum\fP nvme_lba_status_atype
+.IP "nss" 12
+NVM Subsystem Status
+.IP "sw" 12
+Smart Warnings
+.IP "ctemp" 12
+Composite Temperature
+.IP "pdlu" 12
+Percentage Drive Life Used
+.IP "ccs" 12
+Composite Controller Status
 .IP "rsvd8" 12
 Reserved
-.IP "lba_rd" 12
-LBA Range Descriptor
```

### Comparing `libnvme-1.4/doc/man/nvme_lookup_ctrl.2` & `libnvme-1.5/doc/man/nvme_lookup_ctrl.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_ctrl" 9 "nvme_lookup_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_lookup_ctrl" 9 "nvme_lookup_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_ctrl \- Lookup nvme_ctrl_t object
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvme_lookup_ctrl
 .BI "(nvme_subsystem_t s "  ","
 .BI "const char *transport "  ","
 .BI "const char *traddr "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_lookup_host.2` & `libnvme-1.5/doc/man/nvme_lookup_host.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_host" 9 "nvme_lookup_host" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_lookup_host" 9 "nvme_lookup_host" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_host \- Lookup nvme_host_t object
 .SH SYNOPSIS
 .B "nvme_host_t" nvme_lookup_host
 .BI "(nvme_root_t r "  ","
 .BI "const char *hostnqn "  ","
 .BI "const char *hostid "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_lookup_subsystem.2` & `libnvme-1.5/doc/man/nvme_lookup_subsystem.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_subsystem" 9 "nvme_lookup_subsystem" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_lookup_subsystem" 9 "nvme_lookup_subsystem" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_subsystem \- Lookup nvme_subsystem_t object
 .SH SYNOPSIS
 .B "nvme_subsystem_t" nvme_lookup_subsystem
 .BI "(struct nvme_host *h "  ","
 .BI "const char *name "  ","
 .BI "const char *subsysnqn "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_media_unit_stat_desc.2` & `libnvme-1.5/doc/man/nvme_media_unit_stat_desc.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_media_unit_stat_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_media_unit_stat_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_media_unit_stat_desc \- Media Unit Status Descriptor
 .SH SYNOPSIS
 struct nvme_media_unit_stat_desc {
 .br
 .BI "    __le16 muid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_admin_passthru.2` & `libnvme-1.5/doc/man/nvme_mi_admin_admin_passthru.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_admin_passthru" 9 "nvme_mi_admin_admin_passthru" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_admin_passthru" 9 "nvme_mi_admin_admin_passthru" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_admin_passthru \- Submit an nvme admin passthrough command
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_admin_passthru
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_format_nvm.2` & `libnvme-1.5/doc/man/nvme_mi_admin_format_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_format_nvm" 9 "nvme_mi_admin_format_nvm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_format_nvm" 9 "nvme_mi_admin_format_nvm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_format_nvm \- Format NVMe namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_format_nvm
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_format_nvm_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_fw_commit.2` & `libnvme-1.5/doc/man/nvme_mi_admin_fw_commit.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_fw_commit" 9 "nvme_mi_admin_fw_commit" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_fw_commit" 9 "nvme_mi_admin_fw_commit" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_fw_commit \- Commit firmware using the specified action
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_fw_commit
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_fw_commit_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_fw_download.2` & `libnvme-1.5/doc/man/nvme_mi_admin_fw_download.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_fw_download" 9 "nvme_mi_admin_fw_download" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_fw_download" 9 "nvme_mi_admin_fw_download" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_fw_download \- Download part or all of a firmware image to the controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_fw_download
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_fw_download_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_features_data.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_features_data.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_features_data" 9 "nvme_mi_admin_get_features_data" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_features_data" 9 "nvme_mi_admin_get_features_data" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_features_data \- Helper function for &nvme_mi_admin_get_features()
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_features_data
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_page.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-.TH "nvme_mi_admin_get_log" 9 "nvme_mi_admin_get_log" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_page" 9 "nvme_mi_admin_get_log_page" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log \- Retrieve log page data from controller
+nvme_mi_admin_get_log_page \- Retrieve log page data from controller
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log
+.B "int" nvme_mi_admin_get_log_page
 .BI "(nvme_mi_ctrl_t ctrl "  ","
+.BI "__u32 xfer_len "  ","
 .BI "struct nvme_get_log_args *args "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
+.IP "xfer_len" 12
+The chunk size of the read
 .IP "args" 12
 Get Log Page command arguments
 .SH "DESCRIPTION"
 Performs a Get Log Page Admin command as specified by \fIargs\fP. Response data
 is stored in \fIargs->data\fP, which should be a buffer of \fIargs->data_len\fP bytes.
 Resulting data length is stored in \fIargs->data_len\fP on successful
 command completion.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_ana.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_ana.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_ana" 9 "nvme_mi_admin_get_log_ana" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_ana" 9 "nvme_mi_admin_get_log_ana" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_ana \- Retrieve Asymmetric Namespace Access log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_ana
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_log_ana_lsp lsp "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_ana_groups.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_ana_groups.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_ana_groups" 9 "nvme_mi_admin_get_log_ana_groups" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_ana_groups" 9 "nvme_mi_admin_get_log_ana_groups" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_ana_groups \- Retrieve Asymmetric Namespace Access groups only log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_ana_groups
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_changed_ns_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_changed_ns_list.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_changed_ns_list" 9 "nvme_mi_admin_get_log_changed_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_changed_ns_list" 9 "nvme_mi_admin_get_log_changed_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_changed_ns_list \- Retrieve namespace changed list
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_changed_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_ns_list *ns_log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_cmd_effects.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_cmd_effects.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_cmd_effects" 9 "nvme_mi_admin_get_log_cmd_effects" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_cmd_effects" 9 "nvme_mi_admin_get_log_cmd_effects" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_cmd_effects \- Retrieve nvme command effects log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_cmd_effects
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_csi csi "  ","
 .BI "struct nvme_cmd_effects_log *effects_log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_create_telemetry_host" 9 "nvme_mi_admin_get_log_create_telemetry_host" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_create_telemetry_host" 9 "nvme_mi_admin_get_log_create_telemetry_host" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_create_telemetry_host \- Create host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_create_telemetry_host
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_telemetry_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_device_self_test.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_device_self_test.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_device_self_test" 9 "nvme_mi_admin_get_log_device_self_test" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_device_self_test" 9 "nvme_mi_admin_get_log_device_self_test" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_device_self_test \- Retrieve the device self test log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_device_self_test
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_self_test_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_endurance_group.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_endurance_group.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_endurance_group" 9 "nvme_mi_admin_get_log_endurance_group" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_endurance_group" 9 "nvme_mi_admin_get_log_endurance_group" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_endurance_group \- Get Endurance Group log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_endurance_group
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 endgid "  ","
 .BI "struct nvme_endurance_group_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_lba_status.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-.TH "nvme_mi_admin_get_log_endurance_grp_evt" 9 "nvme_mi_admin_get_log_endurance_grp_evt" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_lba_status" 9 "nvme_mi_admin_get_log_lba_status" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_endurance_grp_evt \- Retrieve Rotational Media Information
+nvme_mi_admin_get_log_lba_status \- Retrieve LBA Status
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_endurance_grp_evt
+.B "int" nvme_mi_admin_get_log_lba_status
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
-.BI "__u32 offset "  ","
+.BI "__u64 offset "  ","
 .BI "__u32 len "  ","
 .BI "void *log "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
 .IP "rae" 12
 Retain asynchronous events
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_error.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_error.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_error" 9 "nvme_mi_admin_get_log_error" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_error" 9 "nvme_mi_admin_get_log_error" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_error \- Retrieve nvme error log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_error
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "unsigned int nr_entries "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_fid_supported_effects" 9 "nvme_mi_admin_get_log_fid_supported_effects" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_fid_supported_effects" 9 "nvme_mi_admin_get_log_fid_supported_effects" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_fid_supported_effects \- Retrieve Feature Identifiers Supported and Effects
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_fid_supported_effects
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_fid_supported_effects_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_fw_slot.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_fw_slot.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_fw_slot" 9 "nvme_mi_admin_get_log_fw_slot" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_fw_slot" 9 "nvme_mi_admin_get_log_fw_slot" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_fw_slot \- Retrieves the controller firmware log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_fw_slot
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_firmware_slot *fw_log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_lba_status.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_sanitize.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-.TH "nvme_mi_admin_get_log_lba_status" 9 "nvme_mi_admin_get_log_lba_status" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_sanitize" 9 "nvme_mi_admin_get_log_sanitize" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_lba_status \- Retrieve LBA Status
+nvme_mi_admin_get_log_sanitize \- Retrieve Sanitize Status
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_lba_status
+.B "int" nvme_mi_admin_get_log_sanitize
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
-.BI "__u64 offset "  ","
-.BI "__u32 len "  ","
-.BI "void *log "  ");"
+.BI "struct nvme_sanitize_log_page *log "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
 .IP "rae" 12
 Retain asynchronous events
-.IP "offset" 12
-Offset to the start of the log page
-.IP "len" 12
-The allocated length of the log page
 .IP "log" 12
-User address to store the log page
+User address to store the sanitize log
+.SH "DESCRIPTION"
+The Sanitize Status log page reports sanitize operation time estimates and
+information about the most recent sanitize operation.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_media_unit_stat.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_media_unit_stat.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_media_unit_stat" 9 "nvme_mi_admin_get_log_media_unit_stat" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_media_unit_stat" 9 "nvme_mi_admin_get_log_media_unit_stat" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_media_unit_stat \- Retrieve Media Unit Status
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_media_unit_stat
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_media_unit_stat_log *mus "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_mi_cmd_supported_effects" 9 "nvme_mi_admin_get_log_mi_cmd_supported_effects" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_mi_cmd_supported_effects" 9 "nvme_mi_admin_get_log_mi_cmd_supported_effects" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_mi_cmd_supported_effects \- displays the MI Commands Supported by the controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_mi_cmd_supported_effects
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_mi_cmd_supported_effects_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_page.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-.TH "nvme_mi_admin_get_log_page" 9 "nvme_mi_admin_get_log_page" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log" 9 "nvme_mi_admin_get_log" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_page \- Retrieve log page data from controller
+nvme_mi_admin_get_log \- Retrieve log page data from controller
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_page
+.B "int" nvme_mi_admin_get_log
 .BI "(nvme_mi_ctrl_t ctrl "  ","
-.BI "__u32 xfer_len "  ","
 .BI "struct nvme_get_log_args *args "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
-.IP "xfer_len" 12
-The chunk size of the read
 .IP "args" 12
 Get Log Page command arguments
 .SH "DESCRIPTION"
 Performs a Get Log Page Admin command as specified by \fIargs\fP. Response data
 is stored in \fIargs->data\fP, which should be a buffer of \fIargs->data_len\fP bytes.
 Resulting data length is stored in \fIargs->data_len\fP on successful
 command completion.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_persistent_event.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_persistent_event.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_persistent_event" 9 "nvme_mi_admin_get_log_persistent_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_persistent_event" 9 "nvme_mi_admin_get_log_persistent_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_persistent_event \- Retrieve Persistent Event Log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_persistent_event
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_pevent_log_action action "  ","
 .BI "__u32 size "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_predictable_lat_event" 9 "nvme_mi_admin_get_log_predictable_lat_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_predictable_lat_event" 9 "nvme_mi_admin_get_log_predictable_lat_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_predictable_lat_event \- Retrieve Predictable Latency Event Aggregate Log Page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_predictable_lat_event
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_predictable_lat_nvmset" 9 "nvme_mi_admin_get_log_predictable_lat_nvmset" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_predictable_lat_nvmset" 9 "nvme_mi_admin_get_log_predictable_lat_nvmset" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_predictable_lat_nvmset \- Predictable Latency Per NVM Set
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_predictable_lat_nvmset
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 nvmsetid "  ","
 .BI "struct nvme_nvmset_predictable_lat_log *log "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_sanitize.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-.TH "nvme_mi_admin_get_log_sanitize" 9 "nvme_mi_admin_get_log_sanitize" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_telemetry_ctrl" 9 "nvme_mi_admin_get_log_telemetry_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_sanitize \- Retrieve Sanitize Status
+nvme_mi_admin_get_log_telemetry_ctrl \- Get Telemetry Controller-Initiated log page
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_sanitize
+.B "int" nvme_mi_admin_get_log_telemetry_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
-.BI "struct nvme_sanitize_log_page *log "  ");"
+.BI "__u64 offset "  ","
+.BI "__u32 len "  ","
+.BI "void *log "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
 .IP "rae" 12
 Retain asynchronous events
+.IP "offset" 12
+Offset into the telemetry data
+.IP "len" 12
+Length of provided user buffer to hold the log data in bytes
 .IP "log" 12
-User address to store the sanitize log
+User address for log page data
 .SH "DESCRIPTION"
-The Sanitize Status log page reports sanitize operation time estimates and
-information about the most recent sanitize operation.
+Retrieves the Telemetry Controller-Initiated log page at the requested offset
+using the previously existing capture.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_simple.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_simple.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_simple" 9 "nvme_mi_admin_get_log_simple" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_simple" 9 "nvme_mi_admin_get_log_simple" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_simple \- Helper for Get Log Page functions with no NSID or RAE requirements
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_simple
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_cmd_get_log_lid lid "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_smart.2` & `libnvme-1.5/doc/man/nvme_get_log_smart.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-.TH "nvme_mi_admin_get_log_smart" 9 "nvme_mi_admin_get_log_smart" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_log_smart" 9 "nvme_get_log_smart" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_smart \- Retrieve nvme smart log
+nvme_get_log_smart \- Retrieve nvme smart log
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_smart
-.BI "(nvme_mi_ctrl_t ctrl "  ","
+.B "int" nvme_get_log_smart
+.BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_smart_log *smart_log "  ");"
 .SH ARGUMENTS
-.IP "ctrl" 12
-Controller to query
+.IP "fd" 12
+File descriptor of nvme device
 .IP "nsid" 12
 Optional namespace identifier
 .IP "rae" 12
 Retain asynchronous events
 .IP "smart_log" 12
 User address to store the smart log
 .SH "DESCRIPTION"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_support_cap_config_list" 9 "nvme_mi_admin_get_log_support_cap_config_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_support_cap_config_list" 9 "nvme_mi_admin_get_log_support_cap_config_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_support_cap_config_list \- Retrieve Supported Capacity Configuration List
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_support_cap_config_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_supported_cap_config_list_log *cap "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_ns_descs.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-.TH "nvme_mi_admin_get_log_telemetry_ctrl" 9 "nvme_mi_admin_get_log_telemetry_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ns_descs" 9 "nvme_mi_admin_identify_ns_descs" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_telemetry_ctrl \- Get Telemetry Controller-Initiated log page
+nvme_mi_admin_identify_ns_descs \- Perform an Admin identify Namespace Identification Descriptor list command for a namespace
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_telemetry_ctrl
+.B "int" nvme_mi_admin_identify_ns_descs
 .BI "(nvme_mi_ctrl_t ctrl "  ","
-.BI "bool rae "  ","
-.BI "__u64 offset "  ","
-.BI "__u32 len "  ","
-.BI "void *log "  ");"
+.BI "__u32 nsid "  ","
+.BI "struct nvme_ns_id_desc *descs "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
-Controller to query
-.IP "rae" 12
-Retain asynchronous events
-.IP "offset" 12
-Offset into the telemetry data
-.IP "len" 12
-Length of provided user buffer to hold the log data in bytes
-.IP "log" 12
-User address for log page data
+Controller to process identify command
+.IP "nsid" 12
+Namespace ID
+.IP "descs" 12
+Namespace Identification Descriptor list to populate
 .SH "DESCRIPTION"
-Retrieves the Telemetry Controller-Initiated log page at the requested offset
-using the previously existing capture.
+Perform an Identify namespace identification description list command,
+setting the namespace identification description list in \fIdescs\fP
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_telemetry_host.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_telemetry_host.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_telemetry_host" 9 "nvme_mi_admin_get_log_telemetry_host" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_telemetry_host" 9 "nvme_mi_admin_get_log_telemetry_host" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_telemetry_host \- Get Telemetry Host-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_telemetry_host
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u64 offset "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_zns_changed_zones" 9 "nvme_mi_admin_get_log_zns_changed_zones" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_zns_changed_zones" 9 "nvme_mi_admin_get_log_zns_changed_zones" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_zns_changed_zones \- Retrieve list of zones that have changed
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_zns_changed_zones
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_get_nsid_log.2` & `libnvme-1.5/doc/man/nvme_mi_admin_get_nsid_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_nsid_log" 9 "nvme_mi_admin_get_nsid_log" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_nsid_log" 9 "nvme_mi_admin_get_nsid_log" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_nsid_log \- Helper for Get Log Page functions
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_nsid_log
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "enum nvme_cmd_get_log_lid lid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify" 9 "nvme_mi_admin_identify" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify" 9 "nvme_mi_admin_identify" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify \- Perform an Admin identify command.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_identify_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_active_ns_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_allocated_ns_list.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_mi_admin_identify_active_ns_list" 9 "nvme_mi_admin_identify_active_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_allocated_ns_list" 9 "nvme_mi_admin_identify_allocated_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_identify_active_ns_list \- Perform an Admin identify for an active namespace list
+nvme_mi_admin_identify_allocated_ns_list \- Perform an Admin identify for an allocated namespace list
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_identify_active_ns_list
+.B "int" nvme_mi_admin_identify_allocated_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to process identify command
 .IP "nsid" 12
 Namespace ID to specify list start
 .IP "list" 12
 List data to populate
 .SH "DESCRIPTION"
-Perform an Identify command, for the active namespace list starting with
+Perform an Identify command, for the allocated namespace list starting with
 IDs greater than or equal to \fInsid\fP. Specify \fINVME_NSID_NONE\fP for the start
 of the list.
 
 Will return an error if the length of the response data (from the
 controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIlist\fP will be
 be fully populated on success.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_allocated_ns.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_allocated_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_allocated_ns" 9 "nvme_mi_admin_identify_allocated_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_allocated_ns" 9 "nvme_mi_admin_identify_allocated_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_allocated_ns \- Perform an Admin identify command for an allocated namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_allocated_ns
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_allocated_ns_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_active_ns_list.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_mi_admin_identify_allocated_ns_list" 9 "nvme_mi_admin_identify_allocated_ns_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_active_ns_list" 9 "nvme_mi_admin_identify_active_ns_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_identify_allocated_ns_list \- Perform an Admin identify for an allocated namespace list
+nvme_mi_admin_identify_active_ns_list \- Perform an Admin identify for an active namespace list
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_identify_allocated_ns_list
+.B "int" nvme_mi_admin_identify_active_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to process identify command
 .IP "nsid" 12
 Namespace ID to specify list start
 .IP "list" 12
 List data to populate
 .SH "DESCRIPTION"
-Perform an Identify command, for the allocated namespace list starting with
+Perform an Identify command, for the active namespace list starting with
 IDs greater than or equal to \fInsid\fP. Specify \fINVME_NSID_NONE\fP for the start
 of the list.
 
 Will return an error if the length of the response data (from the
 controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIlist\fP will be
 be fully populated on success.
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_cns_nsid.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_cns_nsid.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_cns_nsid" 9 "nvme_mi_admin_identify_cns_nsid" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_cns_nsid" 9 "nvme_mi_admin_identify_cns_nsid" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_cns_nsid \- Perform an Admin identify command using specific CNS/NSID parameters.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_cns_nsid
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_identify_cns cns "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_ctrl.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ctrl" 9 "nvme_mi_admin_identify_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ctrl" 9 "nvme_mi_admin_identify_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ctrl \- Perform an Admin identify for a controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_ctrl_list.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ctrl_list" 9 "nvme_mi_admin_identify_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ctrl_list" 9 "nvme_mi_admin_identify_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ctrl_list \- Perform an Admin identify for a controller list.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ctrl_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_ctrl_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_ns.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_ns.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ns" 9 "nvme_mi_admin_identify_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ns" 9 "nvme_mi_admin_identify_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ns \- Perform an Admin identify command for a namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ns
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_nsid_ctrl_list" 9 "nvme_mi_admin_identify_nsid_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_nsid_ctrl_list" 9 "nvme_mi_admin_identify_nsid_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_nsid_ctrl_list \- Perform an Admin identify for a controller list with specific namespace ID
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_nsid_ctrl_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 cntid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_partial.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_partial.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_partial" 9 "nvme_mi_admin_identify_partial" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_partial" 9 "nvme_mi_admin_identify_partial" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_partial \- Perform an Admin identify command, and retrieve partial response data.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_partial
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_identify_args *args "  ","
 .BI "off_t offset "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_primary_ctrl.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_primary_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_primary_ctrl" 9 "nvme_mi_admin_identify_primary_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_primary_ctrl" 9 "nvme_mi_admin_identify_primary_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_primary_ctrl \- Perform an Admin identify for primary controller capabilities data structure.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_primary_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_primary_ctrl_cap *cap "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_secondary_ctrl_list" 9 "nvme_mi_admin_identify_secondary_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_secondary_ctrl_list" 9 "nvme_mi_admin_identify_secondary_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_secondary_ctrl_list \- Perform an Admin identify for a secondary controller list.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_secondary_ctrl_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 cntid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_ns_attach.2` & `libnvme-1.5/doc/man/nvme_mi_admin_ns_attach.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_attach" 9 "nvme_mi_admin_ns_attach" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_attach" 9 "nvme_mi_admin_ns_attach" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_attach \- Attach or detach namespace to controller(s)
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_attach
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_ns_attach_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_ns_attach_ctrls.2` & `libnvme-1.5/doc/man/nvme_mi_admin_ns_attach_ctrls.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_attach_ctrls" 9 "nvme_mi_admin_ns_attach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_attach_ctrls" 9 "nvme_mi_admin_ns_attach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_attach_ctrls \- Attach namespace to controllers
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_attach_ctrls
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_ns_detach_ctrls.2` & `libnvme-1.5/doc/man/nvme_mi_admin_ns_detach_ctrls.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_detach_ctrls" 9 "nvme_mi_admin_ns_detach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_detach_ctrls" 9 "nvme_mi_admin_ns_detach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_detach_ctrls \- Detach namespace from controllers
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_detach_ctrls
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_req_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_admin_req_hdr.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_admin_req_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_admin_req_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_admin_req_hdr \- Admin command request header.
 .SH SYNOPSIS
 struct nvme_mi_admin_req_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_resp_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_admin_resp_hdr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_admin_resp_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_admin_resp_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_admin_resp_hdr \- Admin command response header.
 .SH SYNOPSIS
 struct nvme_mi_admin_resp_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_sanitize_nvm.2` & `libnvme-1.5/doc/man/nvme_mi_admin_sanitize_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_sanitize_nvm" 9 "nvme_mi_admin_sanitize_nvm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_sanitize_nvm" 9 "nvme_mi_admin_sanitize_nvm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_sanitize_nvm \- Start a subsystem Sanitize operation
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_sanitize_nvm
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_sanitize_nvm_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_security_recv.2` & `libnvme-1.5/doc/man/nvme_mi_admin_security_recv.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_security_recv" 9 "nvme_mi_admin_security_recv" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_security_recv" 9 "nvme_mi_admin_security_recv" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_security_recv \- Perform a Security Receive command on a controller.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_security_recv
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_security_receive_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_security_send.2` & `libnvme-1.5/doc/man/nvme_mi_admin_security_send.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_security_send" 9 "nvme_mi_admin_security_send" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_security_send" 9 "nvme_mi_admin_security_send" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_security_send \- Perform a Security Send command on a controller.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_security_send
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_security_send_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_admin_xfer.2` & `libnvme-1.5/doc/man/nvme_mi_admin_xfer.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_xfer" 9 "nvme_mi_admin_xfer" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_xfer" 9 "nvme_mi_admin_xfer" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_xfer \- Raw admin transfer interface.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_xfer
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_mi_admin_req_hdr *admin_req "  ","
 .BI "size_t req_data_size "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_ccs.2` & `libnvme-1.5/doc/man/nvme_mi_ccs.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_ccs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_ccs" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_ccs \- Get State Control Primitive Success Response Fields - Control Primitive Specific Response
 .SH SYNOPSIS
 enum nvme_mi_ccs {
 .br
 .BI "    NVME_MI_CCS_RDY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_cmd_supported_effects.2` & `libnvme-1.5/doc/man/nvme_mi_cmd_supported_effects.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_cmd_supported_effects" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_cmd_supported_effects" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_cmd_supported_effects \- MI Command Supported and Effects Data Structure
 .SH SYNOPSIS
 enum nvme_mi_cmd_supported_effects {
 .br
 .BI "    NVME_MI_CMD_SUPPORTED_EFFECTS_CSUPP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_config_id.2` & `libnvme-1.5/doc/man/nvme_mi_config_id.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_config_id" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_config_id" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_config_id \- NVMe-MI Configuration identifier.
 .SH SYNOPSIS
 enum nvme_mi_config_id {
 .br
 .BI "    NVME_MI_CONFIG_SMBUS_FREQ"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_config_smbus_freq.2` & `libnvme-1.5/doc/man/nvme_mi_config_smbus_freq.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_config_smbus_freq" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_config_smbus_freq" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_config_smbus_freq \- SMBus/I2C frequency values
 .SH SYNOPSIS
 enum nvme_mi_config_smbus_freq {
 .br
 .BI "    NVME_MI_CONFIG_SMBUS_FREQ_100kHz"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_create_root.2` & `libnvme-1.5/doc/man/nvme_mi_create_root.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_create_root" 9 "nvme_mi_create_root" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_create_root" 9 "nvme_mi_create_root" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_create_root \- Create top-level MI (root) handle.
 .SH SYNOPSIS
 .B "nvme_root_t" nvme_mi_create_root
 .BI "(FILE *fp "  ","
 .BI "int log_level "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_csts.2` & `libnvme-1.5/doc/man/nvme_mi_csts.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_csts" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_csts" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_csts \- Controller Health Data Structure (CHDS) - Controller Status (CSTS)
 .SH SYNOPSIS
 enum nvme_mi_csts {
 .br
 .BI "    NVME_MI_CSTS_RDY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_ctrl_health_status.2` & `libnvme-1.5/doc/man/nvme_mi_ctrl_health_status.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_ctrl_health_status" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_ctrl_health_status" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_ctrl_health_status \- Controller Health Data Structure (CHDS)
 .SH SYNOPSIS
 struct nvme_mi_ctrl_health_status {
 .br
 .BI "    __le16 ctlid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_cwarn.2` & `libnvme-1.5/doc/man/nvme_mi_cwarn.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_cwarn" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_cwarn" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_cwarn \- Controller Health Data Structure (CHDS) - Critical Warning (CWARN)
 .SH SYNOPSIS
 enum nvme_mi_cwarn {
 .br
 .BI "    NVME_MI_CWARN_ST"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_dtyp.2` & `libnvme-1.5/doc/man/nvme_mi_dtyp.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_dtyp" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_dtyp" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_dtyp \- Data Structure Type field.
 .SH SYNOPSIS
 enum nvme_mi_dtyp {
 .br
 .BI "    nvme_mi_dtyp_subsys_info"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_elem.2` & `libnvme-1.5/doc/man/nvme_mi_elem.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_elem" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_elem" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_elem \- Element Descriptor Types
 .SH SYNOPSIS
 enum nvme_mi_elem {
 .br
 .BI "    NVME_MI_ELEM_EED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_init_ctrl.2` & `libnvme-1.5/doc/man/nvme_mi_init_ctrl.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_init_ctrl" 9 "nvme_mi_init_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_init_ctrl" 9 "nvme_mi_init_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_init_ctrl \- initialise a NVMe controller.
 .SH SYNOPSIS
 .B "nvme_mi_ctrl_t" nvme_mi_init_ctrl
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u16 ctrl_id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_message_type.2` & `libnvme-1.5/doc/man/nvme_mi_message_type.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_message_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_message_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_message_type \- NVMe-MI message type field.
 .SH SYNOPSIS
 enum nvme_mi_message_type {
 .br
 .BI "    NVME_MI_MT_CONTROL"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_opcode.2` & `libnvme-1.5/doc/man/nvme_mi_mi_opcode.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_mi_opcode" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_mi_opcode" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_mi_opcode \- Operation code for supported NVMe-MI commands.
 .SH SYNOPSIS
 enum nvme_mi_mi_opcode {
 .br
 .BI "    nvme_mi_mi_opcode_mi_data_read"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_ctrl.2` & `libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_ctrl" 9 "nvme_mi_mi_read_mi_data_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_ctrl" 9 "nvme_mi_mi_read_mi_data_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_ctrl \- Perform a Read MI Data Structure command, retrieving controller information
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_ctrl
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u16 ctrl_id "  ","
 .BI "struct nvme_mi_read_ctrl_info *ctrl "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2` & `libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_ctrl_list" 9 "nvme_mi_mi_read_mi_data_ctrl_list" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_ctrl_list" 9 "nvme_mi_mi_read_mi_data_ctrl_list" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_ctrl_list \- Perform a Read MI Data Structure command, retrieving the list of attached controllers.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_ctrl_list
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u8 start_ctrlid "  ","
 .BI "struct nvme_ctrl_list *list "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_port.2` & `libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_port.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_port" 9 "nvme_mi_mi_read_mi_data_port" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_port" 9 "nvme_mi_mi_read_mi_data_port" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_port \- Perform a Read MI Data Structure command, retrieving port data.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_port
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u8 portid "  ","
 .BI "struct nvme_mi_read_port_info *p "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_read_mi_data_subsys.2` & `libnvme-1.5/doc/man/nvme_mi_mi_read_mi_data_subsys.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_subsys" 9 "nvme_mi_mi_read_mi_data_subsys" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_subsys" 9 "nvme_mi_mi_read_mi_data_subsys" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_subsys \- Perform a Read MI Data Structure command, retrieving subsystem data.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_subsys
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "struct nvme_mi_read_nvm_ss_info *s "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_req_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_mi_req_hdr.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_mi_req_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_mi_req_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_mi_req_hdr \- MI request message header.
 .SH SYNOPSIS
 struct nvme_mi_mi_req_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_resp_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_mi_resp_hdr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_mi_resp_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_mi_resp_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_mi_resp_hdr \- MI response message header.
 .SH SYNOPSIS
 struct nvme_mi_mi_resp_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_mi_subsystem_health_status_poll.2` & `libnvme-1.5/doc/man/nvme_mi_mi_subsystem_health_status_poll.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_subsystem_health_status_poll" 9 "nvme_mi_mi_subsystem_health_status_poll" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_subsystem_health_status_poll" 9 "nvme_mi_mi_subsystem_health_status_poll" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_subsystem_health_status_poll \- Read the Subsystem Health Data Structure from the NVM subsystem
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_subsystem_health_status_poll
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "bool clear "  ","
 .BI "struct nvme_mi_nvm_ss_health_status *nshds "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_msg_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_msg_hdr.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_msg_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_msg_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_msg_hdr \- General MI message header.
 .SH SYNOPSIS
 struct nvme_mi_msg_hdr {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_msg_resp.2` & `libnvme-1.5/doc/man/nvme_mi_msg_resp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_msg_resp" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_msg_resp" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_msg_resp \- Generic response type.
 .SH SYNOPSIS
 struct nvme_mi_msg_resp {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_nvm_ss_health_status.2` & `libnvme-1.5/doc/man/nvme_mi_read_port_info.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-.TH "libnvme" 9 "struct nvme_mi_nvm_ss_health_status" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_read_port_info" "June 2023" "API Manual" LINUX
 .SH NAME
-struct nvme_mi_nvm_ss_health_status \- Subsystem Management Data Structure
+struct nvme_mi_read_port_info \- Port Information Data Structure
 .SH SYNOPSIS
-struct nvme_mi_nvm_ss_health_status {
+struct nvme_mi_read_port_info {
 .br
-.BI "    __u8 nss;"
+.BI "    __u8 portt;"
 .br
-.BI "    __u8 sw;"
+.BI "    __u8 rsvd1;"
 .br
-.BI "    __u8 ctemp;"
+.BI "    __le16 mmctptus;"
 .br
-.BI "    __u8 pdlu;"
+.BI "    __le32 meb;"
 .br
-.BI "    __le16 ccs;"
+.BI "    union {"
 .br
-.BI "    __u8 rsvd8[2];"
+.BI "      struct nvme_mi_port_pcie pcie;"
+.br
+.BI "      struct nvme_mi_port_smb smb;"
+.br
+.BI "    };"
 .br
 .BI "
 };
 .br
 
 .SH Members
-.IP "nss" 12
-NVM Subsystem Status
-.IP "sw" 12
-Smart Warnings
-.IP "ctemp" 12
-Composite Temperature
-.IP "pdlu" 12
-Percentage Drive Life Used
-.IP "ccs" 12
-Composite Controller Status
-.IP "rsvd8" 12
+.IP "portt" 12
+Port Type
+.IP "rsvd1" 12
 Reserved
+.IP "mmctptus" 12
+Maximum MCTP Transmission Unit Size
+.IP "meb" 12
+Management Endpoint Buffer Size
+.IP "{unnamed_union}" 12
+anonymous
+.IP "pcie" 12
+PCIe Port Specific Data
+.IP "smb" 12
+SMBus Port Specific Data
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_open_mctp.2` & `libnvme-1.5/doc/man/nvme_mi_open_mctp.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_open_mctp" 9 "nvme_mi_open_mctp" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_open_mctp" 9 "nvme_mi_open_mctp" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_open_mctp \- Create an endpoint using a MCTP connection.
 .SH SYNOPSIS
 .B "nvme_mi_ep_t" nvme_mi_open_mctp
 .BI "(nvme_root_t root "  ","
 .BI "unsigned int netid "  ","
 .BI "uint8_t eid "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_port_pcie.2` & `libnvme-1.5/doc/man/nvme_mi_port_pcie.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_port_pcie" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_port_pcie" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_port_pcie \- PCIe Port Specific Data
 .SH SYNOPSIS
 struct nvme_mi_port_pcie {
 .br
 .BI "    __u8 mps;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_port_smb.2` & `libnvme-1.5/doc/man/nvme_mi_port_smb.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_port_smb" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_port_smb" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_port_smb \- SMBus Port Specific Data
 .SH SYNOPSIS
 struct nvme_mi_port_smb {
 .br
 .BI "    __u8 vpd_addr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_read_ctrl_info.2` & `libnvme-1.5/doc/man/nvme_mi_read_ctrl_info.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_read_ctrl_info" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_read_ctrl_info" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_read_ctrl_info \- Controller Information Data Structure
 .SH SYNOPSIS
 struct nvme_mi_read_ctrl_info {
 .br
 .BI "    __u8 portid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_read_port_info.2` & `libnvme-1.5/doc/man/nvme_zns_desc.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-.TH "libnvme" 9 "struct nvme_mi_read_port_info" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_zns_desc" "June 2023" "API Manual" LINUX
 .SH NAME
-struct nvme_mi_read_port_info \- Port Information Data Structure
+struct nvme_zns_desc \- Zone Descriptor Data Structure
 .SH SYNOPSIS
-struct nvme_mi_read_port_info {
+struct nvme_zns_desc {
 .br
-.BI "    __u8 portt;"
+.BI "    __u8 zt;"
 .br
-.BI "    __u8 rsvd1;"
+.BI "    __u8 zs;"
 .br
-.BI "    __le16 mmctptus;"
+.BI "    __u8 za;"
 .br
-.BI "    __le32 meb;"
+.BI "    __u8 zai;"
 .br
-.BI "    union {"
+.BI "    __u8 rsvd4[4];"
 .br
-.BI "      struct nvme_mi_port_pcie pcie;"
+.BI "    __le64 zcap;"
 .br
-.BI "      struct nvme_mi_port_smb smb;"
+.BI "    __le64 zslba;"
 .br
-.BI "    };"
+.BI "    __le64 wp;"
+.br
+.BI "    __u8 rsvd32[32];"
 .br
 .BI "
 };
 .br
 
 .SH Members
-.IP "portt" 12
-Port Type
-.IP "rsvd1" 12
+.IP "zt" 12
+Zone Type
+.IP "zs" 12
+Zone State
+.IP "za" 12
+Zone Attributes
+.IP "zai" 12
+Zone Attributes Information
+.IP "rsvd4" 12
+Reserved
+.IP "zcap" 12
+Zone Capacity
+.IP "zslba" 12
+Zone Start Logical Block Address
+.IP "wp" 12
+Write Pointer
+.IP "rsvd32" 12
 Reserved
-.IP "mmctptus" 12
-Maximum MCTP Transmission Unit Size
-.IP "meb" 12
-Management Endpoint Buffer Size
-.IP "{unnamed_union}" 12
-anonymous
-.IP "pcie" 12
-PCIe Port Specific Data
-.IP "smb" 12
-SMBus Port Specific Data
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_resp_status.2` & `libnvme-1.5/doc/man/nvme_mi_resp_status.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_resp_status" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_resp_status" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_resp_status \- values for the response status field
 .SH SYNOPSIS
 enum nvme_mi_resp_status {
 .br
 .BI "    NVME_MI_RESP_SUCCESS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_set_probe_enabled.2` & `libnvme-1.5/doc/man/nvme_mi_set_probe_enabled.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_set_probe_enabled" 9 "nvme_mi_set_probe_enabled" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_set_probe_enabled" 9 "nvme_mi_set_probe_enabled" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_set_probe_enabled \- enable/disable the probe for new endpoints
 .SH SYNOPSIS
 .B "void" nvme_mi_set_probe_enabled
 .BI "(nvme_root_t root "  ","
 .BI "bool enabled "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_status_to_string.2` & `libnvme-1.5/doc/man/nvme_mi_status_to_string.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_status_to_string" 9 "nvme_mi_status_to_string" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_mi_status_to_string" 9 "nvme_mi_status_to_string" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_status_to_string \- return a string representation of the MI status.
 .SH SYNOPSIS
 .B "const char *" nvme_mi_status_to_string
 .BI "(int status "  ");"
 .SH ARGUMENTS
 .IP "status" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_vpd_hdr.2` & `libnvme-1.5/doc/man/nvme_mi_vpd_hdr.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_hdr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_hdr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_hdr \- Vital Product Data Common Header
 .SH SYNOPSIS
 struct nvme_mi_vpd_hdr {
 .br
 .BI "    __u8 ipmiver;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_vpd_mr_common.2` & `libnvme-1.5/doc/man/nvme_mi_vpd_mr_common.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_mr_common" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_mr_common" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_mr_common \- NVMe MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_mr_common {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_vpd_mra.2` & `libnvme-1.5/doc/man/nvme_mi_vpd_mra.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_mra" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_mra" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_mra \- NVMe MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_mra {
 .br
 .BI "    __u8 nmravn;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_vpd_ppmra.2` & `libnvme-1.5/doc/man/nvme_mi_vpd_ppmra.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_ppmra" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_ppmra" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_ppmra \- NVMe PCIe Port MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_ppmra {
 .br
 .BI "    __u8 nppmravn;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_mi_vpd_telem.2` & `libnvme-1.5/doc/man/nvme_mi_vpd_telem.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_telem" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_telem" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_telem \- Vital Product Data Element Descriptor
 .SH SYNOPSIS
 struct nvme_mi_vpd_telem {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_namespace_attach_ctrls.2` & `libnvme-1.5/doc/man/nvme_namespace_attach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_namespace_attach_ctrls" 9 "nvme_namespace_attach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_namespace_attach_ctrls" 9 "nvme_namespace_attach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_namespace_attach_ctrls \- Attach namespace to controller(s)
 .SH SYNOPSIS
 .B "int" nvme_namespace_attach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 num_ctrls "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_namespace_detach_ctrls.2` & `libnvme-1.5/doc/man/nvme_namespace_detach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_namespace_detach_ctrls" 9 "nvme_namespace_detach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_namespace_detach_ctrls" 9 "nvme_namespace_detach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_namespace_detach_ctrls \- Detach namespace from controller(s)
 .SH SYNOPSIS
 .B "int" nvme_namespace_detach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 num_ctrls "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_nd_ns_fpi.2` & `libnvme-1.5/doc/man/nvme_nd_ns_fpi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nd_ns_fpi" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nd_ns_fpi" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_nd_ns_fpi \- If a format operation is in progress, this field indicates the percentage of the namespace that remains to be formatted.
 .SH SYNOPSIS
 enum nvme_nd_ns_fpi {
 .br
 .BI "    NVME_NS_FPI_REMAINING"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_attach_ctrls.2` & `libnvme-1.5/doc/man/nvme_ns_attach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_attach_ctrls" 9 "nvme_ns_attach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_ns_attach_ctrls" 9 "nvme_ns_attach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_attach_ctrls \- Attach namespace to controllers
 .SH SYNOPSIS
 .B "int" nvme_ns_attach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_detach_ctrls.2` & `libnvme-1.5/doc/man/nvme_ns_detach_ctrls.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_detach_ctrls" 9 "nvme_ns_detach_ctrls" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_ns_detach_ctrls" 9 "nvme_ns_detach_ctrls" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_detach_ctrls \- Detach namespace from controllers
 .SH SYNOPSIS
 .B "int" nvme_ns_detach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_id_desc.2` & `libnvme-1.5/doc/man/nvme_ns_id_desc.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_ns_id_desc" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_ns_id_desc" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_ns_id_desc \- Namespace identifier type descriptor
 .SH SYNOPSIS
 struct nvme_ns_id_desc {
 .br
 .BI "    __u8 nidt;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_id_desc_nidt.2` & `libnvme-1.5/doc/man/nvme_ns_id_desc_nidt.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_id_desc_nidt" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_id_desc_nidt" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_id_desc_nidt \- Known namespace identifier types
 .SH SYNOPSIS
 enum nvme_ns_id_desc_nidt {
 .br
 .BI "    NVME_NIDT_EUI64"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_metadata_type.2` & `libnvme-1.5/doc/man/nvme_ns_metadata_type.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_metadata_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_metadata_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_metadata_type \- Namespace Metadata Element Types
 .SH SYNOPSIS
 enum nvme_ns_metadata_type {
 .br
 .BI "    NVME_NS_METADATA_OS_NS_NAME"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_mgmt_create.2` & `libnvme-1.5/doc/man/nvme_ns_mgmt_create.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-.TH "nvme_ns_mgmt_create" 9 "nvme_ns_mgmt_create" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_ns_mgmt_create" 9 "nvme_ns_mgmt_create" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_mgmt_create \- Create a non attached namespace
 .SH SYNOPSIS
 .B "int" nvme_ns_mgmt_create
 .BI "(int fd "  ","
 .BI "struct nvme_id_ns *ns "  ","
 .BI "__u32 *nsid "  ","
 .BI "__u32 timeout "  ","
-.BI "__u8 csi "  ");"
+.BI "__u8 csi "  ","
+.BI "struct nvme_ns_mgmt_host_sw_specified *data "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "ns" 12
 Namespace identification that defines ns creation parameters
 .IP "nsid" 12
 On success, set to the namespace id that was created
 .IP "timeout" 12
 Override the default timeout to this value in milliseconds;
 set to 0 to use the system default.
 .IP "csi" 12
 Command Set Identifier
+.IP "data" 12
+Host Software Specified Fields that defines ns creation parameters
 .SH "DESCRIPTION"
 On successful creation, the namespace exists in the subsystem, but is not
 attached to any controller. Use the \fBnvme_ns_attach_ctrls\fP to assign the
 namespace to one or more controllers.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_mgmt_delete.2` & `libnvme-1.5/doc/man/nvme_ns_mgmt_delete.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_mgmt_delete" 9 "nvme_ns_mgmt_delete" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_ns_mgmt_delete" 9 "nvme_ns_mgmt_delete" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_mgmt_delete \- Delete a non attached namespace
 .SH SYNOPSIS
 .B "int" nvme_ns_mgmt_delete
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_ns_write_protect_cfg.2` & `libnvme-1.5/doc/man/nvme_ns_write_protect_cfg.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_write_protect_cfg" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_write_protect_cfg" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_write_protect_cfg \- Write Protection - Write Protection State
 .SH SYNOPSIS
 enum nvme_ns_write_protect_cfg {
 .br
 .BI "    NVME_NS_WP_CFG_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_nvm_id_ns.2` & `libnvme-1.5/doc/man/nvme_nvm_id_ns.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvm_id_ns" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvm_id_ns" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_nvm_id_ns \- NVME Command Set I/O Command Set Specific Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_nvm_id_ns {
 .br
 .BI "    __le64 lbstm;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_nvm_id_ns_elbaf.2` & `libnvme-1.5/doc/man/nvme_nvm_id_ns_elbaf.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvm_id_ns_elbaf" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvm_id_ns_elbaf" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_nvm_id_ns_elbaf \- This field indicates the extended LBA format
 .SH SYNOPSIS
 enum nvme_nvm_id_ns_elbaf {
 .br
 .BI "    NVME_NVM_ELBAF_STS_MASK"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_nvm_identify_ctrl.2` & `libnvme-1.5/doc/man/nvme_nvm_identify_ctrl.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_nvm_identify_ctrl" 9 "nvme_nvm_identify_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_nvm_identify_ctrl" 9 "nvme_nvm_identify_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_nvm_identify_ctrl \- Identify controller data
 .SH SYNOPSIS
 .B "int" nvme_nvm_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_id_ctrl_nvm *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_nvmeset_pl_status.2` & `libnvme-1.5/doc/man/nvme_nvmeset_pl_status.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvmeset_pl_status" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvmeset_pl_status" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_nvmeset_pl_status \- Predictable Latency Per NVM Set Log - Status
 .SH SYNOPSIS
 enum nvme_nvmeset_pl_status {
 .br
 .BI "    NVME_NVMSET_PL_STATUS_DISABLED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_nvmset_attr.2` & `libnvme-1.5/doc/man/nvme_nvmset_attr.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvmset_attr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvmset_attr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_nvmset_attr \- NVM Set Attributes Entry
 .SH SYNOPSIS
 struct nvme_nvmset_attr {
 .br
 .BI "    __le16 nvmsetid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_nvmset_pl_events.2` & `libnvme-1.5/doc/man/nvme_nvmset_pl_events.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvmset_pl_events" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvmset_pl_events" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_nvmset_pl_events \- Predictable Latency Per NVM Set Log - Event Type
 .SH SYNOPSIS
 enum nvme_nvmset_pl_events {
 .br
 .BI "    NVME_NVMSET_PL_EVENT_DTWIN_READ_WARN"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_nvmset_predictable_lat_log.2` & `libnvme-1.5/doc/man/nvme_nvmset_predictable_lat_log.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvmset_predictable_lat_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvmset_predictable_lat_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_nvmset_predictable_lat_log \- Predictable Latency Mode - Deterministic Threshold Configuration Data
 .SH SYNOPSIS
 struct nvme_nvmset_predictable_lat_log {
 .br
 .BI "    __u8 status;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_passthru_cmd.2` & `libnvme-1.5/doc/man/nvme_passthru_cmd.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_passthru_cmd" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_passthru_cmd" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_passthru_cmd \- nvme passthrough command structure
 .SH SYNOPSIS
 struct nvme_passthru_cmd {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_passthru_cmd64.2` & `libnvme-1.5/doc/man/nvme_passthru_cmd64.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_passthru_cmd64" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_passthru_cmd64" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_passthru_cmd64 \- 64-bit nvme passthrough command structure
 .SH SYNOPSIS
 struct nvme_passthru_cmd64 {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_persistent_event_entry.2` & `libnvme-1.5/doc/man/nvme_persistent_event_entry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_persistent_event_entry" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_persistent_event_entry" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_persistent_event_entry \- Persistent Event
 .SH SYNOPSIS
 struct nvme_persistent_event_entry {
 .br
 .BI "    __u8 etype;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_persistent_event_log.2` & `libnvme-1.5/doc/man/nvme_persistent_event_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_persistent_event_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_persistent_event_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_persistent_event_log \- Persistent Event Log
 .SH SYNOPSIS
 struct nvme_persistent_event_log {
 .br
 .BI "    __u8 lid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_persistent_event_types.2` & `libnvme-1.5/doc/man/nvme_persistent_event_types.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_persistent_event_types" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_persistent_event_types" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_persistent_event_types \- Persistent event log events
 .SH SYNOPSIS
 enum nvme_persistent_event_types {
 .br
 .BI "    NVME_PEL_SMART_HEALTH_EVENT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_pevent_log_action.2` & `libnvme-1.5/doc/man/nvme_pevent_log_action.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_pevent_log_action" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_pevent_log_action" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_pevent_log_action \- Persistent Event Log - Action
 .SH SYNOPSIS
 enum nvme_pevent_log_action {
 .br
 .BI "    NVME_PEVENT_LOG_READ"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_plm_config.2` & `libnvme-1.5/doc/man/nvme_plm_config.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_plm_config" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_plm_config" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_plm_config \- Predictable Latency Mode - Deterministic Threshold Configuration Data Structure
 .SH SYNOPSIS
 struct nvme_plm_config {
 .br
 .BI "    __le16 ee;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_power_on_reset_info_list.2` & `libnvme-1.5/doc/man/nvme_power_on_reset_info_list.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_power_on_reset_info_list" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_power_on_reset_info_list" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_power_on_reset_info_list \- Controller Reset Information
 .SH SYNOPSIS
 struct nvme_power_on_reset_info_list {
 .br
 .BI "    __le16 cid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_primary_ctrl_cap.2` & `libnvme-1.5/doc/man/nvme_primary_ctrl_cap.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_primary_ctrl_cap" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_primary_ctrl_cap" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_primary_ctrl_cap \- Identify - Controller Capabilities Structure
 .SH SYNOPSIS
 struct nvme_primary_ctrl_cap {
 .br
 .BI "    __le16 cntlid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_psd_flags.2` & `libnvme-1.5/doc/man/nvme_psd_flags.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_flags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_flags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_flags \- Possible flag values in nvme power state descriptor
 .SH SYNOPSIS
 enum nvme_psd_flags {
 .br
 .BI "    NVME_PSD_FLAGS_MXPS"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_psd_ps.2` & `libnvme-1.5/doc/man/nvme_psd_ps.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_ps" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_ps" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_ps \- Known values for &struct nvme_psd %ips and %aps. Use with nvme_psd_power_scale() to extract the power scale field to match this enum.
 .SH SYNOPSIS
 enum nvme_psd_ps {
 .br
 .BI "    NVME_PSD_PS_NOT_REPORTED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_psd_workload.2` & `libnvme-1.5/doc/man/nvme_psd_workload.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_workload" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_workload" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_workload \- Specifies a workload hint in the Power Management Feature (see &struct nvme_psd.apw) to inform the NVM subsystem or indicate the conditions for the active power level.
 .SH SYNOPSIS
 enum nvme_psd_workload {
 .br
 .BI "    NVME_PSD_WORKLOAD_NP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_register_offsets.2` & `libnvme-1.5/doc/man/nvme_register_offsets.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_register_offsets" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_register_offsets" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_register_offsets \- controller registers for all transports. This is the layout of BAR0/1 for PCIe, and properties for fabrics.
 .SH SYNOPSIS
 enum nvme_register_offsets {
 .br
 .BI "    NVME_REG_CAP"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_registered_ctrl.2` & `libnvme-1.5/doc/man/nvme_registered_ctrl_ext.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-.TH "libnvme" 9 "struct nvme_registered_ctrl" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_registered_ctrl_ext" "June 2023" "API Manual" LINUX
 .SH NAME
-struct nvme_registered_ctrl \- Registered Controller Data Structure
+struct nvme_registered_ctrl_ext \- Registered Controller Extended Data Structure
 .SH SYNOPSIS
-struct nvme_registered_ctrl {
+struct nvme_registered_ctrl_ext {
 .br
 .BI "    __le16 cntlid;"
 .br
 .BI "    __u8 rcsts;"
 .br
 .BI "    __u8 rsvd3[5];"
 .br
-.BI "    __le64 hostid;"
-.br
 .BI "    __le64 rkey;"
 .br
+.BI "    __u8 hostid[16];"
+.br
+.BI "    __u8 rsvd32[32];"
+.br
 .BI "
 };
 .br
 
 .SH Members
 .IP "cntlid" 12
 Controller ID
 .IP "rcsts" 12
 Reservation Status
 .IP "rsvd3" 12
 Reserved
-.IP "hostid" 12
-Host Identifier
 .IP "rkey" 12
 Reservation Key
+.IP "hostid" 12
+Host Identifier
+.IP "rsvd32" 12
+Reserved
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_acquire.2` & `libnvme-1.5/doc/man/nvme_resv_acquire.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_acquire" 9 "nvme_resv_acquire" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_resv_acquire" 9 "nvme_resv_acquire" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_acquire \- Send an nvme reservation acquire
 .SH SYNOPSIS
 .B "int" nvme_resv_acquire
 .BI "(struct nvme_resv_acquire_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_cptpl.2` & `libnvme-1.5/doc/man/nvme_resv_cptpl.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_cptpl" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_cptpl" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_cptpl \- Reservation Register - Change Persist Through Power Loss State
 .SH SYNOPSIS
 enum nvme_resv_cptpl {
 .br
 .BI "    NVME_RESERVATION_CPTPL_NO_CHANGE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_notification_log.2` & `libnvme-1.5/doc/man/nvme_resv_notification_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_resv_notification_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_resv_notification_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_resv_notification_log \- Reservation Notification Log
 .SH SYNOPSIS
 struct nvme_resv_notification_log {
 .br
 .BI "    __le64 lpc;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_notify_rnlpt.2` & `libnvme-1.5/doc/man/nvme_resv_notify_rnlpt.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_notify_rnlpt" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_notify_rnlpt" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_notify_rnlpt \- Reservation Notification Log - Reservation Notification Log Page Type
 .SH SYNOPSIS
 enum nvme_resv_notify_rnlpt {
 .br
 .BI "    NVME_RESV_NOTIFY_RNLPT_EMPTY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_racqa.2` & `libnvme-1.5/doc/man/nvme_resv_racqa.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_racqa" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_racqa" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_racqa \- Reservation Acquire - Reservation Acquire Action
 .SH SYNOPSIS
 enum nvme_resv_racqa {
 .br
 .BI "    NVME_RESERVATION_RACQA_ACQUIRE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_register.2` & `libnvme-1.5/doc/man/nvme_resv_register.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_register" 9 "nvme_resv_register" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_resv_register" 9 "nvme_resv_register" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_register \- Send an nvme reservation register
 .SH SYNOPSIS
 .B "int" nvme_resv_register
 .BI "(struct nvme_resv_register_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_report.2` & `libnvme-1.5/doc/man/nvme_resv_report.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_report" 9 "nvme_resv_report" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_resv_report" 9 "nvme_resv_report" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_report \- Send an nvme reservation report
 .SH SYNOPSIS
 .B "int" nvme_resv_report
 .BI "(struct nvme_resv_report_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_rrega.2` & `libnvme-1.5/doc/man/nvme_resv_rrega.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_rrega" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_rrega" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_rrega \- Reservation Register - Reservation Register Action
 .SH SYNOPSIS
 enum nvme_resv_rrega {
 .br
 .BI "    NVME_RESERVATION_RREGA_REGISTER_KEY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_rtype.2` & `libnvme-1.5/doc/man/nvme_resv_rtype.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_rtype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_rtype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_rtype \- Reservation Type Encoding
 .SH SYNOPSIS
 enum nvme_resv_rtype {
 .br
 .BI "    NVME_RESERVATION_RTYPE_WE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_resv_status.2` & `libnvme-1.5/doc/man/nvme_resv_status.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_resv_status" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_resv_status" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_resv_status \- Reservation Status Data Structure
 .SH SYNOPSIS
 struct nvme_resv_status {
 .br
 .BI "    __le32 gen;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_sanitize_log_page.2` & `libnvme-1.5/doc/man/nvme_sanitize_log_page.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_sanitize_log_page" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_sanitize_log_page" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_sanitize_log_page \- Sanitize Status (Log Identifier 81h)
 .SH SYNOPSIS
 struct nvme_sanitize_log_page {
 .br
 .BI "    __le16 sprog;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_sanitize_nvm.2` & `libnvme-1.5/doc/man/nvme_sanitize_nvm.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_sanitize_nvm" 9 "nvme_sanitize_nvm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_sanitize_nvm" 9 "nvme_sanitize_nvm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_sanitize_nvm \- Start a sanitize operation
 .SH SYNOPSIS
 .B "int" nvme_sanitize_nvm
 .BI "(struct nvme_sanitize_nvm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_sanitize_sanact.2` & `libnvme-1.5/doc/man/nvme_sanitize_sanact.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_sanitize_sanact" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_sanitize_sanact" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_sanitize_sanact \- Sanitize Action
 .SH SYNOPSIS
 enum nvme_sanitize_sanact {
 .br
 .BI "    NVME_SANITIZE_SANACT_EXIT_FAILURE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_sanitize_sstat.2` & `libnvme-1.5/doc/man/nvme_sanitize_sstat.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_sanitize_sstat" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_sanitize_sstat" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_sanitize_sstat \- Sanitize Status (SSTAT)
 .SH SYNOPSIS
 enum nvme_sanitize_sstat {
 .br
 .BI "    NVME_SANITIZE_SSTAT_STATUS_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_scan_topology.2` & `libnvme-1.5/doc/man/nvme_scan_topology.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_scan_topology" 9 "nvme_scan_topology" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_scan_topology" 9 "nvme_scan_topology" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_scan_topology \- Scan NVMe topology and apply filter
 .SH SYNOPSIS
 .B "int" nvme_scan_topology
 .BI "(nvme_root_t r "  ","
 .BI "nvme_scan_filter_t f "  ","
 .BI "void *f_args "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_secondary_ctrl.2` & `libnvme-1.5/doc/man/nvme_secondary_ctrl.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_secondary_ctrl" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_secondary_ctrl" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_secondary_ctrl \- Secondary Controller Entry
 .SH SYNOPSIS
 struct nvme_secondary_ctrl {
 .br
 .BI "    __le16 scid;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_security_send.2` & `libnvme-1.5/doc/man/nvme_security_send.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_security_send" 9 "nvme_security_send" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_security_send" 9 "nvme_security_send" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_security_send \- Security Send command
 .SH SYNOPSIS
 .B "int" nvme_security_send
 .BI "(struct nvme_security_send_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_self_test_log.2` & `libnvme-1.5/doc/man/nvme_self_test_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_self_test_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_self_test_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_self_test_log \- Device Self-test (Log Identifier 06h)
 .SH SYNOPSIS
 struct nvme_self_test_log {
 .br
 .BI "    __u8 current_operation;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_arbitration.2` & `libnvme-1.5/doc/man/nvme_set_features_arbitration.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_arbitration" 9 "nvme_set_features_arbitration" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_arbitration" 9 "nvme_set_features_arbitration" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_arbitration \- Set arbitration features
 .SH SYNOPSIS
 .B "int" nvme_set_features_arbitration
 .BI "(int fd "  ","
 .BI "__u8 ab "  ","
 .BI "__u8 lpw "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_async_event.2` & `libnvme-1.5/doc/man/nvme_set_features_async_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_async_event" 9 "nvme_set_features_async_event" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_async_event" 9 "nvme_set_features_async_event" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_async_event \- Set asynchronous event feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_async_event
 .BI "(int fd "  ","
 .BI "__u32 events "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_auto_pst.2` & `libnvme-1.5/doc/man/nvme_set_features_auto_pst.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_auto_pst" 9 "nvme_set_features_auto_pst" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_auto_pst" 9 "nvme_set_features_auto_pst" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_auto_pst \- Set autonomous power state feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_auto_pst
 .BI "(int fd "  ","
 .BI "bool apste "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_data.2` & `libnvme-1.5/doc/man/nvme_set_features_data.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_data" 9 "nvme_set_features_data" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_data" 9 "nvme_set_features_data" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_data \- Helper function for @nvme_set_features()
 .SH SYNOPSIS
 .B "int" nvme_set_features_data
 .BI "(int fd "  ","
 .BI "__u8 fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_endurance_evt_cfg.2` & `libnvme-1.5/doc/man/nvme_set_features_endurance_evt_cfg.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_endurance_evt_cfg" 9 "nvme_set_features_endurance_evt_cfg" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_endurance_evt_cfg" 9 "nvme_set_features_endurance_evt_cfg" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_endurance_evt_cfg \- Set endurance event config feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_endurance_evt_cfg
 .BI "(int fd "  ","
 .BI "__u16 endgid "  ","
 .BI "__u8 egwarn "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_err_recovery.2` & `libnvme-1.5/doc/man/nvme_set_features_err_recovery.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_err_recovery" 9 "nvme_set_features_err_recovery" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_err_recovery" 9 "nvme_set_features_err_recovery" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_err_recovery \- Set error recovery feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_err_recovery
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 tler "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_hctm.2` & `libnvme-1.5/doc/man/nvme_set_features_hctm.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_hctm" 9 "nvme_set_features_hctm" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_hctm" 9 "nvme_set_features_hctm" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_hctm \- Set thermal management feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_hctm
 .BI "(int fd "  ","
 .BI "__u16 tmt2 "  ","
 .BI "__u16 tmt1 "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_host_behavior.2` & `libnvme-1.5/doc/man/nvme_set_features_host_behavior.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_host_behavior" 9 "nvme_set_features_host_behavior" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_host_behavior" 9 "nvme_set_features_host_behavior" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_host_behavior \- Set host behavior feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_host_behavior
 .BI "(int fd "  ","
 .BI "bool save "  ","
 .BI "struct nvme_feat_host_behavior *data "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_host_id.2` & `libnvme-1.5/doc/man/nvme_set_features_host_id.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_host_id" 9 "nvme_set_features_host_id" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_host_id" 9 "nvme_set_features_host_id" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_host_id \- Set enable extended host identifiers feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_host_id
 .BI "(int fd "  ","
 .BI "bool exhid "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_irq_coalesce.2` & `libnvme-1.5/doc/man/nvme_set_features_irq_coalesce.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_irq_coalesce" 9 "nvme_set_features_irq_coalesce" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_irq_coalesce" 9 "nvme_set_features_irq_coalesce" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_irq_coalesce \- Set IRQ coalesce feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_irq_coalesce
 .BI "(int fd "  ","
 .BI "__u8 thr "  ","
 .BI "__u8 time "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_irq_config.2` & `libnvme-1.5/doc/man/nvme_set_features_irq_config.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_irq_config" 9 "nvme_set_features_irq_config" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_irq_config" 9 "nvme_set_features_irq_config" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_irq_config \- Set IRQ config feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_irq_config
 .BI "(int fd "  ","
 .BI "__u16 iv "  ","
 .BI "bool cd "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_lba_range.2` & `libnvme-1.5/doc/man/nvme_set_features_write_protect.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-.TH "nvme_set_features_lba_range" 9 "nvme_set_features_lba_range" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_write_protect" 9 "nvme_set_features_write_protect" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_lba_range \- Set LBA range feature
+nvme_set_features_write_protect \- Set write protect feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_lba_range
+.B "int" nvme_set_features_write_protect
 .BI "(int fd "  ","
-.BI "__u32 nsid "  ","
-.BI "__u32 nr_ranges "  ","
+.BI "enum nvme_feat_nswpcfg_state state "  ","
 .BI "bool save "  ","
-.BI "struct nvme_lba_range_type *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "nsid" 12
-Namespace ID
-.IP "nr_ranges" 12
-Number of ranges in \fIdata\fP
+.IP "state" 12
+Write Protection State
 .IP "save" 12
 Save value across power states
-.IP "data" 12
-User address of feature data
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_lba_sts_interval.2` & `libnvme-1.5/doc/man/nvme_set_features_lba_sts_interval.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_lba_sts_interval" 9 "nvme_set_features_lba_sts_interval" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_lba_sts_interval" 9 "nvme_set_features_lba_sts_interval" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_lba_sts_interval \- Set LBA status information feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_lba_sts_interval
 .BI "(int fd "  ","
 .BI "__u16 lsiri "  ","
 .BI "__u16 lsipi "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_nopsc.2` & `libnvme-1.5/doc/man/nvme_set_features_nopsc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_nopsc" 9 "nvme_set_features_nopsc" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_nopsc" 9 "nvme_set_features_nopsc" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_nopsc \- Set non-operational power state feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_nopsc
 .BI "(int fd "  ","
 .BI "bool noppme "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_plm_config.2` & `libnvme-1.5/doc/man/nvme_set_features_plm_config.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_plm_config" 9 "nvme_set_features_plm_config" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_plm_config" 9 "nvme_set_features_plm_config" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_plm_config \- Set predictable latency feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_plm_config
 .BI "(int fd "  ","
 .BI "bool enable "  ","
 .BI "__u16 nvmsetid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_plm_window.2` & `libnvme-1.5/doc/man/nvme_set_features_plm_window.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_plm_window" 9 "nvme_set_features_plm_window" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_plm_window" 9 "nvme_set_features_plm_window" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_plm_window \- Set window select feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_plm_window
 .BI "(int fd "  ","
 .BI "enum nvme_feat_plm_window_select sel "  ","
 .BI "__u16 nvmsetid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_power_mgmt.2` & `libnvme-1.5/doc/man/nvme_set_features_power_mgmt.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_power_mgmt" 9 "nvme_set_features_power_mgmt" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_power_mgmt" 9 "nvme_set_features_power_mgmt" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_power_mgmt \- Set power management feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_power_mgmt
 .BI "(int fd "  ","
 .BI "__u8 ps "  ","
 .BI "__u8 wh "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_resv_mask.2` & `libnvme-1.5/doc/man/nvme_set_features_resv_mask.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_resv_mask" 9 "nvme_set_features_resv_mask" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_mask" 9 "nvme_set_features_resv_mask" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_resv_mask \- Set reservation notification mask feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_resv_mask
 .BI "(int fd "  ","
 .BI "__u32 mask "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_resv_persist.2` & `libnvme-1.5/doc/man/nvme_set_features_resv_persist.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_resv_persist" 9 "nvme_set_features_resv_persist" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_persist" 9 "nvme_set_features_resv_persist" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_resv_persist \- Set persist through power loss feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_resv_persist
 .BI "(int fd "  ","
 .BI "bool ptpl "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_rrl.2` & `libnvme-1.5/doc/man/nvme_set_features_rrl.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_rrl" 9 "nvme_set_features_rrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_rrl" 9 "nvme_set_features_rrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_rrl \- Set read recovery level feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_rrl
 .BI "(int fd "  ","
 .BI "__u8 rrl "  ","
 .BI "__u16 nvmsetid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_sanitize.2` & `libnvme-1.5/doc/man/nvme_set_features_sanitize.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_sanitize" 9 "nvme_set_features_sanitize" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_sanitize" 9 "nvme_set_features_sanitize" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_sanitize \- Set sanitize feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_sanitize
 .BI "(int fd "  ","
 .BI "bool nodrm "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_simple.2` & `libnvme-1.5/doc/man/nvme_set_features_simple.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_simple" 9 "nvme_set_features_simple" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_simple" 9 "nvme_set_features_simple" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_simple \- Helper function for @nvme_set_features()
 .SH SYNOPSIS
 .B "int" nvme_set_features_simple
 .BI "(int fd "  ","
 .BI "__u8 fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_sw_progress.2` & `libnvme-1.5/doc/man/nvme_set_features_temp_thresh.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-.TH "nvme_set_features_sw_progress" 9 "nvme_set_features_sw_progress" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_temp_thresh" 9 "nvme_set_features_temp_thresh" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_sw_progress \- Set pre-boot software load count feature
+nvme_set_features_temp_thresh \- Set temperature threshold feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_sw_progress
+.B "int" nvme_set_features_temp_thresh
 .BI "(int fd "  ","
-.BI "__u8 pbslc "  ","
+.BI "__u16 tmpth "  ","
+.BI "__u8 tmpsel "  ","
+.BI "enum nvme_feat_tmpthresh_thsel thsel "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "pbslc" 12
-Pre-boot Software Load Count
+.IP "tmpth" 12
+Temperature Threshold
+.IP "tmpsel" 12
+Threshold Temperature Select
+.IP "thsel" 12
+Threshold Type Select
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_timestamp.2` & `libnvme-1.5/doc/man/nvme_set_features_timestamp.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_timestamp" 9 "nvme_set_features_timestamp" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_timestamp" 9 "nvme_set_features_timestamp" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_timestamp \- Set timestamp feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_timestamp
 .BI "(int fd "  ","
 .BI "bool save "  ","
 .BI "__u64 timestamp "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_volatile_wc.2` & `libnvme-1.5/doc/man/nvme_set_features_volatile_wc.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_volatile_wc" 9 "nvme_set_features_volatile_wc" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_volatile_wc" 9 "nvme_set_features_volatile_wc" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_volatile_wc \- Set volatile write cache feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_volatile_wc
 .BI "(int fd "  ","
 .BI "bool wce "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_write_atomic.2` & `libnvme-1.5/doc/man/nvme_set_features_write_atomic.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_write_atomic" 9 "nvme_set_features_write_atomic" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_features_write_atomic" 9 "nvme_set_features_write_atomic" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_write_atomic \- Set write atomic feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_write_atomic
 .BI "(int fd "  ","
 .BI "bool dn "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_set_features_write_protect.2` & `libnvme-1.5/doc/man/nvme_get_features_temp_thresh.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-.TH "nvme_set_features_write_protect" 9 "nvme_set_features_write_protect" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_get_features_temp_thresh" 9 "nvme_get_features_temp_thresh" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_write_protect \- Set write protect feature
+nvme_get_features_temp_thresh \- Get temperature threshold feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_write_protect
+.B "int" nvme_get_features_temp_thresh
 .BI "(int fd "  ","
-.BI "enum nvme_feat_nswpcfg_state state "  ","
-.BI "bool save "  ","
+.BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "state" 12
-Write Protection State
-.IP "save" 12
-Save value across power states
+.IP "sel" 12
+Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_set_property.2` & `libnvme-1.5/doc/man/nvme_set_property.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_property" 9 "nvme_set_property" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_set_property" 9 "nvme_set_property" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_property \- Set controller property
 .SH SYNOPSIS
 .B "int" nvme_set_property
 .BI "(struct nvme_set_property_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_smart_crit.2` & `libnvme-1.5/doc/man/nvme_smart_crit.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_smart_crit" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_smart_crit" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_smart_crit \- Critical Warning
 .SH SYNOPSIS
 enum nvme_smart_crit {
 .br
 .BI "    NVME_SMART_CRIT_SPARE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_smart_egcw.2` & `libnvme-1.5/doc/man/nvme_smart_egcw.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_smart_egcw" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_smart_egcw" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_smart_egcw \- Endurance Group Critical Warning Summary
 .SH SYNOPSIS
 enum nvme_smart_egcw {
 .br
 .BI "    NVME_SMART_EGCW_SPARE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_smart_log.2` & `libnvme-1.5/doc/man/nvme_smart_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_smart_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_smart_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_smart_log \- SMART / Health Information Log (Log Identifier 02h)
 .SH SYNOPSIS
 struct nvme_smart_log {
 .br
 .BI "    __u8 critical_warning;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_st_code.2` & `libnvme-1.5/doc/man/nvme_st_code.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_code" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_code" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_st_code \- Self-test Code value
 .SH SYNOPSIS
 enum nvme_st_code {
 .br
 .BI "    NVME_ST_CODE_RESERVED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_st_curr_op.2` & `libnvme-1.5/doc/man/nvme_st_curr_op.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_curr_op" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_curr_op" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_st_curr_op \- Current Device Self-Test Operation
 .SH SYNOPSIS
 enum nvme_st_curr_op {
 .br
 .BI "    NVME_ST_CURR_OP_NOT_RUNNING"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_st_result.2` & `libnvme-1.5/doc/man/nvme_st_result.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_st_result" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_st_result" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_st_result \- Self-test Result
 .SH SYNOPSIS
 struct nvme_st_result {
 .br
 .BI "    __u8 dsts;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_st_valid_diag_info.2` & `libnvme-1.5/doc/man/nvme_st_valid_diag_info.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_valid_diag_info" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_valid_diag_info" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_st_valid_diag_info \- Valid Diagnostic Information
 .SH SYNOPSIS
 enum nvme_st_valid_diag_info {
 .br
 .BI "    NVME_ST_VALID_DIAG_INFO_NSID"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_status_equals.2` & `libnvme-1.5/doc/man/nvme_status_equals.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_equals" 9 "nvme_status_equals" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_status_equals" 9 "nvme_status_equals" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_equals \- helper to check a status against a type and value
 .SH SYNOPSIS
 .B "__u32" nvme_status_equals
 .BI "(int status "  ","
 .BI "enum nvme_status_type type "  ","
 .BI "unsigned int value "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_status_field.2` & `libnvme-1.5/doc/man/nvme_status_field.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_field" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_field" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_status_field \- Defines all parts of the nvme status field: status code, status code type, and additional flags.
 .SH SYNOPSIS
 enum nvme_status_field {
 .br
 .BI "    NVME_SCT_GENERIC"
 , 
@@ -180,14 +180,22 @@
 , 
 .br
 .br
 .BI "    NVME_SC_ADMIN_CMD_MEDIA_NOT_READY"
 , 
 .br
 .br
+.BI "    NVME_SC_FDP_DISABLED"
+, 
+.br
+.br
+.BI "    NVME_SC_INVALID_PLACEMENT_HANDLE_LIST"
+, 
+.br
+.br
 .BI "    NVME_SC_LBA_RANGE"
 , 
 .br
 .br
 .BI "    NVME_SC_CAP_EXCEEDED"
 , 
 .br
@@ -769,14 +777,23 @@
 Lockdown: The command was aborted due to
 command execution being prohibited by
 the Command and Feature Lockdown.
 .IP "NVME_SC_ADMIN_CMD_MEDIA_NOT_READY" 12
 Admin Command Media Not Ready: The Admin
 command requires access to media and
 the media is not ready.
+.IP "NVME_SC_FDP_DISABLED" 12
+Command is not allowed when
+Flexible Data Placement is disabled.
+.IP "NVME_SC_INVALID_PLACEMENT_HANDLE_LIST" 12
+The Placement Handle List is invalid
+due to invalid Reclaim Unit Handle Identifier or
+valid Reclaim Unit Handle Identifier but restricted or
+the Placement Handle List number of entries exceeded the
+maximum number allowed.
 .IP "NVME_SC_LBA_RANGE" 12
 LBA Out of Range: The command references
 an LBA that exceeds the size of the namespace.
 .IP "NVME_SC_CAP_EXCEEDED" 12
 Capacity Exceeded: Execution of the
 command has caused the capacity of the
 namespace to be exceeded.
```

### Comparing `libnvme-1.4/doc/man/nvme_status_result.2` & `libnvme-1.5/doc/man/nvme_status_result.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_result" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_result" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_status_result \- Result of the device self-test operation
 .SH SYNOPSIS
 enum nvme_status_result {
 .br
 .BI "    NVME_ST_RESULT_NO_ERR"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_status_to_errno.2` & `libnvme-1.5/doc/man/nvme_status_to_errno.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_to_errno" 9 "nvme_status_to_errno" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_status_to_errno" 9 "nvme_status_to_errno" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_to_errno \- Converts nvme return status to errno
 .SH SYNOPSIS
 .B "__u8" nvme_status_to_errno
 .BI "(int status "  ","
 .BI "bool fabrics "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_status_to_string.2` & `libnvme-1.5/doc/man/nvme_status_to_string.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_to_string" 9 "nvme_status_to_string" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_status_to_string" 9 "nvme_status_to_string" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_to_string \- Returns string describing nvme return status.
 .SH SYNOPSIS
 .B "const char *" nvme_status_to_string
 .BI "(int status "  ","
 .BI "bool fabrics "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_status_type.2` & `libnvme-1.5/doc/man/nvme_status_type.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_status_type \- type encoding for NVMe return values, when represented as an int.
 .SH SYNOPSIS
 enum nvme_status_type {
 .br
 .BI "    NVME_STATUS_TYPE_SHIFT"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_streams_directive_params.2` & `libnvme-1.5/doc/man/nvme_streams_directive_params.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_streams_directive_params" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_streams_directive_params" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_streams_directive_params \- Streams Directive - Return Parameters Data Structure
 .SH SYNOPSIS
 struct nvme_streams_directive_params {
 .br
 .BI "    __le16 msl;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_submit_admin_passthru.2` & `libnvme-1.5/doc/man/nvme_submit_io_passthru.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.TH "nvme_submit_admin_passthru" 9 "nvme_submit_admin_passthru" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_submit_io_passthru" 9 "nvme_submit_io_passthru" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_submit_admin_passthru \- Submit an nvme passthrough admin command
+nvme_submit_io_passthru \- Submit an nvme passthrough command
 .SH SYNOPSIS
-.B "int" nvme_submit_admin_passthru
+.B "int" nvme_submit_io_passthru
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd *cmd "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "cmd" 12
-The nvme admin command to send
+The nvme io command to send
 .IP "result" 12
 Optional field to return the result from the CQE DW0
 .SH "DESCRIPTION"
-Uses NVME_IOCTL_ADMIN_CMD for the ioctl request.
+Uses NVME_IOCTL_IO_CMD for the ioctl request.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_submit_admin_passthru64.2` & `libnvme-1.5/doc/man/nvme_submit_admin_passthru64.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_submit_admin_passthru64" 9 "nvme_submit_admin_passthru64" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_submit_admin_passthru64" 9 "nvme_submit_admin_passthru64" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_submit_admin_passthru64 \- Submit a 64-bit nvme passthrough admin command
 .SH SYNOPSIS
 .B "int" nvme_submit_admin_passthru64
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd64 *cmd "  ","
 .BI "__u64 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_submit_io_passthru.2` & `libnvme-1.5/doc/man/nvme_submit_admin_passthru.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.TH "nvme_submit_io_passthru" 9 "nvme_submit_io_passthru" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_submit_admin_passthru" 9 "nvme_submit_admin_passthru" "June 2023" "libnvme API manual" LINUX
 .SH NAME
-nvme_submit_io_passthru \- Submit an nvme passthrough command
+nvme_submit_admin_passthru \- Submit an nvme passthrough admin command
 .SH SYNOPSIS
-.B "int" nvme_submit_io_passthru
+.B "int" nvme_submit_admin_passthru
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd *cmd "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "cmd" 12
-The nvme io command to send
+The nvme admin command to send
 .IP "result" 12
 Optional field to return the result from the CQE DW0
 .SH "DESCRIPTION"
-Uses NVME_IOCTL_IO_CMD for the ioctl request.
+Uses NVME_IOCTL_ADMIN_CMD for the ioctl request.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.4/doc/man/nvme_submit_io_passthru64.2` & `libnvme-1.5/doc/man/nvme_submit_io_passthru64.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_submit_io_passthru64" 9 "nvme_submit_io_passthru64" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_submit_io_passthru64" 9 "nvme_submit_io_passthru64" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_submit_io_passthru64 \- Submit a 64-bit nvme passthrough command
 .SH SYNOPSIS
 .B "int" nvme_submit_io_passthru64
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd64 *cmd "  ","
 .BI "__u64 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_subsys_type.2` & `libnvme-1.5/doc/man/nvme_subsys_type.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_subsys_type" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_subsys_type" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_subsys_type \- Type of the NVM subsystem.
 .SH SYNOPSIS
 enum nvme_subsys_type {
 .br
 .BI "    NVME_NQN_DISC"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_supported_cap_config_list_log.2` & `libnvme-1.5/doc/man/nvme_supported_cap_config_list_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_supported_cap_config_list_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_supported_cap_config_list_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_supported_cap_config_list_log \- Supported Capacity Configuration list log page
 .SH SYNOPSIS
 struct nvme_supported_cap_config_list_log {
 .br
 .BI "    __u8 sccn;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_telemetry_log.2` & `libnvme-1.5/doc/man/nvme_telemetry_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_telemetry_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_telemetry_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_telemetry_log \- Retrieve internal data specific to the manufacturer.
 .SH SYNOPSIS
 struct nvme_telemetry_log {
 .br
 .BI "    __u8 lpi;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_uring_cmd.2` & `libnvme-1.5/doc/man/nvme_uring_cmd.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_uring_cmd" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_uring_cmd" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_uring_cmd \- nvme uring command structure
 .SH SYNOPSIS
 struct nvme_uring_cmd {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_verify.2` & `libnvme-1.5/doc/man/nvme_verify.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_verify" 9 "nvme_verify" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_verify" 9 "nvme_verify" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_verify \- Send an nvme verify command
 .SH SYNOPSIS
 .B "int" nvme_verify
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_virt_mgmt_act.2` & `libnvme-1.5/doc/man/nvme_virt_mgmt_act.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_virt_mgmt_act" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_virt_mgmt_act" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_virt_mgmt_act \- Virtualization Management - Action
 .SH SYNOPSIS
 enum nvme_virt_mgmt_act {
 .br
 .BI "    NVME_VIRT_MGMT_ACT_PRIM_CTRL_FLEX_ALLOC"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_virtual_mgmt.2` & `libnvme-1.5/doc/man/nvme_virtual_mgmt.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_virtual_mgmt" 9 "nvme_virtual_mgmt" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_virtual_mgmt" 9 "nvme_virtual_mgmt" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_virtual_mgmt \- Virtualization resource management
 .SH SYNOPSIS
 .B "int" nvme_virtual_mgmt
 .BI "(struct nvme_virtual_mgmt_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_write_uncorrectable.2` & `libnvme-1.5/doc/man/nvme_write_uncorrectable.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_write_uncorrectable" 9 "nvme_write_uncorrectable" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_write_uncorrectable" 9 "nvme_write_uncorrectable" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_write_uncorrectable \- Submit an nvme write uncorrectable command
 .SH SYNOPSIS
 .B "int" nvme_write_uncorrectable
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_write_zeros.2` & `libnvme-1.5/doc/man/nvme_write_zeros.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_write_zeros" 9 "nvme_write_zeros" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_write_zeros" 9 "nvme_write_zeros" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_write_zeros \- Submit an nvme write zeroes command
 .SH SYNOPSIS
 .B "int" nvme_write_zeros
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_id_ns.2` & `libnvme-1.5/doc/man/nvme_zns_id_ns.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_zns_id_ns" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_zns_id_ns" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvme_zns_id_ns \- Zoned Namespace Command Set Specific Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_zns_id_ns {
 .br
 .BI "    __le16 zoc;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_identify_ctrl.2` & `libnvme-1.5/doc/man/nvme_zns_identify_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_identify_ctrl" 9 "nvme_zns_identify_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_zns_identify_ctrl" 9 "nvme_zns_identify_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_identify_ctrl \- ZNS identify controller data
 .SH SYNOPSIS
 .B "int" nvme_zns_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_zns_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_identify_ns.2` & `libnvme-1.5/doc/man/nvme_zns_identify_ns.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_identify_ns" 9 "nvme_zns_identify_ns" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_zns_identify_ns" 9 "nvme_zns_identify_ns" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_identify_ns \- ZNS identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_zns_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_zns_id_ns *data "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_report_options.2` & `libnvme-1.5/doc/man/nvme_zns_report_options.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_report_options" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_report_options" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_report_options \- Zone Management Receive - Zone Receive Action Specific Field
 .SH SYNOPSIS
 enum nvme_zns_report_options {
 .br
 .BI "    NVME_ZNS_ZRAS_REPORT_ALL"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_report_zones.2` & `libnvme-1.5/doc/man/nvme_zns_report_zones.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_report_zones" 9 "nvme_zns_report_zones" "March 2023" "libnvme API manual" LINUX
+.TH "nvme_zns_report_zones" 9 "nvme_zns_report_zones" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_report_zones \- Return the list of zones
 .SH SYNOPSIS
 .B "int" nvme_zns_report_zones
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u64 slba "  ","
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_send_action.2` & `libnvme-1.5/doc/man/nvme_zns_send_action.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_send_action" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_send_action" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_send_action \- Zone Management Send - Zone Send Action
 .SH SYNOPSIS
 enum nvme_zns_send_action {
 .br
 .BI "    NVME_ZNS_ZSA_CLOSE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_za.2` & `libnvme-1.5/doc/man/nvme_zns_za.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_za" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_za" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_za \- Zone Descriptor Data Structure
 .SH SYNOPSIS
 enum nvme_zns_za {
 .br
 .BI "    NVME_ZNS_ZA_ZFC"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvme_zns_zs.2` & `libnvme-1.5/doc/man/nvme_zns_zs.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_zs" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_zs" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_zs \- Zone Descriptor Data Structure - Zone State
 .SH SYNOPSIS
 enum nvme_zns_zs {
 .br
 .BI "    NVME_ZNS_ZS_EMPTY"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_add_ctrl.2` & `libnvme-1.5/doc/man/nvmf_add_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_add_ctrl" 9 "nvmf_add_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_add_ctrl" 9 "nvmf_add_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_add_ctrl \- Connect a controller and update topology
 .SH SYNOPSIS
 .B "int" nvmf_add_ctrl
 .BI "(nvme_host_t h "  ","
 .BI "nvme_ctrl_t c "  ","
 .BI "const struct nvme_fabrics_config *cfg "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvmf_addr_family.2` & `libnvme-1.5/doc/man/nvmf_addr_family.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_addr_family" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_addr_family" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_addr_family \- Address Family codes for Discovery Log Page entry ADRFAM field
 .SH SYNOPSIS
 enum nvmf_addr_family {
 .br
 .BI "    NVMF_ADDR_FAMILY_PCI"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_connect_data.2` & `libnvme-1.5/doc/man/nvmf_connect_data.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_connect_data" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_connect_data" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_connect_data \- Data payload for the 'connect' command
 .SH SYNOPSIS
 struct nvmf_connect_data {
 .br
 .BI "    __u8 hostid[16];"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_connect_disc_entry.2` & `libnvme-1.5/doc/man/nvmf_connect_disc_entry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_connect_disc_entry" 9 "nvmf_connect_disc_entry" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_connect_disc_entry" 9 "nvmf_connect_disc_entry" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_connect_disc_entry \- Connect controller based on the discovery log page entry
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvmf_connect_disc_entry
 .BI "(nvme_host_t h "  ","
 .BI "struct nvmf_disc_log_entry *e "  ","
 .BI "const struct nvme_fabrics_config *defcfg "  ","
```

### Comparing `libnvme-1.4/doc/man/nvmf_dim_data.2` & `libnvme-1.5/doc/man/nvmf_dim_data.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_dim_data" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_dim_data" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_dim_data \- Discovery Information Management (DIM) - Data
 .SH SYNOPSIS
 struct nvmf_dim_data {
 .br
 .BI "    __le32 tdl;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_disc_eflags.2` & `libnvme-1.5/doc/man/nvmf_disc_eflags.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_disc_eflags" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_disc_eflags" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_disc_eflags \- Discovery Log Page entry flags.
 .SH SYNOPSIS
 enum nvmf_disc_eflags {
 .br
 .BI "    NVMF_DISC_EFLAGS_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_disc_log_entry.2` & `libnvme-1.5/doc/man/nvmf_disc_log_entry.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_disc_log_entry" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_disc_log_entry" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_disc_log_entry \- Discovery Log Page entry
 .SH SYNOPSIS
 struct nvmf_disc_log_entry {
 .br
 .BI "    __u8 trtype;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_discovery_log.2` & `libnvme-1.5/doc/man/nvmf_discovery_log.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_discovery_log" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_discovery_log" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_discovery_log \- Discovery Log Page (Log Identifier 70h)
 .SH SYNOPSIS
 struct nvmf_discovery_log {
 .br
 .BI "    __le64 genctr;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_ext_attr.2` & `libnvme-1.5/doc/man/nvmf_ext_attr.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_ext_attr" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_ext_attr" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_ext_attr \- Extended Attribute (EXAT)
 .SH SYNOPSIS
 struct nvmf_ext_attr {
 .br
 .BI "    __le16 exattype;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_ext_die.2` & `libnvme-1.5/doc/man/nvmf_ext_die.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_ext_die" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_ext_die" "June 2023" "API Manual" LINUX
 .SH NAME
 struct nvmf_ext_die \- Extended Discovery Information Entry (DIE)
 .SH SYNOPSIS
 struct nvmf_ext_die {
 .br
 .BI "    __u8 trtype;"
 .br
```

### Comparing `libnvme-1.4/doc/man/nvmf_get_discovery_log.2` & `libnvme-1.5/doc/man/nvmf_get_discovery_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_get_discovery_log" 9 "nvmf_get_discovery_log" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_get_discovery_log" 9 "nvmf_get_discovery_log" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_get_discovery_log \- Return the discovery log page
 .SH SYNOPSIS
 .B "int" nvmf_get_discovery_log
 .BI "(nvme_ctrl_t c "  ","
 .BI "struct nvmf_discovery_log **logp "  ","
 .BI "int max_retries "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvmf_get_discovery_wargs.2` & `libnvme-1.5/doc/man/nvmf_get_discovery_wargs.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_get_discovery_wargs" 9 "nvmf_get_discovery_wargs" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_get_discovery_wargs" 9 "nvmf_get_discovery_wargs" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_get_discovery_wargs \- Get the discovery log page with args
 .SH SYNOPSIS
 .B "struct nvmf_discovery_log *" nvmf_get_discovery_wargs
 .BI "(struct nvme_get_discovery_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.4/doc/man/nvmf_log_discovery_lsp.2` & `libnvme-1.5/doc/man/nvmf_log_discovery_lsp.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_log_discovery_lsp" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_log_discovery_lsp" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_log_discovery_lsp \- Discovery log specific field
 .SH SYNOPSIS
 enum nvmf_log_discovery_lsp {
 .br
 .BI "    NVMF_LOG_DISC_LSP_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_rdma_prtype.2` & `libnvme-1.5/doc/man/nvmf_rdma_prtype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_rdma_prtype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_rdma_prtype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_rdma_prtype \- RDMA Provider Type codes for Discovery Log Page entry TSAS RDMA_PRTYPE field
 .SH SYNOPSIS
 enum nvmf_rdma_prtype {
 .br
 .BI "    NVMF_RDMA_PRTYPE_NOT_SPECIFIED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_register_ctrl.2` & `libnvme-1.5/doc/man/nvmf_register_ctrl.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_register_ctrl" 9 "nvmf_register_ctrl" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_register_ctrl" 9 "nvmf_register_ctrl" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_register_ctrl \- Perform registration task with a DC
 .SH SYNOPSIS
 .B "int" nvmf_register_ctrl
 .BI "(nvme_ctrl_t c "  ","
 .BI "enum nvmf_dim_tas tas "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.4/doc/man/nvmf_tcp_sectype.2` & `libnvme-1.5/doc/man/nvmf_tcp_sectype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_tcp_sectype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_tcp_sectype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_tcp_sectype \- Transport Specific Address Subtype Definition for NVMe/TCP Transport
 .SH SYNOPSIS
 enum nvmf_tcp_sectype {
 .br
 .BI "    NVMF_TCP_SECTYPE_NONE"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_treq.2` & `libnvme-1.5/doc/man/nvmf_treq.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_treq" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_treq" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_treq \- Transport Requirements codes for Discovery Log Page entry TREQ field
 .SH SYNOPSIS
 enum nvmf_treq {
 .br
 .BI "    NVMF_TREQ_NOT_SPECIFIED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_trtype.2` & `libnvme-1.5/doc/man/nvmf_trtype.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_trtype" "March 2023" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_trtype" "June 2023" "API Manual" LINUX
 .SH NAME
 enum nvmf_trtype \- Transport Type codes for Discovery Log Page entry TRTYPE field
 .SH SYNOPSIS
 enum nvmf_trtype {
 .br
 .BI "    NVMF_TRTYPE_UNSPECIFIED"
 ,
```

### Comparing `libnvme-1.4/doc/man/nvmf_update_config.2` & `libnvme-1.5/doc/man/nvmf_update_config.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_update_config" 9 "nvmf_update_config" "March 2023" "libnvme API manual" LINUX
+.TH "nvmf_update_config" 9 "nvmf_update_config" "June 2023" "libnvme API manual" LINUX
 .SH NAME
 nvmf_update_config \- Update fabrics configuration values
 .SH SYNOPSIS
 .B "void" nvmf_update_config
 .BI "(nvme_ctrl_t c "  ","
 .BI "const struct nvme_fabrics_config *cfg "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.4/doc/meson.build` & `libnvme-1.5/doc/meson.build`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # Copyright (c) 2022 SUSE LLC
 #
 # Authors: Martin Belanger <Martin.Belanger@dell.com>
 # Authors: Daniel Wagner <dwagner@suse.de>
 #
 
 api_files = [
+  'fabrics.h',
   'filters.h',
   'ioctl.h',
   'linux.h',
   'log.h',
   'mi.h',
+  'nbft.h',
   'tree.h',
   'types.h',
-  'fabrics.h',
   'util.h'
 ]
 
 api_paths = []
 foreach f: api_files
   api_paths += files('../src/nvme/' + f)
 endforeach
@@ -40,26 +41,28 @@
   static_sources += configure_file(input: file + '.in',
                                    output: file,
                                    configuration: substs)
 endforeach
 
 subdir('rst')
 
+top_source_dir = meson.current_source_dir() + '/../'
+
 want_docs = get_option('docs')
 want_docs_build = get_option('docs-build')
-kernel_doc = find_program('kernel-doc')
-kernel_doc_check = find_program('kernel-doc-check')
+kernel_doc = find_program(top_source_dir + 'scripts/kernel-doc')
+kernel_doc_check = find_program(top_source_dir +'scripts/kernel-doc-check')
 
 test('kdoc', kernel_doc_check, args: api_paths)
 
 if want_docs != 'false'
 
   if want_docs == 'all' or want_docs == 'man'
     mandir = join_paths(get_option('mandir'), 'man2')
-    list_man_pages = find_program('list-man-pages.sh')
+    list_man_pages = find_program(top_source_dir + 'scripts/list-man-pages.sh')
     if want_docs_build
       foreach apif : api_paths
         c = run_command(list_man_pages, apif, check: true)
         man_pages = c.stdout().split()
         foreach page : man_pages
           custom_target(
             page.underscorify() + '_man',
@@ -74,15 +77,15 @@
                       apif],
             install: true,
             install_dir: mandir)
         endforeach
       endforeach
     else
       if want_docs == 'all' or want_docs == 'man'
-        list_pre_compiled = find_program('list-pre-compiled.sh')
+        list_pre_compiled = find_program(top_source_dir + 'scripts/list-pre-compiled.sh')
         m = run_command(list_pre_compiled, check: true)
         man_pages = m.stdout().strip().split('\n')
         install_data(man_pages, install_dir: mandir)
       endif
     endif
   endif
```

### Comparing `libnvme-1.4/doc/mi.rst.in` & `libnvme-1.5/doc/mi.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/rst/fabrics.rst` & `libnvme-1.5/doc/rst/fabrics.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/rst/filters.rst` & `libnvme-1.5/doc/rst/filters.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/rst/ioctl.rst` & `libnvme-1.5/doc/rst/ioctl.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3879,15 +3879,15 @@
 
 **Return**
 
 The nvme command status if a response was received (see
 :c:type:`enum nvme_status_field <nvme_status_field>`) or -1 with errno set otherwise.
 
 
-.. c:function:: int nvme_ns_mgmt_create (int fd, struct nvme_id_ns *ns, __u32 *nsid, __u32 timeout, __u8 csi)
+.. c:function:: int nvme_ns_mgmt_create (int fd, struct nvme_id_ns *ns, __u32 *nsid, __u32 timeout, __u8 csi, struct nvme_ns_mgmt_host_sw_specified *data)
 
    Create a non attached namespace
 
 **Parameters**
 
 ``int fd``
   File descriptor of nvme device
@@ -3901,14 +3901,17 @@
 ``__u32 timeout``
   Override the default timeout to this value in milliseconds;
   set to 0 to use the system default.
 
 ``__u8 csi``
   Command Set Identifier
 
+``struct nvme_ns_mgmt_host_sw_specified *data``
+  Host Software Specified Fields that defines ns creation parameters
+
 **Description**
 
 On successful creation, the namespace exists in the subsystem, but is not
 attached to any controller. Use the nvme_ns_attach_ctrls() to assign the
 namespace to one or more controllers.
 
 **Return**
```

### Comparing `libnvme-1.4/doc/rst/linux.rst` & `libnvme-1.5/doc/rst/linux.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/doc/rst/meson.build` & `libnvme-1.5/doc/rst/meson.build`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+top_source_dir = meson.current_source_dir() + '/../../'
+
 want_docs = get_option('docs')
 
 if want_docs != 'false'
   want_docs_build = get_option('docs-build')
   rstdir = get_option('rstdir')
   if want_docs_build
-    kernel_doc = find_program('../kernel-doc')
+    kernel_doc = find_program(top_source_dir + 'scripts/kernel-doc')
 
     conf = configuration_data()
     conf.set('SYSCONFDIR', sysconfdir)
 
     if want_docs == 'all' or want_docs == 'rst' or want_docs == 'html'
       foreach apif : api_files
-        afile = files('../../src/nvme/' + apif)
+        afile = files(top_source_dir + 'src/nvme/' + apif)
         subst = configure_file(
             input: afile,
             output: '@BASENAME@.subst',
             configuration: conf)
         rst = custom_target(
           apif.underscorify() + '_rst',
           input: subst,
```

### Comparing `libnvme-1.4/doc/rst/mi.rst` & `libnvme-1.5/doc/rst/mi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1025,14 +1025,35 @@
 
 **Parameters**
 
 ``nvme_mi_ctrl_t ctrl``
   controller to free
 
 
+.. c:function:: __u16 nvme_mi_ctrl_id (nvme_mi_ctrl_t ctrl)
+
+   get the ID of a controller
+
+**Parameters**
+
+``nvme_mi_ctrl_t ctrl``
+  controller to query
+
+**Description**
+
+Retrieve the ID of the controller, as defined by hardware, and available
+in the Identify (Controller List) data. This is the value passed to
+**nvme_mi_init_ctrl**, but may have been created internally via
+**nvme_mi_scan_ep**.
+
+**Return**
+
+the (locally-stored) ID of this controller.
+
+
 .. c:function:: char * nvme_mi_endpoint_desc (nvme_mi_ep_t ep)
 
    Get a string describing a MI endpoint.
 
 **Parameters**
 
 ``nvme_mi_ep_t ep``
@@ -2965,15 +2986,15 @@
 
 **Return**
 
 The nvme command status if a response was received (see
 :c:type:`enum nvme_status_field <nvme_status_field>`) or -1 with errno set otherwise.
 
 
-.. c:function:: int nvme_mi_admin_ns_mgmt_create (nvme_mi_ctrl_t ctrl, struct nvme_id_ns *ns, __u8 csi, __u32 *nsid)
+.. c:function:: int nvme_mi_admin_ns_mgmt_create (nvme_mi_ctrl_t ctrl, struct nvme_id_ns *ns, __u8 csi, __u32 *nsid, struct nvme_ns_mgmt_host_sw_specified *data)
 
    Helper for Namespace Management Create command
 
 **Parameters**
 
 ``nvme_mi_ctrl_t ctrl``
   Controller to send command to
@@ -2983,14 +3004,17 @@
 
 ``__u8 csi``
   Command Set Identifier for new NS
 
 ``__u32 *nsid``
   Set to new namespace ID on create
 
+``struct nvme_ns_mgmt_host_sw_specified *data``
+  Host Software Specified Fields that defines ns creation parameters
+
 **Description**
 
 Issues a Namespace Management (Create) command to **ctrl**, to create a
 new namespace specified by **ns**, using command set **csi**. On success,
 the new namespace ID will be written to **nsid**.
 
 **Return**
```

### Comparing `libnvme-1.4/doc/rst/tree.rst` & `libnvme-1.5/doc/rst/tree.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,45 @@
   Logging level to use
 
 **Return**
 
 Initialized :c:type:`nvme_root_t` object
 
 
+.. c:function:: void nvme_root_set_application (nvme_root_t r, const char *a)
+
+   Specify managing application
+
+**Parameters**
+
+``nvme_root_t r``
+  :c:type:`nvme_root_t` object
+
+``const char *a``
+  Application string
+
+**Description**
+
+Sets the managing application string for **r**.
+
+
+.. c:function:: const char * nvme_root_get_application (nvme_root_t r)
+
+   Get managing application
+
+**Parameters**
+
+``nvme_root_t r``
+  :c:type:`nvme_root_t` object
+
+**Description**
+
+Returns the managing application string for **r** or NULL if not set.
+
+
 .. c:function:: void nvme_free_tree (nvme_root_t r)
 
    Free root object
 
 **Parameters**
 
 ``nvme_root_t r``
@@ -1315,14 +1346,29 @@
 
 **Return**
 
 NVMe-over-Fabrics address string of **c** or empty string
 of no address is present.
 
 
+.. c:function:: const char * nvme_ctrl_get_phy_slot (nvme_ctrl_t c)
+
+   PCI physical slot number of a controller
+
+**Parameters**
+
+``nvme_ctrl_t c``
+  Controller instance
+
+**Return**
+
+PCI physical slot number of **c** or empty string if slot
+number is not present.
+
+
 .. c:function:: const char * nvme_ctrl_get_firmware (nvme_ctrl_t c)
 
    Firmware string of a controller
 
 **Parameters**
 
 ``nvme_ctrl_t c``
@@ -1881,14 +1927,45 @@
 Returns the subsystem type of **s**.
 
 **Return**
 
 'nvm' or 'discovery'
 
 
+.. c:function:: const char * nvme_subsystem_get_application (nvme_subsystem_t s)
+
+   Return the application string
+
+**Parameters**
+
+``nvme_subsystem_t s``
+  nvme_subsystem_t object
+
+**Return**
+
+Managing application string or NULL if not set.
+
+
+.. c:function:: void nvme_subsystem_set_application (nvme_subsystem_t s, const char *a)
+
+   Set the application string
+
+**Parameters**
+
+``nvme_subsystem_t s``
+  nvme_subsystem_t object
+
+``const char *a``
+  application string
+
+**Description**
+
+Sets the managing application string for **s**.
+
+
 .. c:function:: int nvme_scan_topology (nvme_root_t r, nvme_scan_filter_t f, void *f_args)
 
    Scan NVMe topology and apply filter
 
 **Parameters**
 
 ``nvme_root_t r``
```

### Comparing `libnvme-1.4/doc/rst/types.rst` & `libnvme-1.5/doc/rst/types.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9621,14 +9621,25 @@
   the Command and Feature Lockdown.
 
 ``NVME_SC_ADMIN_CMD_MEDIA_NOT_READY``
   Admin Command Media Not Ready: The Admin
   command requires access to media and
   the media is not ready.
 
+``NVME_SC_FDP_DISABLED``
+  Command is not allowed when
+  Flexible Data Placement is disabled.
+
+``NVME_SC_INVALID_PLACEMENT_HANDLE_LIST``
+  The Placement Handle List is invalid
+  due to invalid Reclaim Unit Handle Identifier or
+  valid Reclaim Unit Handle Identifier but restricted or
+  the Placement Handle List number of entries exceeded the
+  maximum number allowed.
+
 ``NVME_SC_LBA_RANGE``
   LBA Out of Range: The command references
   an LBA that exceeds the size of the namespace.
 
 ``NVME_SC_CAP_EXCEEDED``
   Capacity Exceeded: Execution of the
   command has caused the capacity of the
@@ -11748,7 +11759,129 @@
 
 **Constants**
 
 ``NVME_IO_MGMT_SEND_RUH_UPDATE``
   Reclaim Unit Handle Update
 
 
+
+
+.. c:struct:: nvme_ns_mgmt_host_sw_specified
+
+   Namespace management Host Software Specified Fields.
+
+**Definition**
+
+::
+
+  struct nvme_ns_mgmt_host_sw_specified {
+    __le64 nsze;
+    __le64 ncap;
+    __u8 rsvd16[10];
+    __u8 flbas;
+    __u8 rsvd27[2];
+    __u8 dps;
+    __u8 nmic;
+    __u8 rsvd31[61];
+    __le32 anagrpid;
+    __u8 rsvd96[4];
+    __le16 nvmsetid;
+    __le16 endgid;
+    __u8 rsvd104[280];
+    __le64 lbstm;
+    __le16 nphndls;
+    __u8 rsvd394[105];
+    union {
+      __u8 rsvd499[13];
+      struct {
+        __u8 znsco;
+        __le32 rar;
+        __le32 ror;
+        __le32 rnumzrwa;
+      } zns;
+    };
+    __le16 phndl[128];
+    __u8 rsvd768[3328];
+  };
+
+**Members**
+
+``nsze``
+  Namespace Size indicates the total size of the namespace in
+  logical blocks. The number of logical blocks is based on the
+  formatted LBA size.
+
+``ncap``
+  Namespace Capacity indicates the maximum number of logical blocks
+  that may be allocated in the namespace at any point in time. The
+  number of logical blocks is based on the formatted LBA size.
+
+``rsvd16``
+  Reserved
+
+``flbas``
+  Formatted LBA Size, see :c:type:`enum nvme_id_ns_flbas <nvme_id_ns_flbas>`.
+
+``rsvd27``
+  Reserved
+
+``dps``
+  End-to-end Data Protection Type Settings, see
+  :c:type:`enum nvme_id_ns_dps <nvme_id_ns_dps>`.
+
+``nmic``
+  Namespace Multi-path I/O and Namespace Sharing Capabilities, see
+  :c:type:`enum nvme_id_ns_nmic <nvme_id_ns_nmic>`.
+
+``rsvd31``
+  Reserved
+
+``anagrpid``
+  ANA Group Identifier indicates the ANA Group Identifier of the
+  ANA group of which the namespace is a member.
+
+``rsvd96``
+  Reserved
+
+``nvmsetid``
+  NVM Set Identifier indicates the NVM Set with which this
+  namespace is associated.
+
+``endgid``
+  Endurance Group Identifier indicates the Endurance Group with
+  which this namespace is associated.
+
+``rsvd104``
+  Reserved
+
+``lbstm``
+  Logical Block Storage Tag Mask Identifies the mask for the
+  Storage Tag field for the protection information
+
+``nphndls``
+  Number of Placement Handles specifies the number of Placement
+  Handles included in the Placement Handle List
+
+``rsvd394``
+  Reserved
+
+``{unnamed_union}``
+  anonymous
+
+``rsvd499``
+  Reserved for I/O Command Sets that extend this specification.
+
+``zns``
+  rsvd499( Zoned Namespace Command Set specific field )
+
+``phndl``
+  Placement Handle Associated RUH : This field specifies the Reclaim
+  Unit Handle Identifier to be associated with the Placement Handle
+  value. If the Flexible Data Placement capability is not supported or
+  not enabled in specified Endurance Group, then the controller shall
+  ignore this field.
+
+``rsvd768``
+  Reserved
+
+
+
```

### Comparing `libnvme-1.4/doc/rst/util.rst` & `libnvme-1.5/doc/rst/util.rst`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
 ``ENVME_CONNECT_OPNOTSUPP``
   not supported
 
 ``ENVME_CONNECT_CONNREFUSED``
   connection refused
 
+``ENVME_CONNECT_ADDRNOTAVAIL``
+  cannot assign requested address
+
+``ENVME_CONNECT_IGNORED``
+  connect attempt is ignored due to configuration
+
 
 .. c:function:: __u8 nvme_status_to_errno (int status, bool fabrics)
 
    Converts nvme return status to errno
 
 **Parameters**
 
@@ -571,7 +577,24 @@
 https://www.rfc-editor.org/rfc/rfc4122#section-4.4
 
 **Return**
 
 Returns error code if generating of random number fails.
 
 
+.. c:function:: bool nvme_ipaddrs_eq (const char *addr1, const char *addr2)
+
+   Check if 2 IP addresses are equal.
+
+**Parameters**
+
+``const char *addr1``
+  IP address (can be IPv4 or IPv6)
+
+``const char *addr2``
+  IP address (can be IPv4 or IPv6)
+
+**Return**
+
+true if addr1 == addr2. false otherwise.
+
+
```

### Comparing `libnvme-1.4/examples/discover-loop.c` & `libnvme-1.5/examples/discover-loop.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/examples/discover-loop.py` & `libnvme-1.5/examples/discover-loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,14 @@
     lsp = nvme.NVMF_LOG_DISC_LSP_PLEO if dlp_supp_opts & nvme.NVMF_LOG_DISC_LID_PLEOS else 0
     d = c.discover(lsp=lsp)
     print(pprint.pformat(d))
 except Exception as e:
     sys.exit(f'Failed to discover: {e}')
 
 try:
-c.disconnect()
+    c.disconnect()
 except Exception as e:
     sys.exit(f'Failed to disconnect: {e}')
 
 c = None
 h = None
 r = None
```

### Comparing `libnvme-1.4/examples/display-columnar.c` & `libnvme-1.5/examples/display-columnar.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/examples/display-tree.c` & `libnvme-1.5/examples/display-tree.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/examples/meson.build` & `libnvme-1.5/examples/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/examples/mi-conf.c` & `libnvme-1.5/examples/mi-conf.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/examples/mi-mctp.c` & `libnvme-1.5/examples/mi-mctp.c`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 		err(EXIT_FAILURE, "can't perform Health Status Poll operation");
 
 	printf("NVMe MI subsys health:\n");
 	printf(" subsystem status:  0x%x\n", ss_health.nss);
 	printf(" smart warnings:    0x%x\n", ss_health.sw);
 	printf(" composite temp:    %d\n", ss_health.ctemp);
 	printf(" drive life used:   %d%%\n", ss_health.pdlu);
-	printf(" controller status: 0x%04x\n", le16_to_cpu(ss_health.pdlu));
+	printf(" controller status: 0x%04x\n", le16_to_cpu(ss_health.ccs));
 
 	return 0;
 }
 
 static int show_ctrl(nvme_mi_ep_t ep, uint16_t ctrl_id)
 {
 	struct nvme_mi_read_ctrl_info ctrl;
```

### Comparing `libnvme-1.4/examples/telemetry-listen.c` & `libnvme-1.5/examples/telemetry-listen.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/internal/meson.build` & `libnvme-1.5/internal/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/libnvme/README.md` & `libnvme-1.5/libnvme/README.md`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/libnvme/meson.build` & `libnvme-1.5/libnvme/meson.build`

 * *Files 10% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 # Copyright (c) 2021 Dell Inc.
 #
 # Authors: Martin Belanger <Martin.Belanger@dell.com>
 #
 want_python = get_option('python')
 if want_python.disabled()
     build_python_bindings = false
+    py3_dep = dependency('', required: false)  # Needed for muon
 else
     python3 = import('python').find_installation('python3')
     py3_dep = python3.dependency(required: want_python)
     swig = find_program('swig', required: want_python)
     header_found = cc.has_header('Python.h', dependencies: py3_dep, required: want_python)
     build_python_bindings = py3_dep.found() and swig.found() and header_found
 endif
 
 if build_python_bindings
+    r = run_command(swig, ['-version'], check: true)  # Returns: "\nSWIG Version 4.1.1\n\nCompiled with ..."
+    swig_version = r.stdout().split('\n')[1].split()[2].strip()
+    if swig_version.version_compare('<4.1.0')
+        swig_cmd = [swig, '-python', '-py3', '-o', '@OUTPUT1@', '@INPUT0@']
+    else
+        swig_cmd = [swig, '-python', '-o', '@OUTPUT1@', '@INPUT0@']
+    endif
+
     pymod_swig = custom_target(
         'nvme.py',
         input:   ['nvme.i'],
         output:  ['nvme.py', 'nvme_wrap.c'],
-        command: [swig, '-python', '-py3', '-o', '@OUTPUT1@', '@INPUT0@'],
+        command: swig_cmd,
         install: true,
         install_dir: [python3.get_install_dir(pure: false, subdir: 'libnvme'), false],
     )
 
     pynvme_clib = python3.extension_module(
         '_nvme',
         pymod_swig[1],
@@ -57,16 +66,17 @@
     test_env.append('PYTHONPATH', join_paths(meson.current_build_dir(), '..'))
     test_env.append('PYTHONMALLOC', 'malloc')
 
     # Test section
     test('[Python] import libnvme', python3, args: ['-c', 'from libnvme import nvme'], env: test_env, depends: pynvme_clib)
 
     py_tests = [ 
-        [ 'create ctrl object', files('tests/create-ctrl-obj.py') ], 
-        [ 'SIGSEGV during gc', files('tests/gc.py') ],
+        [ 'create ctrl object', [ files('tests/create-ctrl-obj.py'), ] ],
+        [ 'SIGSEGV during gc', [ files('tests/gc.py'), ] ],
+        [ 'Read NBFT file', [ files('tests/test-nbft.py'), '--filename', join_paths(meson.current_source_dir(), 'tests', 'NBFT') ] ],
     ]
     foreach test: py_tests
         description = test[0]
-        py_script   = test[1]
-        test('[Python] ' + description, python3, args: [py_script, ], env: test_env, depends: pynvme_clib)
+        args = test[1]
+        test('[Python] ' + description, python3, args: args, env: test_env, depends: pynvme_clib)
     endforeach
 endif
```

### Comparing `libnvme-1.4/libnvme/nvme.i` & `libnvme-1.5/libnvme/nvme.i`

 * *Files 26% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 	#include <ccan/endian/endian.h>
 	#include "nvme/tree.h"
 	#include "nvme/fabrics.h"
 	#include "nvme/private.h"
 	#include "nvme/log.h"
 	#include "nvme/ioctl.h"
 	#include "nvme/types.h"
+	#include "nvme/nbft.h"
 
 	static int host_iter_err = 0;
 	static int subsys_iter_err = 0;
 	static int ctrl_iter_err = 0;
 	static int ns_iter_err = 0;
 	static int connect_err = 0;
 	static int discover_err = 0;
@@ -310,26 +311,28 @@
 		PyDict_SetItemStringDecRef(entry, "portid", val);
 		val = PyLong_FromLong(e->cntlid);
 		PyDict_SetItemStringDecRef(entry, "cntlid", val);
 		val = PyLong_FromLong(e->asqsz);
 		PyDict_SetItemStringDecRef(entry, "asqsz", val);
 		val = PyLong_FromLong(e->eflags);
 		PyDict_SetItemStringDecRef(entry, "eflags", val);
-		PyList_SetItem(obj, i, entry); /* steals ref. to entry */
+		PyList_SetItem(obj, i, entry); /* steals ref. to object - no need to decref */
 	}
 	$result = obj;
 };
 
 #include "tree.h"
 #include "fabrics.h"
 #define STR_OR_NONE(str) (!(str) ? "None" : str)
 
 struct nvme_root {
 	%immutable config_file;
+	%immutable application;
 	char *config_file;
+	char *application;
 };
 
 struct nvme_host {
 	%immutable hostnqn;
 	%immutable hostid;
 	%immutable hostsymname;
 	char *hostnqn;
@@ -341,18 +344,20 @@
 };
 
 struct nvme_subsystem {
 	%immutable subsysnqn;
 	%immutable model;
 	%immutable serial;
 	%immutable firmware;
+	%immutable application;
 	char *subsysnqn;
 	char *model;
 	char *serial;
 	char *firmware;
+	char *application;
 };
 
 struct nvme_ctrl {
 	%immutable sysfs_dir;
 	%immutable address;
 	%immutable firmware;
 	%immutable model;
@@ -607,15 +612,17 @@
 		$self->pos = nvme_subsystem_next_ctrl($self->subsystem, this);
 		return this;
 	}
 }
 
 %pythonappend nvme_ctrl::connect(struct nvme_host *h,
 				 struct nvme_fabrics_config *cfg) {
-    self.__parent = h  # Keep a reference to parent to ensure garbage collection happens in the right order}
+    self.__host = h  # Keep a reference to parent to ensure ctrl obj gets GCed before host}
+%pythonappend nvme_ctrl::init(struct nvme_host *h, int instance) {
+    self.__host = h  # Keep a reference to parent to ensure ctrl obj gets GCed before host}
 %extend nvme_ctrl {
 	nvme_ctrl(struct nvme_root *r,
 		  const char *subsysnqn,
 		  const char *transport,
 		  const char *traddr = NULL,
 		  const char *host_traddr = NULL,
 		  const char *host_iface = NULL,
@@ -729,15 +736,15 @@
 			Py_RETURN_NONE;
 		}
 
 		obj = PyList_New(NVME_LOG_SUPPORTED_LOG_PAGES_MAX);
 		if (!obj) Py_RETURN_NONE;
 
 		for (int i = 0; i < NVME_LOG_SUPPORTED_LOG_PAGES_MAX; i++)
-			PyList_SetItem(obj, i, PyLong_FromLong(le32_to_cpu(log.lid_support[i]))); /* steals ref. */
+			PyList_SetItem(obj, i, PyLong_FromLong(le32_to_cpu(log.lid_support[i]))); /* steals ref. to object - no need to decref */
 
 		return obj;
 	}
 
 	PyObject* __str__() {
 		return $self->address ?
 		       PyUnicode_FromFormat("nvme_ctrl(transport=%s,%s)", STR_OR_NONE($self->transport), STR_OR_NONE($self->address)) :
@@ -808,16 +815,254 @@
 
 %{
 	const char *nvme_ns_name_get(struct nvme_ns *n) {
 		return nvme_ns_get_name(n);
 	}
 %};
 
+/******
+  NBFT
+ ******/
+%{
+	static PyObject *ssns_to_dict(struct nbft_info_subsystem_ns *ss)
+	{
+		unsigned int i;
+		PyObject *output = PyDict_New();
+		PyObject *hfis = PyList_New(ss->num_hfis);
+
+		for (i = 0; i < ss->num_hfis; i++)
+			PyList_SetItem(hfis, i, PyLong_FromLong(ss->hfis[i]->index - 1)); /* steals ref. to object - no need to decref */
+
+		PyDict_SetItemStringDecRef(output, "hfi_indexes", hfis);
+
+		PyDict_SetItemStringDecRef(output, "trtype", PyUnicode_FromString(ss->transport));
+		PyDict_SetItemStringDecRef(output, "traddr", PyUnicode_FromString(ss->traddr));
+		PyDict_SetItemStringDecRef(output, "trsvcid", PyUnicode_FromString(ss->trsvcid));
+		PyDict_SetItemStringDecRef(output, "subsys_port_id", PyLong_FromLong(ss->subsys_port_id));
+		PyDict_SetItemStringDecRef(output, "nsid", PyLong_FromLong(ss->nsid));
+
+		{
+			PyObject *nid;
+			switch (ss->nid_type) {
+			case NBFT_INFO_NID_TYPE_EUI64:
+				PyDict_SetItemStringDecRef(output, "nid_type", PyUnicode_FromString("eui64"));
+				nid = PyUnicode_FromFormat("%02x%02x%02x%02x%02x%02x%02x%02x",
+							   ss->nid[0], ss->nid[1], ss->nid[2], ss->nid[3],
+							   ss->nid[4], ss->nid[5], ss->nid[6], ss->nid[7]);
+				break;
+
+			case NBFT_INFO_NID_TYPE_NGUID:
+				PyDict_SetItemStringDecRef(output, "nid_type", PyUnicode_FromString("nguid"));
+				nid = PyUnicode_FromFormat("%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x%02x",
+							   ss->nid[0], ss->nid[1], ss->nid[2], ss->nid[3],
+							   ss->nid[4], ss->nid[5], ss->nid[6], ss->nid[7],
+							   ss->nid[8], ss->nid[9], ss->nid[10], ss->nid[11],
+							   ss->nid[12], ss->nid[13], ss->nid[14], ss->nid[15]);
+				break;
+
+			case NBFT_INFO_NID_TYPE_NS_UUID:
+			{
+				char uuid_str[NVME_UUID_LEN_STRING];
+				PyDict_SetItemStringDecRef(output, "nid_type", PyUnicode_FromString("uuid"));
+				nvme_uuid_to_string(ss->nid, uuid_str);
+				nid = PyUnicode_FromString(uuid_str);
+				break;
+			}
+
+			default:
+				nid = NULL;
+				break;
+			}
+			if (nid)
+				PyDict_SetItemStringDecRef(output, "nid", nid);
+		}
+
+		if (ss->subsys_nqn)
+			PyDict_SetItemStringDecRef(output, "subsys_nqn", PyUnicode_FromString(ss->subsys_nqn));
+
+		PyDict_SetItemStringDecRef(output, "controller_id", PyLong_FromLong(ss->controller_id));
+		PyDict_SetItemStringDecRef(output, "asqsz", PyLong_FromLong(ss->asqsz));
+
+		if (ss->dhcp_root_path_string)
+			PyDict_SetItemStringDecRef(output, "dhcp_root_path_string", PyUnicode_FromString(ss->dhcp_root_path_string));
+
+		PyDict_SetItemStringDecRef(output, "pdu_header_digest_required", PyBool_FromLong(ss->pdu_header_digest_required));
+		PyDict_SetItemStringDecRef(output, "data_digest_required", PyBool_FromLong(ss->data_digest_required));
+
+		return output;
+	}
+
+	static PyObject *hfi_to_dict(struct nbft_info_hfi *hfi)
+	{
+		PyObject *output = PyDict_New();
+
+		PyDict_SetItemStringDecRef(output, "trtype", PyUnicode_FromString(hfi->transport));
+
+		if (!strcmp(hfi->transport, "tcp")) {
+			PyDict_SetItemStringDecRef(output, "pcidev",
+						   PyUnicode_FromFormat("%x:%x:%x.%x",
+									((hfi->tcp_info.pci_sbdf & 0xffff0000) >> 16),
+									((hfi->tcp_info.pci_sbdf & 0x0000ff00) >> 8),
+									((hfi->tcp_info.pci_sbdf & 0x000000f8) >> 3),
+									((hfi->tcp_info.pci_sbdf & 0x00000007) >> 0)));
+
+			PyDict_SetItemStringDecRef(output, "mac_addr",
+						   PyUnicode_FromFormat("%02x:%02x:%02x:%02x:%02x:%02x",
+									hfi->tcp_info.mac_addr[0],
+									hfi->tcp_info.mac_addr[1],
+									hfi->tcp_info.mac_addr[2],
+									hfi->tcp_info.mac_addr[3],
+									hfi->tcp_info.mac_addr[4],
+									hfi->tcp_info.mac_addr[5]));
+
+			PyDict_SetItemStringDecRef(output, "vlan", PyLong_FromLong(hfi->tcp_info.vlan));
+			PyDict_SetItemStringDecRef(output, "ip_origin", PyLong_FromLong(hfi->tcp_info.ip_origin));
+			PyDict_SetItemStringDecRef(output, "ipaddr", PyUnicode_FromString(hfi->tcp_info.ipaddr));
+			PyDict_SetItemStringDecRef(output, "subnet_mask_prefix", PyLong_FromLong(hfi->tcp_info.subnet_mask_prefix));
+			PyDict_SetItemStringDecRef(output, "gateway_ipaddr", PyUnicode_FromString(hfi->tcp_info.gateway_ipaddr));
+			PyDict_SetItemStringDecRef(output, "route_metric", PyLong_FromLong(hfi->tcp_info.route_metric));
+			PyDict_SetItemStringDecRef(output, "primary_dns_ipaddr", PyUnicode_FromString(hfi->tcp_info.primary_dns_ipaddr));
+			PyDict_SetItemStringDecRef(output, "secondary_dns_ipaddr", PyUnicode_FromString(hfi->tcp_info.secondary_dns_ipaddr));
+			PyDict_SetItemStringDecRef(output, "dhcp_server_ipaddr", PyUnicode_FromString(hfi->tcp_info.dhcp_server_ipaddr));
+
+			if (hfi->tcp_info.host_name)
+				PyDict_SetItemStringDecRef(output, "host_name", PyUnicode_FromString(hfi->tcp_info.host_name));
+
+			PyDict_SetItemStringDecRef(output, "this_hfi_is_default_route", PyBool_FromLong(hfi->tcp_info.this_hfi_is_default_route));
+			PyDict_SetItemStringDecRef(output, "dhcp_override", PyBool_FromLong(hfi->tcp_info.dhcp_override));
+		}
+
+		return output;
+	}
+
+	static PyObject *discovery_to_dict(struct nbft_info_discovery *disc)
+	{
+		PyObject *output = PyDict_New();
+
+		if (disc->security)
+			PyDict_SetItemStringDecRef(output, "security_index", PyLong_FromLong(disc->security->index));
+		if (disc->hfi)
+			PyDict_SetItemStringDecRef(output, "hfi_index", PyLong_FromLong(disc->hfi->index - 1));
+		if (disc->uri)
+			PyDict_SetItemStringDecRef(output, "uri", PyUnicode_FromString(disc->uri));
+		if (disc->nqn)
+			PyDict_SetItemStringDecRef(output, "nqn", PyUnicode_FromString(disc->nqn));
+
+		return output;
+	}
+
+	static PyObject *nbft_to_pydict(struct nbft_info *nbft)
+	{
+		PyObject *val;
+		PyObject *output = PyDict_New();
+
+		{
+			PyObject *host = PyDict_New();
+
+			if (nbft->host.nqn)
+				PyDict_SetItemStringDecRef(host, "nqn", PyUnicode_FromString(nbft->host.nqn));
+			if (nbft->host.id) {
+				char uuid_str[NVME_UUID_LEN_STRING];
+				nvme_uuid_to_string((unsigned char *)nbft->host.id, uuid_str);
+				PyDict_SetItemStringDecRef(host, "id", PyUnicode_FromString(uuid_str));
+			}
+
+			PyDict_SetItemStringDecRef(host, "host_id_configured", PyBool_FromLong(nbft->host.host_id_configured));
+			PyDict_SetItemStringDecRef(host, "host_nqn_configured", PyBool_FromLong(nbft->host.host_nqn_configured));
+
+			val = PyUnicode_FromString(nbft->host.primary == NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_NOT_INDICATED ? "not indicated" :
+						   nbft->host.primary == NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_UNSELECTED ? "unselected" :
+						   nbft->host.primary == NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_SELECTED ? "selected" : "reserved");
+			PyDict_SetItemStringDecRef(host, "primary_admin_host_flag", val);
+
+			PyDict_SetItemStringDecRef(output, "host", host);
+		}
+
+		{
+			size_t ss_num = 0;
+			struct nbft_info_subsystem_ns **ss;
+			PyObject *subsystem;
+
+			/* First, let's find how many entries there are */
+			for (ss = nbft->subsystem_ns_list; ss && *ss; ss++)
+				ss_num++;
+
+			/* Now, let's fill the list using "(*ss)->index - 1"
+			   as the index for writing to the list */
+			subsystem = PyList_New(ss_num);
+			for (ss = nbft->subsystem_ns_list; ss && *ss; ss++)
+				PyList_SetItem(subsystem, (*ss)->index - 1, ssns_to_dict(*ss)); /* steals ref. to object - no need to decref */
+
+			PyDict_SetItemStringDecRef(output, "subsystem", subsystem);
+		}
+
+		{
+			size_t hfi_num = 0;
+			struct nbft_info_hfi **hfi;
+			PyObject *hfis;
+
+			/* First, let's find how many entries there are */
+			for (hfi = nbft->hfi_list; hfi && *hfi; hfi++)
+				hfi_num++;
+
+			/* Now, let's fill the list using "(*hfi)->index - 1"
+			   as the index for writing to the list */
+			hfis = PyList_New(hfi_num);
+			for (hfi = nbft->hfi_list; hfi && *hfi; hfi++)
+				PyList_SetItem(hfis, (*hfi)->index-1, hfi_to_dict(*hfi)); /* steals ref. to object - no need to decref */
+
+			PyDict_SetItemStringDecRef(output, "hfi", hfis);
+		}
+
+		{
+			size_t disc_num = 0;
+			struct nbft_info_discovery **disc;
+			PyObject *discovery;
+
+			/* First, let's find how many entries there are */
+			for (disc = nbft->discovery_list; disc && *disc; disc++)
+				disc_num++;
+
+			/* Now, let's fill the list using "(*disc)->index - 1"
+			   as the index for writing to the list */
+			discovery = PyList_New(disc_num);
+			for (disc = nbft->discovery_list; disc && *disc; disc++)
+				PyList_SetItem(discovery, (*disc)->index - 1, discovery_to_dict(*disc)); /* steals ref. to object - no need to decref */
+
+			PyDict_SetItemStringDecRef(output, "discovery", discovery);
+		}
+
+		/* Security profiles are currently not implemented. */
+
+		return output;
+	}
+
+	PyObject *nbft_get(const char * filename)
+	{
+		struct nbft_info *nbft;
+		PyObject *output;
+		int ret;
+
+		ret = nvme_nbft_read(&nbft, filename);
+		if (ret) {
+			Py_RETURN_NONE;
+		}
+
+		output = nbft_to_pydict(nbft);
+		nvme_nbft_free(nbft);
+		return output;
+	}
+%};
+
+%feature("autodoc", "@return an NBFT table as a dict on success, None otherwise.\n"
+		    "@param filename: file to read") nbft_get;
+PyObject *nbft_get(const char * filename);
 
 // We want to swig all the #define and enum from types.h, but none of the structs.
+#pragma SWIG nowarn=503             // Supress warnings about unnamed struct
 #define __attribute__(x)
 %rename($ignore, %$isclass) "";     // ignore all classes/structs
 %rename($ignore, %$isfunction) "";  // ignore all functions
 %rename($ignore, %$isunion) "";     // ignore all unions
-%rename($ignore, %$isvariable ) ""; // ignore all variables
+%rename($ignore, %$isvariable) "";  // ignore all variables
 
 %include "../src/nvme/types.h"
```

### Comparing `libnvme-1.4/libnvme/tests/gc.py` & `libnvme-1.5/libnvme/tests/gc.py`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/libnvme.spec.in` & `libnvme-1.5/libnvme.spec.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/meson-vcs-tag.sh` & `libnvme-1.5/scripts/meson-vcs-tag.sh`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/meson.build` & `libnvme-1.5/meson.build`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # Copyright (c) 2021 Dell Inc.
 #
 # Authors: Martin Belanger <Martin.Belanger@dell.com>
 #
 project(
     'libnvme', ['c'],
     meson_version: '>= 0.50.0',
-    version: '1.4',
+    version: '1.5',
     license: 'LGPL-2.1-or-later',
     default_options: [
         'c_std=gnu99',
         'warning_level=1',
         'buildtype=debug',
         'prefix=/usr/local',
         'sysconfdir=etc',
+        'wrap_mode=nofallback'
     ]
 )
 
 maj_min = meson.project_version().split('-rc')[0]
 library_version =  maj_min + '.0'
 
 ################################################################################
@@ -37,30 +38,30 @@
 ################################################################################
 conf = configuration_data()
 
 version_tag = get_option('version-tag')
 if version_tag != ''
         conf.set('GIT_VERSION', '"@0@"'.format(version_tag))
 else
-    r = run_command('meson-vcs-tag.sh',
+    r = run_command('scripts/meson-vcs-tag.sh',
                     meson.current_source_dir(),
                     meson.project_version(),
                     check: true)
     conf.set('GIT_VERSION', '"@0@"'.format(r.stdout().strip()))
 endif
 conf.set('PROJECT_VERSION', '"@0@"'.format(meson.project_version()))
 
 conf.set('SYSCONFDIR', '"@0@"'.format(sysconfdir))
 
 if get_option('json-c').disabled()
     json_c_dep = dependency('', required: false)
 else
     json_c_dep = dependency('json-c',
                             version: '>=0.13',
-                            required: true,
+                            required: get_option('json-c'),
                             fallback : ['json-c', 'json_c_dep'])
 endif
 conf.set('CONFIG_JSONC', json_c_dep.found(), description: 'Is json-c required?')
 
 if get_option('openssl').disabled()
   openssl_dep = dependency('', required: false)
 else
@@ -211,25 +212,25 @@
         '''#include <linux/mctp.h>''',
         name: 'linux/mctp.h'
     ),
     description: 'Is linux/mctp.h include-able?'
 )
 
 conf.set(
-    'HAVE_LIBNSS',
+    'HAVE_NETDB',
     cc.links(
       '''#include <sys/types.h>
          #include <sys/socket.h>
          #include <netdb.h>
          int main(int argc, char **argv) {
              struct addrinfo hints, *result;
              return getaddrinfo(argv[1], argv[2], &hints, &result);
       }
       ''',
-      name: 'libnss',
+      name: 'netdb',
     ),
     description: 'Is network address and service translation available'
 )
 
 if cc.has_function_attribute('fallthrough')
   conf.set('fallthrough', '__attribute__((__fallthrough__))')
 else
@@ -265,19 +266,27 @@
 subdir('libnvme')
 subdir('test')
 subdir('examples')
 subdir('doc')
 
 ################################################################################
 if meson.version().version_compare('>=0.53.0')
-    summary_dict = {
+    path_dict = {
         'prefixdir':         prefixdir,
         'sysconfdir':        sysconfdir,
         'bindir':            bindir,
         'includedir':        includedir,
         'datadir':           datadir,
         'mandir':            mandir,
         'libdir':            libdir,
         'build location':    meson.current_build_dir(),
     }
-    summary(summary_dict)
+    summary(path_dict, section: 'Paths')
+    dep_dict = {
+        'json-c':            json_c_dep.found(),
+        'OpenSSL':           openssl_dep.found(),
+        'keyutitls':         keyutils_dep.found(),
+        'libdbus':           libdbus_dep.found(),
+        'Python 3':          py3_dep.found(),
+    }
+    summary(dep_dict, section: 'Dependencies')
 endif
```

### Comparing `libnvme-1.4/meson_options.txt` & `libnvme-1.5/meson_options.txt`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/pyproject.toml` & `libnvme-1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/libnvme-mi.map` & `libnvme-1.5/src/libnvme-mi.map`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+LIBNVME_MI_1_5 {
+	global:
+		nvme_mi_ctrl_id;
+};
+
 LIBNVME_MI_1_4 {
         global:
                 nvme_mi_admin_get_log_page;
 };
 
 LIBNVME_MI_1_3 {
 	global:
```

### Comparing `libnvme-1.4/src/libnvme.h` & `libnvme-1.5/src/libnvme.h`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include "nvme/types.h"
 #include "nvme/linux.h"
 #include "nvme/ioctl.h"
+#include "nvme/nbft.h"
 #include "nvme/fabrics.h"
 #include "nvme/filters.h"
 #include "nvme/tree.h"
 #include "nvme/util.h"
 #include "nvme/log.h"
 
 #ifdef __cplusplus
```

### Comparing `libnvme-1.4/src/libnvme.map` & `libnvme-1.5/src/libnvme.map`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
+LIBNVME_1_5 {
+	global:
+		nvme_ctrl_get_phy_slot;
+		nvme_ipaddrs_eq;
+		nvme_nbft_free;
+		nvme_nbft_read;
+		nvme_root_get_application;
+		nvme_root_set_application;
+		nvme_subsystem_get_application;
+		nvme_subsystem_set_application;
+};
+
 LIBNVME_1_4 {
 	global:
 		nvme_lookup_keyring;
 		nvme_describe_key_serial;
 		nvme_lookup_key;
 		nvme_set_keyring;
 		nvme_insert_tls_key;
```

### Comparing `libnvme-1.4/src/meson.build` & `libnvme-1.5/src/meson.build`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # This file is part of libnvme.
 # Copyright (c) 2021 Dell Inc.
 #
 # Authors: Martin Belanger <Martin.Belanger@dell.com>
 #
 sources = [
     'nvme/cleanup.c',
+    'nvme/nbft.c',
     'nvme/fabrics.c',
     'nvme/filters.c',
     'nvme/ioctl.c',
     'nvme/linux.c',
     'nvme/log.c',
     'nvme/tree.c',
     'nvme/util.c',
@@ -121,14 +122,15 @@
 install_headers([
         'nvme/api-types.h',
         'nvme/fabrics.h',
         'nvme/filters.h',
         'nvme/ioctl.h',
         'nvme/linux.h',
         'nvme/log.h',
+        'nvme/nbft.h',
         'nvme/tree.h',
         'nvme/types.h',
         'nvme/util.h',
         'nvme/mi.h',
     ],
     subdir: 'nvme',
     install_mode: mode,
```

### Comparing `libnvme-1.4/src/nvme/api-types.h` & `libnvme-1.5/src/nvme/api-types.h`

 * *Files 1% similar despite different names*

```diff
@@ -192,24 +192,30 @@
  * @ns:		Namespace identification descriptors
  * @args_size:	Size of &struct nvme_ns_mgmt_args
  * @fd:		File descriptor of nvme device
  * @timeout:	Timeout in ms
  * @nsid:	Namespace identifier
  * @sel:	Type of management operation to perform
  * @csi:	Command Set Identifier
+ * @rsvd1:	Reserved
+ * @rsvd2:	Reserved
+ * @data:	Host Software Specified Fields
  */
 struct nvme_ns_mgmt_args {
 	__u32 *result;
 	struct nvme_id_ns *ns;
 	int args_size;
 	int fd;
 	__u32 timeout;
 	__u32 nsid;
 	enum nvme_ns_mgmt_sel sel;
 	__u8 csi;
+	__u8 rsvd1[3];
+	void *rsvd2;
+	struct nvme_ns_mgmt_host_sw_specified *data;
 };
 
 /**
  * struct nvme_ns_attach_args - Arguments for Nvme Namespace Management command
  * @result:	NVMe command result
  * @ctrlist:	Controller list to modify attachment state of nsid
  * @args_size:	Size of &struct nvme_ns_attach_args
```

### Comparing `libnvme-1.4/src/nvme/fabrics.c` & `libnvme-1.5/src/nvme/fabrics.c`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #include <arpa/inet.h>
 #include <netdb.h>
 #include <net/if.h>
 
 #include <ccan/endian/endian.h>
 #include <ccan/list/list.h>
 #include <ccan/array_size/array_size.h>
+#include <ccan/str/str.h>
 
 #include "fabrics.h"
 #include "linux.h"
 #include "ioctl.h"
 #include "util.h"
 #include "log.h"
 #include "private.h"
@@ -191,14 +192,45 @@
 };
 
 const char *nvmf_cms_str(__u8 cm)
 {
 	return arg_str(cms, ARRAY_SIZE(cms), cm);
 }
 
+/*
+ * Derived from Linux's supported options (the opt_tokens table)
+ * when the mechanism to report supported options was added (f18ee3d988157).
+ * Not all of these options may actually be supported,
+ * but we retain the old behavior of passing all that might be.
+ */
+static const struct nvme_fabric_options default_supported_options = {
+	.ctrl_loss_tmo = true,
+	.data_digest = true,
+	.disable_sqflow = true,
+	.discovery = true,
+	.duplicate_connect = true,
+	.fast_io_fail_tmo = true,
+	.hdr_digest = true,
+	.host_iface = true,
+	.host_traddr = true,
+	.hostid = true,
+	.hostnqn = true,
+	.keep_alive_tmo = true,
+	.nqn = true,
+	.nr_io_queues = true,
+	.nr_poll_queues = true,
+	.nr_write_queues = true,
+	.queue_size = true,
+	.reconnect_delay = true,
+	.tos = true,
+	.traddr = true,
+	.transport = true,
+	.trsvcid = true,
+};
+
 void nvmf_default_config(struct nvme_fabrics_config *cfg)
 {
 	memset(cfg, 0, sizeof(*cfg));
 	cfg->tos = -1;
 	cfg->ctrl_loss_tmo = NVMF_DEF_CTRL_LOSS_TMO;
 }
 
@@ -257,15 +289,15 @@
 	UPDATE_CFG_OPTION(ctrl_cfg, cfg, duplicate_connect, false);
 	UPDATE_CFG_OPTION(ctrl_cfg, cfg, disable_sqflow, false);
 	UPDATE_CFG_OPTION(ctrl_cfg, cfg, hdr_digest, false);
 	UPDATE_CFG_OPTION(ctrl_cfg, cfg, data_digest, false);
 	UPDATE_CFG_OPTION(ctrl_cfg, cfg, tls, false);
 }
 
-static int add_bool_argument(char **argstr, char *tok, bool arg)
+static int __add_bool_argument(char **argstr, char *tok, bool arg)
 {
 	char *nstr;
 
 	if (!arg)
 		return 0;
 	if (asprintf(&nstr, "%s,%s", *argstr, tok) < 0) {
 		errno = ENOMEM;
@@ -273,15 +305,15 @@
 	}
 	free(*argstr);
 	*argstr = nstr;
 
 	return 0;
 }
 
-static int add_int_argument(char **argstr, char *tok, int arg, bool allow_zero)
+static int __add_int_argument(char **argstr, char *tok, int arg, bool allow_zero)
 {
 	char *nstr;
 
 	if (arg < 0 || (!arg && !allow_zero))
 		return 0;
 	if (asprintf(&nstr, "%s,%s=%d", *argstr, tok, arg) < 0) {
 		errno = ENOMEM;
@@ -289,15 +321,15 @@
 	}
 	free(*argstr);
 	*argstr = nstr;
 
 	return 0;
 }
 
-static int add_int_or_minus_one_argument(char **argstr, char *tok, int arg)
+static int __add_int_or_minus_one_argument(char **argstr, char *tok, int arg)
 {
 	char *nstr;
 
 	if (arg < -1)
 		return 0;
 	if (asprintf(&nstr, "%s,%s=%d", *argstr, tok, arg) < 0) {
 		errno = ENOMEM;
@@ -305,15 +337,15 @@
 	}
 	free(*argstr);
 	*argstr = nstr;
 
 	return 0;
 }
 
-static int add_argument(char **argstr, const char *tok, const char *arg)
+static int __add_argument(char **argstr, const char *tok, const char *arg)
 {
 	char *nstr;
 
 	if (!arg || arg[0] == '\0' || !strcmp(arg, "none"))
 		return 0;
 	if (asprintf(&nstr, "%s,%s=%s", *argstr, tok, arg) < 0) {
 		errno = ENOMEM;
@@ -321,14 +353,79 @@
 	}
 	free(*argstr);
 	*argstr = nstr;
 
 	return 0;
 }
 
+#define add_bool_argument(o, argstr, tok, arg)				\
+({									\
+	int ret;							\
+	if (r->options->tok) {						\
+		ret = __add_bool_argument(argstr,			\
+					  stringify(tok),		\
+					  arg);				\
+	} else {							\
+		nvme_msg(r, LOG_DEBUG,					\
+			 "option \"%s\" ignored\n",			\
+			 stringify(tok));				\
+		ret = 0;						\
+	}								\
+	ret;								\
+})
+
+#define add_int_argument(o, argstr, tok, arg, allow_zero) \
+({									\
+	int ret;							\
+	if (r->options->tok) {						\
+		ret = __add_int_argument(argstr,			\
+					stringify(tok),			\
+					arg,				\
+					allow_zero);			\
+	} else {							\
+		nvme_msg(r, LOG_DEBUG,					\
+			 "option \"%s\" ignored\n",			\
+			 stringify(tok));				\
+		ret = 0;						\
+	}								\
+	ret;								\
+})
+
+#define add_int_or_minus_one_argument(o, argstr, tok, arg)		\
+({									\
+	int ret;							\
+	if (r->options->tok) {						\
+		ret = __add_int_or_minus_one_argument(argstr,		\
+						     stringify(tok),	\
+						     arg);		\
+	} else {							\
+		nvme_msg(r, LOG_DEBUG,					\
+			 "option \"%s\" ignored\n",			\
+			 stringify(tok));				\
+		ret = 0;						\
+	}								\
+	ret;								\
+})
+
+#define add_argument(r, argstr, tok, arg)				\
+({									\
+	int ret;							\
+	if (r->options->tok) {						\
+		ret = __add_argument(argstr,				\
+				     stringify(tok),			\
+				     arg);				\
+	} else {							\
+		nvme_msg(r, LOG_NOTICE,					\
+			 "option \"%s\" ignored\n",			\
+			 stringify(tok));				\
+		ret = 0;						\
+	}								\
+	ret;								\
+})
+
 static int inet4_pton(const char *src, uint16_t port,
 		      struct sockaddr_storage *addr)
 {
 	struct sockaddr_in *addr4 = (struct sockaddr_in *)addr;
 
 	if (strlen(src) > INET_ADDRSTRLEN)
 		return -EINVAL;
@@ -449,14 +546,15 @@
 
 static int build_options(nvme_host_t h, nvme_ctrl_t c, char **argstr)
 {
 	struct nvme_fabrics_config *cfg = nvme_ctrl_get_config(c);
 	const char *transport = nvme_ctrl_get_transport(c);
 	const char *hostnqn, *hostid, *hostkey, *ctrlkey;
 	bool discover = false, discovery_nqn = false;
+	nvme_root_t r = h->r;
 
 	if (!transport) {
 		nvme_msg(h->r, LOG_ERR, "need a transport (-t) argument\n");
 		errno = ENVME_CONNECT_TARG;
 		return -1;
 	}
 
@@ -483,75 +581,174 @@
 		discover = true;
 	hostnqn = nvme_host_get_hostnqn(h);
 	hostid = nvme_host_get_hostid(h);
 	hostkey = nvme_host_get_dhchap_key(h);
 	if (!hostkey)
 		hostkey = nvme_ctrl_get_dhchap_host_key(c);
 	ctrlkey = nvme_ctrl_get_dhchap_key(c);
-	if (add_argument(argstr, "transport", transport) ||
-	    add_argument(argstr, "traddr",
+	if (add_argument(r, argstr, transport, transport) ||
+	    add_argument(r, argstr, traddr,
 			 nvme_ctrl_get_traddr(c)) ||
-	    add_argument(argstr, "host_traddr",
+	    add_argument(r, argstr, host_traddr,
 			 cfg->host_traddr) ||
-	    add_argument(argstr, "host_iface",
+	    add_argument(r, argstr, host_iface,
 			 cfg->host_iface) ||
-	    add_argument(argstr, "trsvcid",
+	    add_argument(r, argstr, trsvcid,
 			 nvme_ctrl_get_trsvcid(c)) ||
-	    (hostnqn && add_argument(argstr, "hostnqn", hostnqn)) ||
-	    (hostid && add_argument(argstr, "hostid", hostid)) ||
+	    (hostnqn && add_argument(r, argstr, hostnqn, hostnqn)) ||
+	    (hostid && add_argument(r, argstr, hostid, hostid)) ||
 	    (discover && !discovery_nqn &&
-	     add_bool_argument(argstr, "discovery", true)) ||
+	     add_bool_argument(r, argstr, discovery, true)) ||
 	    (!discover && hostkey &&
-	     add_argument(argstr, "dhchap_secret", hostkey)) ||
+	     add_argument(r, argstr, dhchap_secret, hostkey)) ||
 	    (!discover && ctrlkey &&
-	     add_argument(argstr, "dhchap_ctrl_secret", ctrlkey)) ||
+	     add_argument(r, argstr, dhchap_ctrl_secret, ctrlkey)) ||
 	    (!discover &&
-	     add_int_argument(argstr, "nr_io_queues",
+	     add_int_argument(r, argstr, nr_io_queues,
 			      cfg->nr_io_queues, false)) ||
 	    (!discover &&
-	     add_int_argument(argstr, "nr_write_queues",
+	     add_int_argument(r, argstr, nr_write_queues,
 			      cfg->nr_write_queues, false)) ||
 	    (!discover &&
-	     add_int_argument(argstr, "nr_poll_queues",
+	     add_int_argument(r, argstr, nr_poll_queues,
 			      cfg->nr_poll_queues, false)) ||
 	    (!discover &&
-	     add_int_argument(argstr, "queue_size",
+	     add_int_argument(r, argstr, queue_size,
 			      cfg->queue_size, false)) ||
-	    add_int_argument(argstr, "keep_alive_tmo",
+	    add_int_argument(r, argstr, keep_alive_tmo,
 			     cfg->keep_alive_tmo, false) ||
-	    add_int_argument(argstr, "reconnect_delay",
+	    add_int_argument(r, argstr, reconnect_delay,
 			     cfg->reconnect_delay, false) ||
 	    (strcmp(transport, "loop") &&
-	     add_int_or_minus_one_argument(argstr, "ctrl_loss_tmo",
+	     add_int_or_minus_one_argument(r, argstr, ctrl_loss_tmo,
 			      cfg->ctrl_loss_tmo)) ||
 	    (strcmp(transport, "loop") &&
-	     add_int_argument(argstr, "fast_io_fail_tmo",
+	     add_int_argument(r, argstr, fast_io_fail_tmo,
 			      cfg->fast_io_fail_tmo, false)) ||
 	    (strcmp(transport, "loop") &&
-	     add_int_argument(argstr, "tos", cfg->tos, true)) ||
-	    add_int_argument(argstr, "keyring", cfg->keyring, false) ||
+	     add_int_argument(r, argstr, tos, cfg->tos, true)) ||
+	    add_int_argument(r, argstr, keyring, cfg->keyring, false) ||
 	    (!strcmp(transport, "tcp") &&
-	     add_int_argument(argstr, "tls_key", cfg->tls_key, false)) ||
-	    add_bool_argument(argstr, "duplicate_connect",
+	     add_int_argument(r, argstr, tls_key, cfg->tls_key, false)) ||
+	    add_bool_argument(r, argstr, duplicate_connect,
 			      cfg->duplicate_connect) ||
-	    add_bool_argument(argstr, "disable_sqflow",
+	    add_bool_argument(r, argstr, disable_sqflow,
 			      cfg->disable_sqflow) ||
 	    (!strcmp(transport, "tcp") &&
-	     add_bool_argument(argstr, "hdr_digest", cfg->hdr_digest)) ||
+	     add_bool_argument(r, argstr, hdr_digest, cfg->hdr_digest)) ||
 	    (!strcmp(transport, "tcp") &&
-	     add_bool_argument(argstr, "data_digest", cfg->data_digest)) ||
+	     add_bool_argument(r, argstr, data_digest, cfg->data_digest)) ||
 	    (!strcmp(transport, "tcp") &&
-	     add_bool_argument(argstr, "tls", cfg->tls))) {
+	     add_bool_argument(r, argstr, tls, cfg->tls))) {
 		free(*argstr);
 		return -1;
 	}
 
 	return 0;
 }
 
+#define parse_option(r, v, name)	   \
+	if (!strcmp(v, stringify(name))) { \
+		r->options->name = true;   \
+		continue;		   \
+	}
+
+static  int __nvmf_supported_options(nvme_root_t r)
+{
+	char buf[0x1000], *options, *p, *v;
+	int fd, ret;
+	ssize_t len;
+
+	if (r->options)
+		return 0;
+
+	r->options = calloc(1, sizeof(*r->options));
+	if (!r->options)
+		return -ENOMEM;
+
+	fd = open(nvmf_dev, O_RDONLY);
+	if (fd < 0) {
+		nvme_msg(r, LOG_ERR, "Failed to open %s: %s\n",
+			 nvmf_dev, strerror(errno));
+		return -ENVME_CONNECT_OPEN;
+	}
+
+	memset(buf, 0x0, sizeof(buf));
+	len = read(fd, buf, sizeof(buf) - 1);
+	if (len < 0) {
+		if (errno == EINVAL) {
+			/*
+			 * Older Linux kernels don't allow reading from nvmf_dev
+			 * to get supported options, so use a default set
+			 */
+			nvme_msg(r, LOG_DEBUG,
+			         "Cannot read %s, using default options\n",
+			         nvmf_dev);
+			*r->options = default_supported_options;
+			ret = 0;
+			goto out_close;
+		}
+
+		nvme_msg(r, LOG_ERR, "Failed to read from %s: %s\n",
+			 nvmf_dev, strerror(errno));
+		ret = -ENVME_CONNECT_READ;
+		goto out_close;
+	}
+
+	buf[len] = '\0';
+	options = buf;
+
+	nvme_msg(r, LOG_DEBUG, "kernel supports: ");
+
+	while ((p = strsep(&options, ",\n")) != NULL) {
+		if (!*p)
+			continue;
+		v = strsep(&p, "= ");
+		if (!v)
+			continue;
+		nvme_msg(r, LOG_DEBUG, "%s ", v);
+
+		parse_option(r, v, cntlid);
+		parse_option(r, v, ctrl_loss_tmo);
+		parse_option(r, v, data_digest);
+		parse_option(r, v, dhchap_ctrl_secret);
+		parse_option(r, v, dhchap_secret);
+		parse_option(r, v, disable_sqflow);
+		parse_option(r, v, discovery);
+		parse_option(r, v, duplicate_connect);
+		parse_option(r, v, fast_io_fail_tmo);
+		parse_option(r, v, hdr_digest);
+		parse_option(r, v, host_iface);
+		parse_option(r, v, host_traddr);
+		parse_option(r, v, hostid);
+		parse_option(r, v, hostnqn);
+		parse_option(r, v, instance);
+		parse_option(r, v, keep_alive_tmo);
+		parse_option(r, v, keyring);
+		parse_option(r, v, nqn);
+		parse_option(r, v, nr_io_queues);
+		parse_option(r, v, nr_poll_queues);
+		parse_option(r, v, nr_write_queues);
+		parse_option(r, v, queue_size);
+		parse_option(r, v, reconnect_delay);
+		parse_option(r, v, tls);
+		parse_option(r, v, tls_key);
+		parse_option(r, v, tos);
+		parse_option(r, v, traddr);
+		parse_option(r, v, transport);
+		parse_option(r, v, trsvcid);
+	}
+	nvme_msg(r, LOG_DEBUG, "\n");
+	ret = 0;
+
+out_close:
+	close(fd);
+	return ret;
+}
+
 static int __nvmf_add_ctrl(nvme_root_t r, const char *argstr)
 {
 	int ret, fd, len = strlen(argstr);
 	char buf[0x1000], *options, *p;
 
 	fd = open(nvmf_dev, O_RDWR);
 	if (fd < 0) {
@@ -578,17 +775,20 @@
 			break;
 		case ENODEV:
 			ret = -ENVME_CONNECT_NODEV;
 			break;
 		case EOPNOTSUPP:
 			ret = -ENVME_CONNECT_OPNOTSUPP;
 			break;
-		case ECONNREFUSED :
+		case ECONNREFUSED:
 			ret = -ENVME_CONNECT_CONNREFUSED;
 			break;
+		case EADDRNOTAVAIL:
+			ret = -ENVME_CONNECT_ADDRNOTAVAIL;
+			break;
 		default:
 			ret = -ENVME_CONNECT_WRITE;
 			break;
 		}
 		goto out_close;
 	}
 
@@ -618,14 +818,15 @@
 	return ret;
 }
 
 int nvmf_add_ctrl(nvme_host_t h, nvme_ctrl_t c,
 		  const struct nvme_fabrics_config *cfg)
 {
 	nvme_subsystem_t s;
+	const char *root_app, *app;
 	char *argstr;
 	int ret;
 
 	/* highest prio have configs from command line */
 	cfg = merge_config(c, cfg);
 
 	/* apply configuration from config file (JSON) */
@@ -654,27 +855,65 @@
 			key = nvme_ctrl_get_dhchap_key(fc);
 			if (key)
 				nvme_ctrl_set_dhchap_key(c, key);
 		}
 
 	}
 
+	root_app = nvme_root_get_application(h->r);
+	if (root_app) {
+		app = nvme_subsystem_get_application(s);
+		if (!app && nvme_ctrl_is_discovery_ctrl(c)) {
+			nvme_subsystem_t s;
+			nvme_ctrl_t fc;
+
+			nvme_for_each_subsystem(h, s) {
+				fc = __nvme_lookup_ctrl(s, nvme_ctrl_get_transport(c),
+							nvme_ctrl_get_traddr(c),
+							NULL,
+							NULL,
+							nvme_ctrl_get_trsvcid(c),
+							NULL);
+
+				if (fc) {
+					app = nvme_subsystem_get_application(s);
+					break;
+				}
+			}
+		}
+		/*
+		 * configuration is managed by an application,
+		 * refuse to act on subsystems which either have
+		 * no application set or which habe a different
+		 * application string.
+		 */
+		if (app && strcmp(app, root_app)) {
+			nvme_msg(h->r, LOG_INFO, "skip %s, not managed by %s\n",
+				 nvme_subsystem_get_nqn(s), root_app);
+			errno = ENVME_CONNECT_IGNORED;
+			return -1;
+		}
+	}
+
 	nvme_ctrl_set_discovered(c, true);
 	if (traddr_is_hostname(h->r, c)) {
 		char *traddr = c->traddr;
 
 		c->traddr = hostname2traddr(h->r, traddr);
 		if (!c->traddr) {
 			c->traddr = traddr;
 			errno = ENVME_CONNECT_TRADDR;
 			return -1;
 		}
 		free(traddr);
 	}
 
+	ret = __nvmf_supported_options(h->r);
+	if (ret)
+		return ret;
 	ret = build_options(h, c, &argstr);
 	if (ret)
 		return ret;
 
 	ret = __nvmf_add_ctrl(h->r, argstr);
 	free(argstr);
 	if (ret < 0) {
@@ -832,17 +1071,18 @@
 			errno = ENOMEM;
 			return NULL;
 		}
 
 		nvme_msg(r, LOG_DEBUG, "%s: get header (try %d/%d)\n",
 			name, retries, max_retries);
 		args->rae = true;
+		args->lpo = 0;
 		args->len = size;
 		args->log = log;
-		ret = nvme_get_log_page(fd, 4096, args);
+		ret = nvme_get_log_page(fd, NVME_LOG_PAGE_PDU_SIZE, args);
 		if (ret) {
 			nvme_msg(r, LOG_INFO,
 				 "%s: discover try %d/%d failed, error %d\n",
 				 name, retries, max_retries, errno);
 			goto out_free_log;
 		}
 
@@ -861,38 +1101,57 @@
 			nvme_msg(r, LOG_ERR,
 				 "could not alloc memory for discovery log page\n");
 			errno = ENOMEM;
 			return NULL;
 		}
 
 		nvme_msg(r, LOG_DEBUG,
-			 "%s: get header and %" PRIu64
+			 "%s: get %" PRIu64
 			 " records (length %d genctr %" PRIu64 ")\n",
 			 name, numrec, size, genctr);
 
+		args->rae = true;
+		args->lpo = sizeof(struct nvmf_discovery_log);
+		args->len = size - sizeof(struct nvmf_discovery_log);
+		args->log = log->entries;
+		ret = nvme_get_log_page(fd, NVME_LOG_PAGE_PDU_SIZE, args);
+		if (ret) {
+			nvme_msg(r, LOG_INFO,
+				 "%s: discover try %d/%d failed, error %d\n",
+				 name, retries, max_retries, errno);
+			goto out_free_log;
+		}
+
+		/*
+		 * If the log page was read with multiple Get Log Page commands,
+		 * genctr must be checked afterwards to ensure atomicity
+		 */
+		nvme_msg(r, LOG_DEBUG, "%s: get header again\n", name);
+
 		args->rae = false;
-		args->len = size;
+		args->lpo = 0;
+		args->len = sizeof(struct nvmf_discovery_log);
 		args->log = log;
-		ret = nvme_get_log_page(fd, 4096, args);
-
+		ret = nvme_get_log_page(fd, NVME_LOG_PAGE_PDU_SIZE, args);
 		if (ret) {
 			nvme_msg(r, LOG_INFO,
 				 "%s: discover try %d/%d failed, error %d\n",
 				 name, retries, max_retries, errno);
 			goto out_free_log;
 		}
 	} while (genctr != le64_to_cpu(log->genctr) &&
 		 ++retries < max_retries);
 
 	if (genctr != le64_to_cpu(log->genctr)) {
 		nvme_msg(r, LOG_INFO, "%s: discover genctr mismatch\n", name);
 		errno = EAGAIN;
 	} else if (numrec != le64_to_cpu(log->numrec)) {
 		nvme_msg(r, LOG_INFO,
-			 "%s: could only fetch %" PRIu64 " of %" PRIu64 " records\n",
+			 "%s: numrec changed unexpectedly "
+			 "from %" PRIu64 " to %" PRIu64 "\n",
 			 name, numrec, le64_to_cpu(log->numrec));
 		errno = EBADSLT;
 	} else {
 		return log;
 	}
 
 out_free_log:
```

### Comparing `libnvme-1.4/src/nvme/fabrics.h` & `libnvme-1.5/src/nvme/fabrics.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/filters.c` & `libnvme-1.5/src/nvme/filters.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/filters.h` & `libnvme-1.5/src/nvme/filters.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/ioctl.c` & `libnvme-1.5/src/nvme/ioctl.c`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
 	return nvme_submit_admin_passthru(args->fd, &cmd, args->result);
 }
 
 int nvme_get_log_page(int fd, __u32 xfer_len, struct nvme_get_log_args *args)
 {
 	__u64 offset = 0, xfer, data_len = args->len;
 	__u64 start = args->lpo;
-	bool retain = true;
+	bool retain = args->rae;
 	void *ptr = args->log;
 	int ret;
 
 	args->fd = fd;
 
 	/*
 	 * 4k is the smallest possible transfer unit, so restricting to 4k
@@ -450,21 +450,18 @@
 			xfer  = xfer_len;
 
 		/*
 		 * Always retain regardless of the RAE parameter until the very
 		 * last portion of this log page so the data remains latched
 		 * during the fetch sequence.
 		 */
-		if (offset + xfer == data_len)
-			retain = args->rae;
-
 		args->lpo = start + offset;
 		args->len = xfer;
 		args->log = ptr;
-		args->rae = retain;
+		args->rae = offset + xfer < data_len || retain;
 		ret = nvme_get_log(args);
 		if (ret)
 			return ret;
 
 		offset += xfer;
 		ptr += xfer;
 	} while (offset < data_len);
@@ -1231,31 +1228,43 @@
 	};
 
 	return nvme_submit_admin_passthru(args->fd, &cmd, args->result);
 }
 
 int nvme_ns_mgmt(struct nvme_ns_mgmt_args *args)
 {
+	const size_t size_v1 = sizeof_args(struct nvme_ns_mgmt_args, csi, __u64);
+	const size_t size_v2 = sizeof_args(struct nvme_ns_mgmt_args, data, __u64);
 	__u32 cdw10    = NVME_SET(args->sel, NAMESPACE_MGMT_CDW10_SEL);
 	__u32 cdw11    = NVME_SET(args->csi, NAMESPACE_MGMT_CDW11_CSI);
-	__u32 data_len = args->ns ? sizeof(*args->ns) : 0;
+
+	if (args->args_size < size_v1 || args->args_size > size_v2) {
+		errno = EINVAL;
+		return -1;
+	}
 
 	struct nvme_passthru_cmd cmd = {
 		.nsid	    = args->nsid,
 		.opcode	    = nvme_admin_ns_mgmt,
 		.cdw10	    = cdw10,
 		.cdw11	    = cdw11,
 		.timeout_ms = args->timeout,
-		.data_len   = data_len,
-		.addr	    = (__u64)(uintptr_t)args->ns,
 	};
 
-	if (args->args_size < sizeof(*args)) {
-		errno = EINVAL;
-		return -1;
+	if (args->args_size == size_v2) {
+		if (args->data) {
+			cmd.data_len = sizeof(*args->data);
+			cmd.addr = (__u64)(uintptr_t)args->data;
+		}
+	}
+	else {
+		if (args->ns) {
+			cmd.data_len = sizeof(*args->ns);
+			cmd.addr = (__u64)(uintptr_t)args->ns;
+		}
 	}
 	return nvme_submit_admin_passthru(args->fd, &cmd, args->result);
 }
 
 int nvme_ns_attach(struct nvme_ns_attach_args *args)
 {
 	__u32 cdw10 = NVME_SET(args->sel, NAMESPACE_ATTACH_CDW10_SEL);
@@ -1897,15 +1906,15 @@
 		return -1;
 	}
 	return nvme_submit_io_passthru(args->fd, &cmd, args->result);
 }
 
 int nvme_io_mgmt_recv(struct nvme_io_mgmt_recv_args *args)
 {
-	__u32 cdw10 = (args->mo & 0xf) | (args->mos & 0xff << 16);
+	__u32 cdw10 = args->mo | (args->mos << 16);
 	__u32 cdw11 = (args->data_len >> 2) - 1;
 
 	struct nvme_passthru_cmd cmd = {
 		.opcode		= nvme_cmd_io_mgmt_recv,
 		.nsid		= args->nsid,
 		.cdw10		= cdw10,
 		.cdw11		= cdw11,
@@ -1920,15 +1929,15 @@
 	}
 
 	return nvme_submit_io_passthru(args->fd, &cmd, NULL);
 }
 
 int nvme_io_mgmt_send(struct nvme_io_mgmt_send_args *args)
 {
-	__u32 cdw10 = (args->mo & 0xf) | ((args->mos & 0xff) << 16);
+	__u32 cdw10 = args->mo | (args->mos << 16);
 
 	struct nvme_passthru_cmd cmd = {
 		.opcode		= nvme_cmd_io_mgmt_send,
 		.nsid		= args->nsid,
 		.cdw10		= cdw10,
 		.addr		= (__u64)(uintptr_t)args->data,
 		.data_len	= args->data_len,
```

### Comparing `libnvme-1.4/src/nvme/ioctl.h` & `libnvme-1.5/src/nvme/ioctl.h`

 * *Files identical despite different names*

```diff
@@ -3032,34 +3032,39 @@
  * nvme_ns_mgmt_create() - Create a non attached namespace
  * @fd:		File descriptor of nvme device
  * @ns:		Namespace identification that defines ns creation parameters
  * @nsid:		On success, set to the namespace id that was created
  * @timeout:		Override the default timeout to this value in milliseconds;
  *			set to 0 to use the system default.
  * @csi:		Command Set Identifier
+ * @data:	Host Software Specified Fields that defines ns creation parameters
  *
  * On successful creation, the namespace exists in the subsystem, but is not
  * attached to any controller. Use the nvme_ns_attach_ctrls() to assign the
  * namespace to one or more controllers.
  *
  * Return: The nvme command status if a response was received (see
  * &enum nvme_status_field) or -1 with errno set otherwise.
  */
 static inline int nvme_ns_mgmt_create(int fd, struct nvme_id_ns *ns,
-			__u32 *nsid, __u32 timeout, __u8 csi)
+			__u32 *nsid, __u32 timeout, __u8 csi,
+			struct nvme_ns_mgmt_host_sw_specified *data)
 {
 	struct nvme_ns_mgmt_args args = {
 		.result = nsid,
 		.ns = ns,
 		.args_size = sizeof(args),
 		.fd = fd,
 		.timeout = timeout,
 		.nsid = NVME_NSID_NONE,
 		.sel = NVME_NS_MGMT_SEL_CREATE,
 		.csi = csi,
+		.rsvd1 = { 0, },
+		.rsvd2 = NULL,
+		.data = data,
 	};
 
 	return nvme_ns_mgmt(&args);
 }
 
 /**
  * nvme_ns_mgmt_delete() - Delete a non attached namespace
@@ -3080,14 +3085,17 @@
 		.ns = NULL,
 		.args_size = sizeof(args),
 		.fd = fd,
 		.timeout = 0,
 		.nsid = nsid,
 		.sel = NVME_NS_MGMT_SEL_DELETE,
 		.csi = 0,
+		.rsvd1 = { 0, },
+		.rsvd2 = NULL,
+		.data = NULL,
 	};
 
 	return nvme_ns_mgmt(&args);
 }
 
 /**
  * nvme_ns_attach() - Attach or detach namespace to controller(s)
```

### Comparing `libnvme-1.4/src/nvme/json.c` & `libnvme-1.5/src/nvme/json.c`

 * *Files 1% similar despite different names*

```diff
@@ -123,24 +123,30 @@
 	attr_obj = json_object_object_get(port_obj, "dhchap_ctrl_key");
 	if (attr_obj)
 		nvme_ctrl_set_dhchap_key(c, json_object_get_string(attr_obj));
 }
 
 static void json_parse_subsys(nvme_host_t h, struct json_object *subsys_obj)
 {
-	struct json_object *nqn_obj, *port_array;
+	struct json_object *nqn_obj, *app_obj, *port_array;
 	nvme_subsystem_t s;
 	const char *nqn;
 	int p;
 
 	nqn_obj = json_object_object_get(subsys_obj, "nqn");
 	if (!nqn_obj)
 		return;
 	nqn = json_object_get_string(nqn_obj);
 	s = nvme_lookup_subsystem(h, NULL, nqn);
+	if (!s)
+		return;
+	app_obj = json_object_object_get(subsys_obj, "application");
+	if (app_obj)
+		nvme_subsystem_set_application(s, json_object_get_string(app_obj));
+
 	port_array = json_object_object_get(subsys_obj, "ports");
 	if (!port_array)
 		return;
 	for (p = 0; p < json_object_array_length(port_array); p++) {
 		struct json_object *port_obj;
 
 		port_obj = json_object_array_get_idx(port_array, p);
@@ -183,43 +189,47 @@
 	}
 }
 
 static struct json_object *parse_json(nvme_root_t r, int fd)
 {
 	char buf[JSON_FILE_BUF_SIZE];
 	struct json_object *obj = NULL;
-	struct printbuf *pb;
+	char *str = NULL;
 	json_tokener *tok = NULL;
 	int ret;
+	void *ptr = NULL;
+	int len = 0;
 
-	pb = printbuf_new();
-	if (!pb)
-		return NULL;
-
-	while ((ret = read(fd, buf, JSON_FILE_BUF_SIZE)) > 0)
-		printbuf_memappend(pb, buf, ret);
+	while ((ret = read(fd, buf, JSON_FILE_BUF_SIZE)) > 0) {
+		str = realloc(ptr, len + ret);
+		if (!str)
+			goto out;
+		memcpy(&str[len], buf, ret);
+		len += ret;
+		ptr = str;
+	}
 
-	if (ret < 0)
+	if (ret < 0 || !len)
 		goto out;
 
 	tok = json_tokener_new_ex(JSON_TOKENER_DEFAULT_DEPTH);
 	if (!tok)
 		goto out;
 
 	/* Enforce correctly formatted JSON */
 	tok->flags = JSON_TOKENER_STRICT;
 
-	obj = json_tokener_parse_ex(tok, pb->buf, printbuf_length(pb));
+	obj = json_tokener_parse_ex(tok, str, len);
 	if (!obj)
 		nvme_msg(r, LOG_DEBUG, "JSON parsing failed: %s\n",
 			 json_util_get_last_err());
 out:
 	if (tok)
 		json_tokener_free(tok);
-	printbuf_free(pb);
+	free(ptr);
 
 	return obj;
 }
 
 int json_read_config(nvme_root_t r, const char *config_file)
 {
 	struct json_object *json_root, *host_obj;
@@ -346,24 +356,28 @@
 	json_object_array_add(ctrl_array, port_obj);
 }
 
 static void json_update_subsys(struct json_object *subsys_array,
 			       nvme_subsystem_t s)
 {
 	nvme_ctrl_t c;
-	const char *subsysnqn = nvme_subsystem_get_nqn(s);
+	const char *subsysnqn = nvme_subsystem_get_nqn(s), *app;
 	struct json_object *subsys_obj = json_object_new_object();
 	struct json_object *port_array;
 
 	/* Skip discovery subsystems as the nqn is not unique */
 	if (!strcmp(subsysnqn, NVME_DISC_SUBSYS_NAME))
 		return;
 
 	json_object_object_add(subsys_obj, "nqn",
 			       json_object_new_string(subsysnqn));
+	app = nvme_subsystem_get_application(s);
+	if (app)
+		json_object_object_add(subsys_obj, "application",
+				       json_object_new_string(app));
 	port_array = json_object_new_array();
 	nvme_subsystem_for_each_ctrl(s, c) {
 		json_update_port(port_array, c);
 	}
 	if (json_object_array_length(port_array))
 		json_object_object_add(subsys_obj, "ports", port_array);
 	else
```

### Comparing `libnvme-1.4/src/nvme/linux.c` & `libnvme-1.5/src/nvme/linux.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/linux.h` & `libnvme-1.5/src/nvme/linux.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/log.c` & `libnvme-1.5/src/nvme/log.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/log.h` & `libnvme-1.5/src/nvme/log.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/mi-mctp.c` & `libnvme-1.5/src/nvme/mi-mctp.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/src/nvme/mi.c` & `libnvme-1.5/src/nvme/mi.c`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,19 @@
 	ctrl->id = ctrl_id;
 
 	list_add_tail(&ep->controllers, &ctrl->ep_entry);
 
 	return ctrl;
 }
 
+__u16 nvme_mi_ctrl_id(nvme_mi_ctrl_t ctrl)
+{
+	return ctrl->id;
+}
+
 int nvme_mi_scan_ep(nvme_mi_ep_t ep, bool force_rescan)
 {
 	struct nvme_ctrl_list list;
 	unsigned int i, n_ctrl;
 	int rc;
 
 	if (ep->controllers_scanned) {
@@ -1073,33 +1078,51 @@
 
 	return 0;
 }
 
 int nvme_mi_admin_ns_mgmt(nvme_mi_ctrl_t ctrl,
 			  struct nvme_ns_mgmt_args *args)
 {
+	const size_t size_v1 = sizeof_args(struct nvme_ns_mgmt_args, csi, __u64);
+	const size_t size_v2 = sizeof_args(struct nvme_ns_mgmt_args, data, __u64);
 	struct nvme_mi_admin_resp_hdr resp_hdr;
 	struct nvme_mi_admin_req_hdr req_hdr;
 	struct nvme_mi_resp resp;
 	struct nvme_mi_req req;
 	int rc;
+	size_t data_len;
 
-	if (args->args_size < sizeof(*args))
-		return -EINVAL;
+	if (args->args_size < size_v1 || args->args_size > size_v2) {
+		errno = EINVAL;
+		return -1;
+	}
 
 	nvme_mi_admin_init_req(&req, &req_hdr, ctrl->id,
 			       nvme_admin_ns_mgmt);
 
 	req_hdr.cdw1 = cpu_to_le32(args->nsid);
 	req_hdr.cdw10 = cpu_to_le32(args->sel & 0xf);
 	req_hdr.cdw11 = cpu_to_le32(args->csi << 24);
-	if (args->ns) {
-		req.data = args->ns;
-		req.data_len = sizeof(*args->ns);
-		req_hdr.dlen = cpu_to_le32(sizeof(*args->ns));
+
+	if (args->args_size == size_v2) {
+		if (args->data) {
+			req.data = args->data;
+			data_len = sizeof(*args->data);
+		}
+	}
+	else {
+		if (args->ns) {
+			req.data = args->ns;
+			data_len = sizeof(*args->ns);
+		}
+	}
+
+	if (req.data) {
+		req.data_len = data_len;
+		req_hdr.dlen = cpu_to_le32(data_len);
 		req_hdr.flags = 0x1;
 	}
 
 	nvme_mi_calc_req_mic(&req);
 
 	nvme_mi_admin_init_resp(&resp, &resp_hdr);
```

### Comparing `libnvme-1.4/src/nvme/mi.h` & `libnvme-1.5/src/nvme/mi.h`

 * *Files 1% similar despite different names*

```diff
@@ -651,14 +651,28 @@
 /**
  * nvme_mi_close_ctrl() - free a controller
  * @ctrl: controller to free
  */
 void nvme_mi_close_ctrl(nvme_mi_ctrl_t ctrl);
 
 /**
+ * nvme_mi_ctrl_id() - get the ID of a controller
+ * @ctrl: controller to query
+ *
+ * Retrieve the ID of the controller, as defined by hardware, and available
+ * in the Identify (Controller List) data. This is the value passed to
+ * @nvme_mi_init_ctrl, but may have been created internally via
+ * @nvme_mi_scan_ep.
+ *
+ * Return: the (locally-stored) ID of this controller.
+ */
+__u16 nvme_mi_ctrl_id(nvme_mi_ctrl_t ctrl);
+
+
+/**
  * nvme_mi_endpoint_desc - Get a string describing a MI endpoint.
  * @ep: endpoint to describe
  *
  * Generates a human-readable string describing the endpoint, with possibly
  * transport-specific data. The string is allocated during the call, and the
  * caller is responsible for free()-ing the string.
  *
@@ -2447,33 +2461,35 @@
 
 /**
  * nvme_mi_admin_ns_mgmt_create - Helper for Namespace Management Create command
  * @ctrl: Controller to send command to
  * @ns: New namespace parameters
  * @csi: Command Set Identifier for new NS
  * @nsid: Set to new namespace ID on create
+ * @data:	Host Software Specified Fields that defines ns creation parameters
  *
  * Issues a Namespace Management (Create) command to @ctrl, to create a
  * new namespace specified by @ns, using command set @csi. On success,
  * the new namespace ID will be written to @nsid.
  *
  * Return: The nvme command status if a response was received (see
  * &enum nvme_status_field) or -1 with errno set otherwise.
  */
 static inline int nvme_mi_admin_ns_mgmt_create(nvme_mi_ctrl_t ctrl,
-					       struct nvme_id_ns *ns,
-					       __u8 csi, __u32 *nsid)
+				struct nvme_id_ns *ns, __u8 csi, __u32 *nsid,
+				struct nvme_ns_mgmt_host_sw_specified *data)
 {
 	struct nvme_ns_mgmt_args args = {
 		.result = nsid,
 		.ns = ns,
 		.args_size = sizeof(args),
 		.nsid = NVME_NSID_NONE,
 		.sel = NVME_NS_MGMT_SEL_CREATE,
 		.csi = csi,
+		.data = data,
 	};
 
 	return nvme_mi_admin_ns_mgmt(ctrl, &args);
 }
 
 /**
  * nvme_mi_admin_ns_mgmt_delete - Helper for Namespace Management Delete command
```

### Comparing `libnvme-1.4/src/nvme/private.h` & `libnvme-1.5/src/nvme/private.h`

 * *Files 8% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 	char *subsysnqn;
 	char *traddr;
 	char *trsvcid;
 	char *dhchap_key;
 	char *dhchap_ctrl_key;
 	char *cntrltype;
 	char *dctype;
+	char *phy_slot;
 	bool discovery_ctrl;
 	bool unique_discovery_ctrl;
 	bool discovered;
 	bool persistent;
 	struct nvme_fabrics_config cfg;
 };
 
@@ -100,14 +101,15 @@
 	char *name;
 	char *sysfs_dir;
 	char *subsysnqn;
 	char *model;
 	char *serial;
 	char *firmware;
 	char *subsystype;
+	char *application;
 };
 
 struct nvme_host {
 	struct list_node entry;
 	struct list_head subsystems;
 	struct nvme_root *r;
 
@@ -116,24 +118,58 @@
 	char *dhchap_key;
 	char *hostsymname;
 	bool pdc_enabled;
 	bool pdc_enabled_valid; /* set if pdc_enabled doesn't have an undefined
 				 * value */
 };
 
+struct nvme_fabric_options {
+	bool cntlid;
+	bool ctrl_loss_tmo;
+	bool data_digest;
+	bool dhchap_ctrl_secret;
+	bool dhchap_secret;
+	bool disable_sqflow;
+	bool discovery;
+	bool duplicate_connect;
+	bool fast_io_fail_tmo;
+	bool hdr_digest;
+	bool host_iface;
+	bool host_traddr;
+	bool hostid;
+	bool hostnqn;
+	bool instance;
+	bool keep_alive_tmo;
+	bool keyring;
+	bool nqn;
+	bool nr_io_queues;
+	bool nr_poll_queues;
+	bool nr_write_queues;
+	bool queue_size;
+	bool reconnect_delay;
+	bool tls;
+	bool tls_key;
+	bool tos;
+	bool traddr;
+	bool transport;
+	bool trsvcid;
+};
+
 struct nvme_root {
 	char *config_file;
+	char *application;
 	struct list_head hosts;
 	struct list_head endpoints; /* MI endpoints */
 	FILE *fp;
 	int log_level;
 	bool log_pid;
 	bool log_timestamp;
 	bool modified;
 	bool mi_probe_enabled;
+	struct nvme_fabric_options *options;
 };
 
 int nvme_set_attr(const char *dir, const char *attr, const char *value);
 
 int json_read_config(nvme_root_t r, const char *config_file);
 
 int json_update_config(nvme_root_t r, const char *config_file);
```

### Comparing `libnvme-1.4/src/nvme/tree.c` & `libnvme-1.5/src/nvme/tree.c`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,58 @@
 #include "tree.h"
 #include "filters.h"
 #include "util.h"
 #include "fabrics.h"
 #include "log.h"
 #include "private.h"
 
+const char *nvme_slots_sysfs_dir = "/sys/bus/pci/slots";
+
 static struct nvme_host *default_host;
 
 static void __nvme_free_host(nvme_host_t h);
 static void __nvme_free_ctrl(nvme_ctrl_t c);
 static int nvme_subsystem_scan_namespace(nvme_root_t r,
 		struct nvme_subsystem *s, char *name,
 		nvme_scan_filter_t f, void *f_args);
 static int nvme_init_subsystem(nvme_subsystem_t s, const char *name);
 static int nvme_scan_subsystem(nvme_root_t r, const char *name,
 			       nvme_scan_filter_t f, void *f_args);
 static int nvme_ctrl_scan_namespace(nvme_root_t r, struct nvme_ctrl *c,
 				    char *name);
 static int nvme_ctrl_scan_path(nvme_root_t r, struct nvme_ctrl *c, char *name);
 
+/**
+ * Compare two C strings and handle NULL pointers gracefully.
+ * Return true if both pointers are equal (including both set to NULL).
+ * Return false if one and only one of the two pointers is NULL.
+ * Perform string comparisong only if both pointers are not NULL and
+ * return true if both strings are the same, false otherwise.
+ */
+static bool streq0(const char *s1, const char *s2)
+{
+	if (s1 == s2)
+		return true;
+	if (!s1 || !s2)
+		return false;
+	return !strcmp(s1, s2);
+}
+
+/**
+ * Same as streq0() but ignore the case of the characters.
+ */
+static bool streqcase0(const char *s1, const char *s2)
+{
+	if (s1 == s2)
+		return true;
+	if (!s1 || !s2)
+		return false;
+	return !strcasecmp(s1, s2);
+}
+
 static inline void nvme_free_dirents(struct dirent **d, int i)
 {
 	while (i-- > 0)
 		free(d[i]);
 	free(d);
 }
 
@@ -193,14 +223,27 @@
 }
 
 int nvme_dump_tree(nvme_root_t r)
 {
 	return json_dump_tree(r);
 }
 
+const char *nvme_root_get_application(nvme_root_t r)
+{
+	return r->application;
+}
+
+void nvme_root_set_application(nvme_root_t r, const char *a)
+{
+	if (r->application)
+		free(r->application);
+	if (a)
+		r->application = strdup(a);
+}
+
 nvme_host_t nvme_first_host(nvme_root_t r)
 {
 	return list_top(&r->hosts, struct nvme_host, entry);
 }
 
 nvme_host_t nvme_next_host(nvme_root_t r, nvme_host_t h)
 {
@@ -284,18 +327,21 @@
 	nvme_scan_topology(r, NULL, NULL);
 }
 
 void nvme_free_tree(nvme_root_t r)
 {
 	struct nvme_host *h, *_h;
 
+	free(r->options);
 	nvme_for_each_host_safe(r, h, _h)
 		__nvme_free_host(h);
 	if (r->config_file)
 		free(r->config_file);
+	if (r->application)
+		free(r->application);
 	free(r);
 }
 
 const char *nvme_subsystem_get_nqn(nvme_subsystem_t s)
 {
 	return s->subsysnqn;
 }
@@ -311,14 +357,27 @@
 }
 
 const char *nvme_subsystem_get_type(nvme_subsystem_t s)
 {
 	return s->subsystype;
 }
 
+const char *nvme_subsystem_get_application(nvme_subsystem_t s)
+{
+	return s->application;
+}
+
+void nvme_subsystem_set_application(nvme_subsystem_t s, const char *a)
+{
+	if (s->application)
+		free(s->application);
+	if (a)
+		s->application = strdup(a);
+}
+
 nvme_ctrl_t nvme_subsystem_first_ctrl(nvme_subsystem_t s)
 {
 	return list_top(&s->ctrls, struct nvme_ctrl, entry);
 }
 
 nvme_ctrl_t nvme_subsystem_next_ctrl(nvme_subsystem_t s, nvme_ctrl_t c)
 {
@@ -386,14 +445,16 @@
 		free(s->model);
 	if (s->serial)
 		free(s->serial);
 	if (s->firmware)
 		free(s->firmware);
 	if (s->subsystype)
 		free(s->subsystype);
+	if (s->application)
+		free(s->application);
 	free(s);
 }
 
 /*
  * Stub for SWIG
  */
 void nvme_free_subsystem(nvme_subsystem_t s)
@@ -431,14 +492,20 @@
 	nvme_for_each_subsystem(h, s) {
 		if (subsysnqn && s->subsysnqn &&
 		    strcmp(s->subsysnqn, subsysnqn))
 			continue;
 		if (name && s->name &&
 		    strcmp(s->name, name))
 			continue;
+		if (h->r->application) {
+			if (!s->application)
+				continue;
+			if (strcmp(h->r->application, s->application))
+				continue;
+		}
 		return s;
 	}
 	return nvme_alloc_subsystem(h, name, subsysnqn);
 }
 
 static void __nvme_free_host(struct nvme_host *h)
 {
@@ -537,14 +604,16 @@
 		if (!strcmp(s->subsysnqn, NVME_DISC_SUBSYS_NAME))
 			s->subsystype = strdup("discovery");
 		else
 			s->subsystype = strdup("nvm");
 	}
 	s->name = strdup(name);
 	s->sysfs_dir = (char *)path;
+	if (s->h->r->application)
+		s->application = strdup(s->h->r->application);
 
 	return 0;
 }
 
 static int nvme_scan_subsystem(struct nvme_root *r, const char *name,
 		nvme_scan_filter_t f, void *f_args)
 {
@@ -751,14 +820,19 @@
 }
 
 const char *nvme_ctrl_get_address(nvme_ctrl_t c)
 {
 	return c->address ? c->address : "";
 }
 
+const char *nvme_ctrl_get_phy_slot(nvme_ctrl_t c)
+{
+	return c->phy_slot ? c->phy_slot : "";
+}
+
 const char *nvme_ctrl_get_firmware(nvme_ctrl_t c)
 {
 	return c->firmware;
 }
 
 const char *nvme_ctrl_get_model(nvme_ctrl_t c)
 {
@@ -938,14 +1012,15 @@
 	FREE_CTRL_ATTR(c->serial);
 	FREE_CTRL_ATTR(c->sqsize);
 	FREE_CTRL_ATTR(c->dhchap_key);
 	FREE_CTRL_ATTR(c->dhchap_ctrl_key);
 	FREE_CTRL_ATTR(c->address);
 	FREE_CTRL_ATTR(c->dctype);
 	FREE_CTRL_ATTR(c->cntrltype);
+	FREE_CTRL_ATTR(c->phy_slot);
 }
 
 int nvme_disconnect_ctrl(nvme_ctrl_t c)
 {
 	nvme_root_t r = c->s && c->s->h ? c->s->h->r : NULL;
 	int ret;
 
@@ -1068,30 +1143,36 @@
 nvme_ctrl_t __nvme_lookup_ctrl(nvme_subsystem_t s, const char *transport,
 			       const char *traddr, const char *host_traddr,
 			       const char *host_iface, const char *trsvcid,
 			       nvme_ctrl_t p)
 
 {
 	struct nvme_ctrl *c;
+	bool (*addreq)(const char *, const char *);
+
+	if (!strcmp(transport, "tcp") || !strcmp(transport, "rdma"))
+		addreq = nvme_ipaddrs_eq; /* IP address compare for TCP/RDMA */
+	else
+		addreq = streqcase0; /* Case-insensitive for FC (n/a for loop) */
 
 	c = p ? nvme_subsystem_next_ctrl(s, p) : nvme_subsystem_first_ctrl(s);
 	for (; c != NULL; c = nvme_subsystem_next_ctrl(s, c)) {
-		if (strcmp(c->transport, transport))
+		if (!streq0(c->transport, transport))
 			continue;
 		if (traddr && c->traddr &&
-		    strcasecmp(c->traddr, traddr))
+		    !addreq(c->traddr, traddr))
 			continue;
 		if (host_traddr && c->cfg.host_traddr &&
-		    strcmp(c->cfg.host_traddr, host_traddr))
+		    !addreq(c->cfg.host_traddr, host_traddr))
 			continue;
 		if (host_iface && c->cfg.host_iface &&
-		    strcmp(c->cfg.host_iface, host_iface))
+		    !streq0(c->cfg.host_iface, host_iface))
 			continue;
 		if (trsvcid && c->trsvcid &&
-		    strcmp(c->trsvcid, trsvcid))
+		    !streq0(c->trsvcid, trsvcid))
 			continue;
 		return c;
 	}
 
 	return NULL;
 }
 
@@ -1179,14 +1260,61 @@
 		free(path);
 		break;
 	}
 	nvme_free_dirents(subsys, ret);
 	return subsys_name;
 }
 
+static char *nvme_ctrl_lookup_phy_slot(nvme_root_t r, const char *address)
+{
+	char *target_addr;
+	char *addr;
+	char *path;
+	int found = 0;
+	int ret;
+	DIR *slots_dir;
+	struct dirent *entry;
+
+	if (!address)
+		return NULL;
+
+	slots_dir = opendir(nvme_slots_sysfs_dir);
+	if (!slots_dir) {
+		nvme_msg(r, LOG_WARNING, "failed to open slots dir %s\n",
+		nvme_slots_sysfs_dir);
+		return NULL;
+	}
+
+	target_addr = strndup(address, 10);
+	while (!(entry = readdir(slots_dir))) {
+		if (entry->d_type == DT_DIR &&
+		    strncmp(entry->d_name, ".", 1) != 0 &&
+		    strncmp(entry->d_name, "..", 2) != 0) {
+			ret = asprintf(&path, "/sys/bus/pci/slots/%s", entry->d_name);
+			if (ret < 0) {
+				errno = ENOMEM;
+				return NULL;
+			}
+			addr = nvme_get_attr(path, "address");
+			if (strcmp(addr, target_addr) == 0) {
+				found = 1;
+				free(path);
+				free(addr);
+				break;
+			}
+			free(path);
+			free(addr);
+		}
+	}
+	free(target_addr);
+	if (found)
+		return strdup(entry->d_name);
+	return NULL;
+}
+
 static int nvme_configure_ctrl(nvme_root_t r, nvme_ctrl_t c, const char *path,
 			       const char *name)
 {
 	DIR *d;
 	char *host_key;
 
 	d = opendir(path);
@@ -1220,14 +1348,15 @@
 	c->dhchap_ctrl_key = nvme_get_ctrl_attr(c, "dhchap_ctrl_secret");
 	if (c->dhchap_ctrl_key && !strcmp(c->dhchap_ctrl_key, "none")) {
 		free(c->dhchap_ctrl_key);
 		c->dhchap_ctrl_key = NULL;
 	}
 	c->cntrltype = nvme_get_ctrl_attr(c, "cntrltype");
 	c->dctype = nvme_get_ctrl_attr(c, "dctype");
+	c->phy_slot = nvme_ctrl_lookup_phy_slot(r, c->address);
 
 	errno = 0; /* cleanup after nvme_get_ctrl_attr() */
 	return 0;
 }
 
 int nvme_init_ctrl(nvme_host_t h, nvme_ctrl_t c, int instance)
 {
@@ -1477,15 +1606,15 @@
 
 static int nvme_bytes_to_lba(nvme_ns_t n, off_t offset, size_t count,
 			    __u64 *lba, __u16 *nlb)
 {
 	int bs;
 
 	bs = nvme_ns_get_lba_size(n);
-	if (!count || offset & bs || count & bs) {
+	if (!count || offset & (bs - 1) || count & (bs - 1)) {
 		errno = EINVAL;
 		return -1;
 	}
 
 	*lba = offset >> n->lba_shift;
 	*nlb = (count >> n->lba_shift) - 1;
 	return 0;
```

### Comparing `libnvme-1.4/src/nvme/tree.h` & `libnvme-1.5/src/nvme/tree.h`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,31 @@
  * @log_level:	Logging level to use
  *
  * Return: Initialized &nvme_root_t object
  */
 nvme_root_t nvme_create_root(FILE *fp, int log_level);
 
 /**
+ * nvme_root_set_application - Specify managing application
+ * @r:	&nvme_root_t object
+ * @a:	Application string
+ *
+ * Sets the managing application string for @r.
+ */
+void nvme_root_set_application(nvme_root_t r, const char *a);
+
+/**
+ * nvme_root_get_application - Get managing application
+ * @r:	&nvme_root_t object
+ *
+ * Returns the managing application string for @r or NULL if not set.
+ */
+const char *nvme_root_get_application(nvme_root_t r);
+
+/**
  * nvme_free_tree() - Free root object
  * @r:	&nvme_root_t object
  *
  * Free an &nvme_root_t object and all attached objects
  */
 void nvme_free_tree(nvme_root_t r);
 
@@ -781,14 +798,23 @@
  *
  * Return: NVMe-over-Fabrics address string of @c or empty string
  * of no address is present.
  */
 const char *nvme_ctrl_get_address(nvme_ctrl_t c);
 
 /**
+ * nvme_ctrl_get_phy_slot() - PCI physical slot number of a controller
+ * @c:	Controller instance
+ *
+ * Return: PCI physical slot number of @c or empty string if slot
+ * number is not present.
+ */
+const char *nvme_ctrl_get_phy_slot(nvme_ctrl_t c);
+
+/**
  * nvme_ctrl_get_firmware() - Firmware string of a controller
  * @c:	Controller instance
  *
  * Return: Firmware string of @c
  */
 const char *nvme_ctrl_get_firmware(nvme_ctrl_t c);
 
@@ -1101,14 +1127,31 @@
  * Returns the subsystem type of @s.
  *
  * Return: 'nvm' or 'discovery'
  */
 const char *nvme_subsystem_get_type(nvme_subsystem_t s);
 
 /**
+ * nvme_subsystem_get_application() - Return the application string
+ * @s:	nvme_subsystem_t object
+ *
+ * Return: Managing application string or NULL if not set.
+ */
+const char *nvme_subsystem_get_application(nvme_subsystem_t s);
+
+/**
+ * nvme_subsystem_set_application() - Set the application string
+ * @s:	nvme_subsystem_t object
+ * @a:  application string
+ *
+ * Sets the managing application string for @s.
+ */
+void nvme_subsystem_set_application(nvme_subsystem_t s, const char *a);
+
+/**
  * nvme_scan_topology() - Scan NVMe topology and apply filter
  * @r:	    nvme_root_t object
  * @f:	    filter to apply
  * @f_args: user-specified argument to @f
  *
  * Scans the NVMe topology and filters out the resulting elements
  * by applying @f.
```

### Comparing `libnvme-1.4/src/nvme/types.h` & `libnvme-1.5/src/nvme/types.h`

 * *Files 1% similar despite different names*

```diff
@@ -5937,14 +5937,21 @@
  * @NVME_SC_PROHIBITED_BY_CMD_AND_FEAT: Command Prohibited by Command and Feature
  *				      Lockdown: The command was aborted due to
  *				      command execution being prohibited by
  *				      the Command and Feature Lockdown.
  * @NVME_SC_ADMIN_CMD_MEDIA_NOT_READY: Admin Command Media Not Ready: The Admin
  *				      command requires access to media and
  *				      the media is not ready.
+ * @NVME_SC_FDP_DISABLED:	      Command is not allowed when
+ *				      Flexible Data Placement is disabled.
+ * @NVME_SC_INVALID_PLACEMENT_HANDLE_LIST: The Placement Handle List is invalid
+ *				      due to invalid Reclaim Unit Handle Identifier or
+ *				      valid Reclaim Unit Handle Identifier but restricted or
+ *				      the Placement Handle List number of entries exceeded the
+ *				      maximum number allowed.
  * @NVME_SC_LBA_RANGE:		      LBA Out of Range: The command references
  *				      an LBA that exceeds the size of the namespace.
  * @NVME_SC_CAP_EXCEEDED:	      Capacity Exceeded: Execution of the
  *				      command has caused the capacity of the
  *				      namespace to be exceeded.
  * @NVME_SC_NS_NOT_READY:	      Namespace Not Ready: The namespace is not
  *				      ready to be accessed as a result of a
@@ -6281,14 +6288,16 @@
 	NVME_SC_SGL_INVALID_GRANULARITY		= 0x1e,
 	NVME_SC_CMD_IN_CMBQ_NOT_SUPP		= 0x1f,
 	NVME_SC_NS_WRITE_PROTECTED		= 0x20,
 	NVME_SC_CMD_INTERRUPTED			= 0x21,
 	NVME_SC_TRAN_TPORT_ERROR		= 0x22,
 	NVME_SC_PROHIBITED_BY_CMD_AND_FEAT	= 0x23,
 	NVME_SC_ADMIN_CMD_MEDIA_NOT_READY	= 0x24,
+	NVME_SC_FDP_DISABLED			= 0x29,
+	NVME_SC_INVALID_PLACEMENT_HANDLE_LIST	= 0x2A,
 	NVME_SC_LBA_RANGE			= 0x80,
 	NVME_SC_CAP_EXCEEDED			= 0x81,
 	NVME_SC_NS_NOT_READY			= 0x82,
 	NVME_SC_RESERVATION_CONFLICT		= 0x83,
 	NVME_SC_FORMAT_IN_PROGRESS		= 0x84,
 
 	/*
@@ -7638,8 +7647,94 @@
  * enum nvme_io_mgmt_send_mo - I/O Management Send - Management Operation
  * @NVME_IO_MGMT_SEND_RUH_UPDATE:	Reclaim Unit Handle Update
  */
 enum nvme_io_mgmt_send_mo {
 	NVME_IO_MGMT_SEND_RUH_UPDATE = 0x1,
 };
 
+#ifndef SWIG
+/**
+ * struct nvme_ns_mgmt_host_sw_specified - Namespace management Host Software
+ * Specified Fields.
+ * @nsze:     Namespace Size indicates the total size of the namespace in
+ *	      logical blocks. The number of logical blocks is based on the
+ *	      formatted LBA size.
+ * @ncap:     Namespace Capacity indicates the maximum number of logical blocks
+ *	      that may be allocated in the namespace at any point in time. The
+ *	      number of logical blocks is based on the formatted LBA size.
+ * @rsvd16:   Reserved
+ * @flbas:    Formatted LBA Size, see &enum nvme_id_ns_flbas.
+ * @rsvd27:   Reserved
+ * @dps:      End-to-end Data Protection Type Settings, see
+ *	      &enum nvme_id_ns_dps.
+ * @nmic:     Namespace Multi-path I/O and Namespace Sharing Capabilities, see
+ *	      &enum nvme_id_ns_nmic.
+ * @rsvd31:   Reserved
+ * @anagrpid: ANA Group Identifier indicates the ANA Group Identifier of the
+ *	      ANA group of which the namespace is a member.
+ * @rsvd96:   Reserved
+ * @nvmsetid: NVM Set Identifier indicates the NVM Set with which this
+ *	      namespace is associated.
+ * @endgid:   Endurance Group Identifier indicates the Endurance Group with
+ *	      which this namespace is associated.
+ * @rsvd104:  Reserved
+ * @lbstm:    Logical Block Storage Tag Mask Identifies the mask for the
+ *        Storage Tag field for the protection information
+ * @nphndls:  Number of Placement Handles specifies the number of Placement
+ *        Handles included in the Placement Handle List
+ * @rsvd394:  Reserved
+ * @rsvd499:  Reserved for I/O Command Sets that extend this specification.
+ * @zns:      rsvd499( Zoned Namespace Command Set specific field )
+ * @znsco:    Zoned Namespace Create Options
+ *	      Bits 7-1: Reserved.
+ *	      Bits 0: Allocate ZRWA Resources (AZR): If set to ‘1’, then the
+ *	      namespace is to be created with the number of ZRWA resource specified
+ *	      in the RNUMZRWA field of this data structure. If cleared to ‘0’, then
+ *	      no ZRWA resources are allocated to the namespace to be created. If
+ *	      the ZRWASUP bit is cleared to ‘0’, then this field shall be ignored
+ *	      by the controller.
+ * @rar:      Requested Active Resources specifies the number of active
+ *	      resources to be allocated to the created namespace.
+ * @ror:      Requested Open Resources specifies the number of open resources
+ *	      to be allocated to the created namespace.
+ * @rnumzrwa: Requested Number of ZRWA Resources specifies the number of ZRWA
+ *	      resources to be allocated to the created namespace.
+ *        see &struct nvme_ns_mgmt_host_sw_specified_zns.
+ * @phndl:    Placement Handle Associated RUH : This field specifies the Reclaim
+ *        Unit Handle Identifier to be associated with the Placement Handle
+ *        value. If the Flexible Data Placement capability is not supported or
+ *        not enabled in specified Endurance Group, then the controller shall
+ *        ignore this field.
+ * @rsvd768:   Reserved
+ */
+struct nvme_ns_mgmt_host_sw_specified {
+	__le64			nsze;
+	__le64			ncap;
+	__u8			rsvd16[10];
+	__u8			flbas;
+	__u8			rsvd27[2];
+	__u8			dps;
+	__u8			nmic;
+	__u8			rsvd31[61];
+	__le32			anagrpid;
+	__u8			rsvd96[4];
+	__le16			nvmsetid;
+	__le16			endgid;
+	__u8			rsvd104[280];
+	__le64			lbstm;
+	__le16			nphndls;
+	__u8			rsvd394[105];
+	union {
+		__u8		rsvd499[13];
+		struct {
+			__u8	znsco;
+			__le32	rar;
+			__le32	ror;
+			__le32	rnumzrwa;
+		} __attribute__((packed)) zns;
+	};
+	__le16			phndl[128];
+	__u8			rsvd768[3328];
+};
+#endif /* SWIG */
+
 #endif /* _LIBNVME_TYPES_H */
```

### Comparing `libnvme-1.4/src/nvme/util.c` & `libnvme-1.5/src/nvme/util.c`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
  * Copyright (c) 2020 Western Digital Corporation or its affiliates.
  *
  * Authors: Keith Busch <keith.busch@wdc.com>
  * 	    Chaitanya Kulkarni <chaitanya.kulkarni@wdc.com>
  */
 
 #include <stdio.h>
+#include <stdbool.h>
 #include <string.h>
 #include <errno.h>
 
 #include <sys/stat.h>
 #include <fcntl.h>
 #include <sys/param.h>
 #include <sys/types.h>
@@ -562,26 +563,27 @@
 	[ENVME_CONNECT_INVAL_TR] = "invalid transport type",
 	[ENVME_CONNECT_LOOKUP_SUBSYS_NAME] = "failed to lookup subsystem name",
 	[ENVME_CONNECT_LOOKUP_SUBSYS] = "failed to lookup subsystem",
 	[ENVME_CONNECT_ALREADY] = "already connected",
 	[ENVME_CONNECT_INVAL] = "invalid arguments/configuration",
 	[ENVME_CONNECT_ADDRINUSE] = "hostnqn already in use",
 	[ENVME_CONNECT_NODEV] = "invalid interface",
-	[ENVME_CONNECT_OPNOTSUPP] ="not supported",
+	[ENVME_CONNECT_OPNOTSUPP] = "not supported",
 	[ENVME_CONNECT_CONNREFUSED] = "connection refused",
+	[ENVME_CONNECT_ADDRNOTAVAIL] = "cannot assign requested address",
 };
 
 const char *nvme_errno_to_string(int status)
 {
 	const char *s = ARGSTR(libnvme_status, status);
 
 	return s;
 }
 
-#ifdef HAVE_LIBNSS
+#ifdef HAVE_NETDB
 char *hostname2traddr(struct nvme_root *r, const char *traddr)
 {
 	struct addrinfo *host_info, hints = {.ai_family = AF_UNSPEC};
 	char addrstr[NVMF_TRADDR_SIZE];
 	const char *p;
 	char *ret_traddr = NULL;
 	int ret;
@@ -617,26 +619,24 @@
 	}
 	ret_traddr = strdup(addrstr);
 
 free_addrinfo:
 	freeaddrinfo(host_info);
 	return ret_traddr;
 }
-
-#else  /* !HAVE_LIBNSS */
-
+#else /* HAVE_NETDB */
 char *hostname2traddr(struct nvme_root *r, const char *traddr)
 {
 	nvme_msg(NULL, LOG_ERR, "No support for hostname IP address resolution; " \
 		"recompile with libnss support.\n");
 
 	errno = -ENOTSUP;
 	return NULL;
 }
-#endif /* HAVE_LIBNSS */
+#endif /* HAVE_NETDB */
 
 char *startswith(const char *s, const char *prefix)
 {
 	size_t l;
 
 	l = strlen(prefix);
 	if (!strncmp(s, prefix, l))
@@ -900,7 +900,75 @@
 	 * or Pseudo-Random Numbers
 	 */
 	uuid[6] = (uuid[6] & 0x0f) | 0x40;
 	uuid[8] = (uuid[8] & 0x3f) | 0x80;
 
 	return 0;
 }
+
+#ifdef HAVE_NETDB
+bool nvme_ipaddrs_eq(const char *addr1, const char *addr2)
+{
+	bool result = false;
+	struct addrinfo *info1 = NULL, hint1 = { .ai_flags=AI_NUMERICHOST, .ai_family=AF_UNSPEC };
+	struct addrinfo *info2 = NULL, hint2 = { .ai_flags=AI_NUMERICHOST, .ai_family=AF_UNSPEC };
+
+	if (addr1 == addr2)
+		return true;
+
+	if (!addr1 || !addr2)
+		return false;
+
+	if (getaddrinfo(addr1, 0, &hint1, &info1) || !info1)
+		goto ipaddrs_eq_fail;
+
+	if (getaddrinfo(addr2, 0, &hint2, &info2) || !info2)
+		goto ipaddrs_eq_fail;
+
+	if (info1->ai_family == AF_INET && info2->ai_family == AF_INET) {
+		struct sockaddr_in *sockaddr1 = (struct sockaddr_in *)(info1->ai_addr);
+		struct sockaddr_in *sockaddr2 = (struct sockaddr_in *)(info2->ai_addr);
+		result = sockaddr1->sin_addr.s_addr == sockaddr2->sin_addr.s_addr;
+	} else if (info1->ai_family == AF_INET6 && info2->ai_family == AF_INET6) {
+		struct sockaddr_in6 *sockaddr1 = (struct sockaddr_in6 *)(info1->ai_addr);
+		struct sockaddr_in6 *sockaddr2 = (struct sockaddr_in6 *)(info2->ai_addr);
+		result = !memcmp(&sockaddr1->sin6_addr, &sockaddr2->sin6_addr, sizeof(struct in6_addr));
+	} else {
+		struct sockaddr_in *sockaddr_v4;
+		struct sockaddr_in6 *sockaddr_v6;
+		switch (info1->ai_family) {
+		case AF_INET:
+			sockaddr_v6 = (struct sockaddr_in6 *)(info2->ai_addr);
+			if (IN6_IS_ADDR_V4MAPPED(&sockaddr_v6->sin6_addr)) {
+				sockaddr_v4 = (struct sockaddr_in *)(info1->ai_addr);
+				result = sockaddr_v4->sin_addr.s_addr == sockaddr_v6->sin6_addr.s6_addr32[3];
+			}
+			break;
+
+		case AF_INET6:
+			sockaddr_v6 = (struct sockaddr_in6 *)(info1->ai_addr);
+			if (IN6_IS_ADDR_V4MAPPED(&sockaddr_v6->sin6_addr)) {
+				sockaddr_v4 = (struct sockaddr_in *)(info2->ai_addr);
+				result = sockaddr_v4->sin_addr.s_addr == sockaddr_v6->sin6_addr.s6_addr32[3];
+			}
+			break;
+
+		default: ;
+		}
+	}
+
+ipaddrs_eq_fail:
+	if (info1)
+		freeaddrinfo(info1);
+	if (info2)
+		freeaddrinfo(info2);
+	return result;
+}
+#else /* HAVE_NETDB */
+bool nvme_ipaddrs_eq(const char *addr1, const char *addr2)
+{
+	nvme_msg(NULL, LOG_ERR, "no support for hostname ip address resolution; " \
+		"recompile with libnss support.\n");
+
+	return false;
+}
+#endif /* HAVE_NETDB */
```

### Comparing `libnvme-1.4/src/nvme/util.h` & `libnvme-1.5/src/nvme/util.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
  * @ENVME_CONNECT_LOOKUP_SUBSYS_NAME:	failed to lookup subsystem name
  * @ENVME_CONNECT_LOOKUP_SUBSYS: failed to lookup subsystem
  * @ENVME_CONNECT_ALREADY:	the connect attempt failed, already connected
  * @ENVME_CONNECT_INVAL:	invalid arguments/configuration
  * @ENVME_CONNECT_ADDRINUSE:	hostnqn already in use
  * @ENVME_CONNECT_NODEV:	invalid interface
  * @ENVME_CONNECT_OPNOTSUPP:	not supported
- * @ENVME_CONNECT_CONNREFUSED:      connection refused
+ * @ENVME_CONNECT_CONNREFUSED:	connection refused
+ * @ENVME_CONNECT_ADDRNOTAVAIL:	cannot assign requested address
+ * @ENVME_CONNECT_IGNORED:	connect attempt is ignored due to configuration
  */
 enum nvme_connect_err {
 	ENVME_CONNECT_RESOLVE	= 1000,
 	ENVME_CONNECT_ADDRFAM,
 	ENVME_CONNECT_TRADDR,
 	ENVME_CONNECT_TARG,
 	ENVME_CONNECT_AARG,
@@ -53,14 +55,16 @@
 	ENVME_CONNECT_LOOKUP_SUBSYS,
 	ENVME_CONNECT_ALREADY,
 	ENVME_CONNECT_INVAL,
 	ENVME_CONNECT_ADDRINUSE,
 	ENVME_CONNECT_NODEV,
 	ENVME_CONNECT_OPNOTSUPP,
 	ENVME_CONNECT_CONNREFUSED,
+	ENVME_CONNECT_ADDRNOTAVAIL,
+	ENVME_CONNECT_IGNORED,
 };
 
 /**
  * nvme_status_to_errno() - Converts nvme return status to errno
  * @status:  Return status from an nvme passthrough command
  * @fabrics: Set to true if &status is to a fabrics target.
  *
@@ -622,8 +626,17 @@
  * Generate random number according
  * https://www.rfc-editor.org/rfc/rfc4122#section-4.4
  *
  * Return: Returns error code if generating of random number fails.
  */
 int nvme_uuid_random(unsigned char uuid[NVME_UUID_LEN]);
 
+/**
+ * nvme_ipaddrs_eq - Check if 2 IP addresses are equal.
+ * @addr1: IP address (can be IPv4 or IPv6)
+ * @addr2: IP address (can be IPv4 or IPv6)
+ *
+ * Return: true if addr1 == addr2. false otherwise.
+ */
+bool nvme_ipaddrs_eq(const char *addr1, const char *addr2);
+
 #endif /* _LIBNVME_UTIL_H */
```

### Comparing `libnvme-1.4/subprojects/openssl.wrap` & `libnvme-1.5/subprojects/openssl.wrap`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/cpp.cc` & `libnvme-1.5/test/cpp.cc`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/meson.build` & `libnvme-1.5/test/meson.build`

 * *Files 15% similar despite different names*

```diff
@@ -61,7 +61,27 @@
     'test-uuid',
     ['uuid.c'],
     dependencies: libnvme_dep,
     include_directories: [incdir, internal_incdir]
 )
 
 test('uuid', uuid)
+
+if conf.get('HAVE_NETDB')
+    tree = executable(
+        'tree',
+        ['tree.c'],
+        dependencies: libnvme_dep,
+        include_directories: [incdir, internal_incdir]
+    )
+
+    test('tree', tree)
+
+    test_util = executable(
+        'test-util',
+        ['test-util.c'],
+        include_directories: [incdir, internal_incdir]
+    )
+    test('Test util.c', test_util)
+endif
+
+subdir('nbft')
```

### Comparing `libnvme-1.4/test/mi-mctp.c` & `libnvme-1.5/test/mi-mctp.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/mi.c` & `libnvme-1.5/test/mi.c`

 * *Files 1% similar despite different names*

```diff
@@ -1287,37 +1287,37 @@
 
 static int test_admin_ns_mgmt_cb(struct nvme_mi_ep *ep,
 				 struct nvme_mi_req *req,
 				 struct nvme_mi_resp *resp,
 				 void *data)
 {
 	__u8 *rq_hdr, *rs_hdr, sel, csi;
-	struct nvme_id_ns *id;
+	struct nvme_ns_mgmt_host_sw_specified *create_data;
 	__u32 nsid;
 
 	rq_hdr = (__u8 *)req->hdr;
 	assert(rq_hdr[4] == nvme_admin_ns_mgmt);
 
 	sel = rq_hdr[44];
 	csi = rq_hdr[45];
 	nsid = rq_hdr[11] << 24 | rq_hdr[10] << 16 | rq_hdr[9] << 8 | rq_hdr[8];
 
 	rs_hdr = (__u8 *)resp->hdr;
 
 	switch (sel) {
 	case NVME_NS_MGMT_SEL_CREATE:
-		assert(req->data_len == sizeof(struct nvme_id_ns));
-		id = req->data;
+		assert(req->data_len == sizeof(struct nvme_ns_mgmt_host_sw_specified));
+		create_data = req->data;
 
 		/* No NSID on created namespaces */
 		assert(nsid == 0);
 		assert(csi == 0);
 
 		/* allow operations on nsze == 42, reject others */
-		if (le64_to_cpu(id->nsze) != 42) {
+		if (le64_to_cpu(create_data->nsze) != 42) {
 			rs_hdr[4] = 0;
 			/* response cdw0 is created NSID */
 			rs_hdr[8] = 0x04;
 			rs_hdr[9] = 0x03;
 			rs_hdr[10] = 0x02;
 			rs_hdr[11] = 0x01;
 		} else {
@@ -1338,30 +1338,30 @@
 	test_transport_resp_calc_mic(resp);
 
 	return 0;
 }
 
 static void test_admin_ns_mgmt_create(struct nvme_mi_ep *ep)
 {
-	struct nvme_id_ns nsid = { 0 };
+	struct nvme_ns_mgmt_host_sw_specified data = { 0 };
 	nvme_mi_ctrl_t ctrl;
 	__u32 ns;
 	int rc;
 
 	test_set_transport_callback(ep, test_admin_ns_mgmt_cb, NULL);
 
 	ctrl = nvme_mi_init_ctrl(ep, 5);
 	assert(ctrl);
 
-	rc = nvme_mi_admin_ns_mgmt_create(ctrl, &nsid, 0, &ns);
+	rc = nvme_mi_admin_ns_mgmt_create(ctrl, NULL, 0, &ns, &data);
 	assert(!rc);
 	assert(ns == 0x01020304);
 
-	nsid.nsze = cpu_to_le64(42);
-	rc = nvme_mi_admin_ns_mgmt_create(ctrl, &nsid, 0, &ns);
+	data.nsze = cpu_to_le64(42);
+	rc = nvme_mi_admin_ns_mgmt_create(ctrl, NULL, 0, &ns, &data);
 	assert(rc);
 }
 
 static void test_admin_ns_mgmt_delete(struct nvme_mi_ep *ep)
 {
 	nvme_mi_ctrl_t ctrl;
 	int rc;
```

### Comparing `libnvme-1.4/test/register.c` & `libnvme-1.5/test/register.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/test.c` & `libnvme-1.5/test/test.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/utils.c` & `libnvme-1.5/test/utils.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/uuid.c` & `libnvme-1.5/test/uuid.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/test/zns.c` & `libnvme-1.5/test/zns.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.4/PKG-INFO` & `libnvme-1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libnvme
-Version: 1.4
+Version: 1.5
 Summary: python bindings for libnvme
 Home-page: https://github.com/linux-nvme/libnvme
 Author: Hannes Reinecke
 Author-email: hare@suse.de
 License: LGPL-2.1-or-later
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 This is the libnvme development C library. libnvme provides type
 definitions for NVMe specification structures, enumerations, and bit
 fields, helper functions to construct, dispatch, and decode commands
 and payloads, and utilities to connect, scan, and manage nvme devices
 on a Linux system.
 
 The public specification is the authority to resolve any protocol
-discrepencies with this library. For more info on NVM Express, please
+discrepancies with this library. For more info on NVM Express, please
 see:
 
   https://nvmexpress.org
 
 Subscribe to linux-nvme@lists.infradead.org for linux-nvme related
 discussions and development for both kernel and userspace. The list is
 archived here:
@@ -52,142 +52,133 @@
 is currently licensed LGPL-2.1-or-later, see COPYING for more
 information.
 
 Keith Busch 2020-02-06
 
 ------
 
-# Building with meson
+# Dependency
 
-## What is the meson build system?
+libnvme depends on minimum Linux kernel version v4.15, which
+introduced the /sys/class/nvme-subsystem.
 
-Here's an excerpt from the meson web site: *Meson is **an open source
-build system** meant to be both extremely fast, and, even more
-importantly, as user friendly as possible. The main design point of
-Meson is that every moment a developer spends writing or debugging
-build definitions is a second wasted.*
+# Build from source
+## Prerequisite
 
-Several well-known projects such as `systemd` and `Gnome` use meson as
-their build system. A summary of projects using meson can be found
-[here](https://mesonbuild.com/Users.html). For more info on meson,
-please consult the following sites:
+A minimal build depends on a set of build tools
 
-**Wiki page**: https://en.wikipedia.org/wiki/Meson_(software)
+  - gcc
+  - ninja
+  - meson
 
-**meson documentation**: https://mesonbuild.com/
+Not all feature will be present with such configuration, e.g.
+the fabrics part of the library wont support authentication or
+TLS over the nvme-tcp transport.
 
-**meson repo**: https://github.com/mesonbuild/meson
+To enable the optional features install following libraries
 
-## Dependency
+`/etc/nvme/config.json`` support:
+  - json-c (recommend)
 
-libnvme depends on minimum Linux kernel version v4.15, which
-introduced the /sys/class/nvme-subsystem.
+Authentication and TLS over nvme-tcp:
+  - openssl
+  - keyutils
 
-## Prerequisite
+End point discovery for MI
+  - libdbus
 
-First, install meson.
+Python bindings
+  - Python 3 interpreter
+  - Python 3 development libraries
 
-**Debian / Ubuntu**:
+## Minimal on embedded builds
 
-```bash
-sudo apt-get install meson
-```
+The reference implemention of the Meson specification is in Python 3. Installing
+or porting this dependency is not really feasible for embedded project. Though
+there are two project which implement the Ninja and the Meson API in pure C99
 
-**Fedora / Red Hat**:
+  - samurai: https://github.com/michaelforney/samurai.git
+  - muon: https://git.sr.ht/~lattis/muon
 
-```bash
-sudo dnf install meson
-```
+See the CI [build](.github/workflows/build.yml) for an example how to use it.
 
 ## To compile libnvme
 
-Using meson is similar to projects that use a `configure` script before running `make`.
-
 To `configure` the project:
 
 ```
 meson setup .build
 ```
 
 Which will default to build a shared library. To configure for static libraries call
 
 ```
-meson setup .build --default-library=static
+meson setup --default-library=static .build
 ```
 
 One nice feature of meson is that it doesn't mix build artifacts
 (e.g. `*.o`, `*.so`, etc.) with source code. In the above example,
 "`.build`" is the name of the directory where the build configuration
 as well as all the build artifacts will be saved. This directory can
 be named anything as long as it's not an existing source directory. To
 completely "clean" all the build artifacts, one need only delete the
 `.build` directory.
 
 To compile:
 
 ```
-cd .build
-ninja
-```
-
-Or:
-
-```
-ninja -C .build
+meson -C .build
 ```
 
 ## To install libnvme
 
 To install `libnvme`:
 
 ```
-cd .build
-meson install
+meson install -C .build
 ```
 
 ## To run unit tests
 
 To run unit tests:
 
 ```
-cd .build
-meson test
-```
-
-## To clean after a build
-
-To perform the equivalent of a `make clean` without deleting the build configuration.
-
-```
-cd .build
-ninja -t clean
-```
-
-Or:
-
-```
-ninja -C .build -t clean
+meson test -C .build
 ```
 
 ## To purge everything
 
 To completely clean all build artifacts, including the build configuration.
 
 ```
 rm -rf .build
 ```
 
 ## Supported build options
 
 A few build options can be specified on the command line when invoking meson.
 
-| Option | Values [default]          | Description                                                  |
-| ------ | ------------------------- | ------------------------------------------------------------ |
-| man    | true, [false]             | Instruct meson to configure the project to build the `libnvme` documentation. <br />Example: `meson .build -Dman=true` |
+| Option      | Values [default]          | Description                                                  |
+| ----------- | ------------------------- | ------------------------------------------------------------ |
+| version-tag | none                      | Overwrite the git version string in the binary               |
+| htmldir     | none                      | Installation directory for the HTML documentation            |
+| rstdir      | none                      | Installation directory for the RST documentation             |
+| docs        | [false], html, man, rst, all | Install documentation                                     |
+| docs-build  | [false], true             | Enable build documentation                                   |
 | python | [auto], enabled, disabled | Whether to build the Python bindings. When set to `auto`, the default, meson will check for the presence of the  tools and libraries (e.g. `swig`) required to build the Python bindings. If found, meson will configure the project to build the Python bindings. If a tool or library is missing, then the Python bindings won't be built. Setting this to `enabled`, forces the Python bindings to be built. When set to `disabled`, meson will configure the project to not build the Python bindings.<br />Example: `meson setup .build -Dpython=disabled` |
+| openssl     | [auto], enabled, disabled | Enables OpenSSL dependend features (e.g. authentication), adds build dependency on OpenSSL |
+| libdbus     | auto, enabled, [disabled] | Enables D-Bus dependend features (libnvme-mi: End point discovery), adds build dependency on libdbus |
+| json-c      | [auto], enabled, disabled | (recommended) Enables JSON-C dependend features (e.g. config.json parsing), adds build depdency on json-c |
+| keyutils    | [auto], enabled, disabled | Enables keyutils dependend features (e.g. TLS over TCP), adds build dependency on keyutils |
+
+See the full configuration options with
+
+```bash
+meson configure .build
+```
 
 ### Changing the build options from the command-line (i.e. w/o modifying any files)
 
 To configure a build for debugging purposes (i.e. optimization turned
 off and debug symbols enabled):
 
 ```bash
@@ -199,16 +190,9 @@
 ```bash
 meson setup .build -Db_sanitize=address
 ```
 
 This option adds `-fsanitize=address` to the gcc options. Note that when using the sanitize feature, the library `libasan.so` must be available and must be the very first library loaded when running an executable. Ensuring that `libasan.so` gets loaded first can be achieved with the `LD_PRELOAD` environment variable as follows: 
 
 ```
-meson setup .build -Db_sanitize=address && LD_PRELOAD=/lib64/libasan.so.6 ninja -C .build test 
-```
-
-To list configuration options that are available and possible values:
-
-```bash
-meson configure .build
+meson setup .build -Db_sanitize=address && LD_PRELOAD=/lib64/libasan.so.6 ninja -C .build test
 ```
-
```

