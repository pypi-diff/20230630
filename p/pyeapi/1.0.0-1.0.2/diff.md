# Comparing `tmp/pyeapi-1.0.0.tar.gz` & `tmp/pyeapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyeapi-1.0.0.tar", last modified: Tue Jun  6 13:22:00 2023, max compression
+gzip compressed data, was "dist/pyeapi-1.0.2.tar", last modified: Thu Jun 29 22:58:19 2023, max compression
```

## Comparing `pyeapi-1.0.0.tar` & `pyeapi-1.0.2.tar`

### file list

```diff
@@ -1,157 +1,183 @@
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:22:00.000000 pyeapi-1.0.0/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1588 2023-06-06 13:22:00.000000 pyeapi-1.0.0/PKG-INFO
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1488 2023-06-06 11:56:48.000000 pyeapi-1.0.0/LICENSE
--rw-r--r--   0 dlyssenko   (501) staff       (20)        8 2023-06-06 11:56:48.000000 pyeapi-1.0.0/requirements.txt
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:57.000000 pyeapi-1.0.0/test/
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:22:00.000000 pyeapi-1.0.0/test/unit/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7678 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_stp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8897 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_switchports.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6111 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_varp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3109 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_utils.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6410 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_vlans.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     5941 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_ospf.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    11572 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_staticroute.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     4292 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_system.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    31011 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_vrrp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6632 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_mlag.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    11353 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_acl.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     4425 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_ntp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    23399 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_interfaces.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7338 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_vrfs.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    18863 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_bgp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7017 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_routemaps.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    19641 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_client.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     9951 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_eapilib.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     5955 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_users.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6142 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/unit/test_api_ipinterfaces.py
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:22:00.000000 pyeapi-1.0.0/test/system/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6185 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_stp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6199 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_switchports.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    12500 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_varp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8594 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_vlans.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     9101 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_ospf.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    10836 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_staticroute.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     9596 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_system.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    22511 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_vrrp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    11542 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_mlag.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    10326 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_acl.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7936 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_ntp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    29085 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_interfaces.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    14942 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_vrfs.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    12357 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_routemaps.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    15031 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_client.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     9678 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_users.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6103 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/system/test_api_ipinterfaces.py
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:22:00.000000 pyeapi-1.0.0/test/lib/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     4253 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/lib/testlib.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     2896 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/lib/systestlib.py
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:59.000000 pyeapi-1.0.0/test/fixtures/
--rw-r--r--   0 dlyssenko   (501) staff       (20)       91 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/env_path.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7185 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/show_interfaces.text
--rw-r--r--   0 dlyssenko   (501) staff       (20)       82 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/eapi.conf.yaml
--rw-r--r--   0 dlyssenko   (501) staff       (20)      685 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/vxlan.json
--rw-r--r--   0 dlyssenko   (501) staff       (20)      409 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.varp
--rw-r--r--   0 dlyssenko   (501) staff       (20)      402 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/show_version.text
--rw-r--r--   0 dlyssenko   (501) staff       (20)       89 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/dut.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)    19736 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/show_interfaces.json
--rw-r--r--   0 dlyssenko   (501) staff       (20)      894 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.ospf
--rw-r--r--   0 dlyssenko   (501) staff       (20)    56445 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.text
--rw-r--r--   0 dlyssenko   (501) staff       (20)        0 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/empty.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)      458 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/show_version.json
--rw-r--r--   0 dlyssenko   (501) staff       (20)     2475 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/ipinterfaces.json
--rw-r--r--   0 dlyssenko   (501) staff       (20)      233 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/eapi.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)       19 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/nohost.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)      508 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.varp_null
--rw-r--r--   0 dlyssenko   (501) staff       (20)      191 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/show_portchannel.json
--rw-r--r--   0 dlyssenko   (501) staff       (20)      476 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.bgp
--rw-r--r--   0 dlyssenko   (501) staff       (20)      922 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.routemaps
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1544 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.vxlan
--rw-r--r--   0 dlyssenko   (501) staff       (20)     5542 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.vrf
--rw-r--r--   0 dlyssenko   (501) staff       (20)    13343 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.vrrp
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8955 2023-06-06 11:56:48.000000 pyeapi-1.0.0/test/fixtures/running_config.portchannel
--rw-r--r--   0 dlyssenko   (501) staff       (20)      164 2023-06-06 11:56:48.000000 pyeapi-1.0.0/CHANGELOG.md
--rw-r--r--   0 dlyssenko   (501) staff       (20)      237 2023-06-06 11:56:48.000000 pyeapi-1.0.0/dev-requirements.txt
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1806 2023-06-06 11:56:48.000000 pyeapi-1.0.0/Makefile
--rw-r--r--   0 dlyssenko   (501) staff       (20)      724 2023-06-06 11:56:48.000000 pyeapi-1.0.0/MANIFEST.in
--rw-r--r--   0 dlyssenko   (501) staff       (20)      656 2023-06-06 11:56:48.000000 pyeapi-1.0.0/.coveragerc
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:58.000000 pyeapi-1.0.0/docs/
--rw-r--r--   0 dlyssenko   (501) staff       (20)       97 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.2.1.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3996 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/install.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1305 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/subinterfaces.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1120 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/index.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      474 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.2.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      106 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.2.2.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7679 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/configfile.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1680 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/configsessions.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)       88 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.2.3.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     5719 2023-06-06 11:57:13.000000 pyeapi-1.0.0/docs/release-notes-1.0.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     4060 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.4.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1058 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/contribute.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)       84 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.2.4.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1867 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.6.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      707 2023-06-06 11:57:13.000000 pyeapi-1.0.0/docs/release-notes.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1176 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/support.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      392 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.6.1.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      234 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.1.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7014 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/Makefile
--rw-r--r--   0 dlyssenko   (501) staff       (20)      105 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.3.2.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      155 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.3.3.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      459 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.1.1.rst
--rwxr-xr-x   0 dlyssenko   (501) staff       (20)    10783 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/conf.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)      228 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.3.1.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      304 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.3.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      121 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/examples.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      315 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/requirements.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1267 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.7.0.rst
--rwxr-xr-x   0 dlyssenko   (501) staff       (20)     2845 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/generate_modules.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     2704 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.5.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      114 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/modules.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      870 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/description.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3964 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/quickstart.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1504 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/license.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      360 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.8.3.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1275 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.8.2.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3700 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.8.0.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1245 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.8.1.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)      221 2023-06-06 11:56:48.000000 pyeapi-1.0.0/docs/release-notes-0.8.4.rst
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3596 2023-06-06 11:56:48.000000 pyeapi-1.0.0/README.md
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:59.000000 pyeapi-1.0.0/pyeapi.egg-info/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1588 2023-06-06 13:21:57.000000 pyeapi-1.0.0/pyeapi.egg-info/PKG-INFO
--rw-r--r--   0 dlyssenko   (501) staff       (20)     3679 2023-06-06 13:21:57.000000 pyeapi-1.0.0/pyeapi.egg-info/SOURCES.txt
--rw-r--r--   0 dlyssenko   (501) staff       (20)       72 2023-06-06 13:21:57.000000 pyeapi-1.0.0/pyeapi.egg-info/requires.txt
--rw-r--r--   0 dlyssenko   (501) staff       (20)        7 2023-06-06 13:21:57.000000 pyeapi-1.0.0/pyeapi.egg-info/top_level.txt
--rw-r--r--   0 dlyssenko   (501) staff       (20)        1 2023-06-06 13:21:57.000000 pyeapi-1.0.0/pyeapi.egg-info/dependency_links.txt
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:59.000000 pyeapi-1.0.0/pyeapi/
--rw-r--r--   0 dlyssenko   (501) staff       (20)    40893 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/client.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1712 2023-06-06 11:57:13.000000 pyeapi-1.0.0/pyeapi/__init__.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8866 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/utils.py
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:59.000000 pyeapi-1.0.0/pyeapi/api/
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8013 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/abstract.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    40060 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/interfaces.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     6781 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/system.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    11972 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/users.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    13418 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/bgp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    12370 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/vrfs.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     1619 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/__init__.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     7261 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/ntp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    10972 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/mlag.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    11123 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/acl.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    10157 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/ipinterfaces.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    14591 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/routemaps.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    61008 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/vrrp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    13291 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/ospf.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    14275 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/staticroute.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    16699 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/switchports.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    12500 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/vlans.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    13541 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/stp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     8273 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/api/varp.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)    28480 2023-06-06 11:56:48.000000 pyeapi-1.0.0/pyeapi/eapilib.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)     2825 2023-06-06 11:56:48.000000 pyeapi-1.0.0/setup.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)        6 2023-06-06 11:57:13.000000 pyeapi-1.0.0/VERSION
-drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-06 13:21:59.000000 pyeapi-1.0.0/examples/
--rw-r--r--   0 dlyssenko   (501) staff       (20)      778 2023-06-06 11:56:48.000000 pyeapi-1.0.0/examples/vlans_api.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)      259 2023-06-06 11:56:48.000000 pyeapi-1.0.0/examples/sysmac.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)      149 2023-06-06 11:56:48.000000 pyeapi-1.0.0/examples/nodes.conf
--rw-r--r--   0 dlyssenko   (501) staff       (20)      479 2023-06-06 11:56:48.000000 pyeapi-1.0.0/examples/get_config.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)      260 2023-06-06 11:56:48.000000 pyeapi-1.0.0/examples/simple.py
--rw-r--r--   0 dlyssenko   (501) staff       (20)       38 2023-06-06 13:22:00.000000 pyeapi-1.0.0/setup.cfg
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      656 2023-06-29 22:55:31.000000 pyeapi-1.0.2/.coveragerc
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      164 2023-06-29 22:55:31.000000 pyeapi-1.0.2/CHANGELOG.md
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1488 2023-06-29 22:55:31.000000 pyeapi-1.0.2/LICENSE
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      724 2023-06-29 22:55:31.000000 pyeapi-1.0.2/MANIFEST.in
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1806 2023-06-29 22:55:31.000000 pyeapi-1.0.2/Makefile
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1588 2023-06-29 22:58:19.000000 pyeapi-1.0.2/PKG-INFO
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     3596 2023-06-29 22:55:31.000000 pyeapi-1.0.2/README.md
+-rw-r--r--   0 dlyssenko   (501) staff       (20)        6 2023-06-29 22:56:43.000000 pyeapi-1.0.2/VERSION
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      237 2023-06-29 22:55:31.000000 pyeapi-1.0.2/dev-requirements.txt
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/docs/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7014 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/Makefile
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/docs/api_modules/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      281 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/_list_of_modules.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      200 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/abstract.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      185 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/acl.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      185 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/bgp.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      206 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/interfaces.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      212 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/ipinterfaces.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      188 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/mlag.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      185 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/ntp.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      188 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/ospf.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      203 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/routemaps.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      209 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/staticroute.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      185 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/stp.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      209 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/switchports.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      194 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/system.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      191 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/users.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      188 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/varp.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      191 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/vlans.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      188 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/vrfs.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      188 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/api_modules/vrrp.rst
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/docs/client_modules/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      136 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/client_modules/_list_of_modules.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      190 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/client_modules/client.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      193 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/client_modules/eapilib.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      187 2023-06-29 22:57:52.000000 pyeapi-1.0.2/docs/client_modules/utils.rst
+-rwxr-xr-x   0 dlyssenko   (501) staff       (20)    10783 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/conf.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7679 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/configfile.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1680 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/configsessions.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1058 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/contribute.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      870 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/description.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      121 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/examples.rst
+-rwxr-xr-x   0 dlyssenko   (501) staff       (20)     2845 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/generate_modules.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1120 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/index.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     3996 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/install.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1504 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/license.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      114 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/modules.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     3964 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/quickstart.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      234 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.1.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      459 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.1.1.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      474 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.2.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       97 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.2.1.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      106 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.2.2.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       88 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.2.3.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       84 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.2.4.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      304 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.3.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      228 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.3.1.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      105 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.3.2.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      155 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.3.3.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     4060 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.4.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     2704 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.5.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1867 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.6.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      392 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.6.1.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1267 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.7.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     3700 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.8.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1245 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.8.1.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1275 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.8.2.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      360 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.8.3.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      221 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-0.8.4.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     5747 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/release-notes-1.0.0.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      577 2023-06-29 22:56:43.000000 pyeapi-1.0.2/docs/release-notes-1.0.2.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      735 2023-06-29 22:56:43.000000 pyeapi-1.0.2/docs/release-notes.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      315 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/requirements.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1305 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/subinterfaces.rst
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1176 2023-06-29 22:55:31.000000 pyeapi-1.0.2/docs/support.rst
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/examples/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      479 2023-06-29 22:55:31.000000 pyeapi-1.0.2/examples/get_config.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      149 2023-06-29 22:55:31.000000 pyeapi-1.0.2/examples/nodes.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      260 2023-06-29 22:55:31.000000 pyeapi-1.0.2/examples/simple.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      259 2023-06-29 22:55:31.000000 pyeapi-1.0.2/examples/sysmac.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      778 2023-06-29 22:55:31.000000 pyeapi-1.0.2/examples/vlans_api.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1712 2023-06-29 22:56:43.000000 pyeapi-1.0.2/pyeapi/__init__.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi/api/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1619 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/__init__.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     8013 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/abstract.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    11123 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/acl.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    13418 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/bgp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    40403 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/interfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    10157 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/ipinterfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    10972 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/mlag.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7261 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/ntp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    13291 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/ospf.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    14591 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/routemaps.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    14275 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/staticroute.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    13541 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/stp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    16699 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/switchports.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6781 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/system.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    11972 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/users.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     8273 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/varp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    12500 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/vlans.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    12370 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/vrfs.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    61008 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/api/vrrp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    41111 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/client.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    28548 2023-06-29 22:55:31.000000 pyeapi-1.0.2/pyeapi/eapilib.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     9761 2023-06-29 22:56:43.000000 pyeapi-1.0.2/pyeapi/utils.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1588 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/PKG-INFO
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     4385 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 dlyssenko   (501) staff       (20)        1 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       72 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/requires.txt
+-rw-r--r--   0 dlyssenko   (501) staff       (20)        7 2023-06-29 22:58:19.000000 pyeapi-1.0.2/pyeapi.egg-info/top_level.txt
+-rw-r--r--   0 dlyssenko   (501) staff       (20)        8 2023-06-29 22:55:31.000000 pyeapi-1.0.2/requirements.txt
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       38 2023-06-29 22:58:19.000000 pyeapi-1.0.2/setup.cfg
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     2825 2023-06-29 22:55:31.000000 pyeapi-1.0.2/setup.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/test/
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/test/fixtures/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       89 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/dut.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      233 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/eapi.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       82 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/eapi.conf.yaml
+-rw-r--r--   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/empty.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       91 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/env_path.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     2475 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/ipinterfaces.json
+-rw-r--r--   0 dlyssenko   (501) staff       (20)       19 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/nohost.conf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      476 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.bgp
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      894 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.ospf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     8955 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.portchannel
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      922 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.routemaps
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    56445 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.text
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      409 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.varp
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      508 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.varp_null
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     5542 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.vrf
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    13343 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.vrrp
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     1544 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/running_config.vxlan
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    19736 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/show_interfaces.json
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7185 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/show_interfaces.text
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      191 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/show_portchannel.json
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      458 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/show_version.json
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      402 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/show_version.text
+-rw-r--r--   0 dlyssenko   (501) staff       (20)      685 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/fixtures/vxlan.json
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/test/lib/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     2896 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/lib/systestlib.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     4814 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/lib/testlib.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/test/system/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    10326 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_acl.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    30034 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_interfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6103 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_ipinterfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    11542 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_mlag.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7936 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_ntp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     9101 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_ospf.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    12357 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_routemaps.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    10268 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_staticroute.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6185 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_stp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6199 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_switchports.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     9596 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_system.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     9678 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_users.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    12500 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_varp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     8594 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_vlans.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    14867 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_vrfs.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    22767 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_api_vrrp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    14899 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/system/test_client.py
+drwxr-xr-x   0 dlyssenko   (501) staff       (20)        0 2023-06-29 22:58:19.000000 pyeapi-1.0.2/test/unit/
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    11353 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_acl.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    18863 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_bgp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    23399 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_interfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6142 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_ipinterfaces.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6632 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_mlag.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     4425 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_ntp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     5941 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_ospf.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7017 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_routemaps.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    11572 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_staticroute.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7678 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_stp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     8897 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_switchports.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     4292 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_system.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     5955 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_users.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6111 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_varp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     6410 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_vlans.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     7338 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_vrfs.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    31011 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_api_vrrp.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)    19650 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_client.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     9960 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_eapilib.py
+-rw-r--r--   0 dlyssenko   (501) staff       (20)     3030 2023-06-29 22:55:31.000000 pyeapi-1.0.2/test/unit/test_utils.py
```

### Comparing `pyeapi-1.0.0/PKG-INFO` & `pyeapi-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeapi
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python Client for eAPI
 Home-page: https://github.com/arista-eosplus/pyeapi
 Author: Arista EOS+ CS
 Author-email: eosplus-dev@arista.com
 License: BSD-3
 Description: The Python Client for eAPI
         ==========================
@@ -29,9 +29,9 @@
 Keywords: networking arista eos eapi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `pyeapi-1.0.0/LICENSE` & `pyeapi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_stp.py` & `pyeapi-1.0.2/test/unit/test_api_stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_switchports.py` & `pyeapi-1.0.2/test/unit/test_api_switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_varp.py` & `pyeapi-1.0.2/test/unit/test_api_varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_utils.py` & `pyeapi-1.0.2/test/unit/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import sys
 import unittest
 
-from mock import patch, Mock
+from unittest.mock import patch, Mock
 import pyeapi.utils
 
-if sys.version_info < (3, 3):
-    from collections import Iterable
-else:
-    from collections.abc import Iterable
+from collections.abc import Iterable
 
 class TestUtils(unittest.TestCase):
 
     @patch('pyeapi.utils.import_module')
     def test_load_module(self, mock_import_module):
         loaded_module = Mock(object='loaded_module')
         mock_import_module.return_value = loaded_module
```

### Comparing `pyeapi-1.0.0/test/unit/test_api_vlans.py` & `pyeapi-1.0.2/test/unit/test_api_vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_ospf.py` & `pyeapi-1.0.2/test/unit/test_api_ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_staticroute.py` & `pyeapi-1.0.2/test/unit/test_api_staticroute.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_system.py` & `pyeapi-1.0.2/test/unit/test_api_system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_vrrp.py` & `pyeapi-1.0.2/test/unit/test_api_vrrp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_mlag.py` & `pyeapi-1.0.2/test/unit/test_api_mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_acl.py` & `pyeapi-1.0.2/test/unit/test_api_acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_ntp.py` & `pyeapi-1.0.2/test/unit/test_api_ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_interfaces.py` & `pyeapi-1.0.2/test/unit/test_api_interfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_vrfs.py` & `pyeapi-1.0.2/test/unit/test_api_vrfs.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_bgp.py` & `pyeapi-1.0.2/test/unit/test_api_bgp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_routemaps.py` & `pyeapi-1.0.2/test/unit/test_api_routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_client.py` & `pyeapi-1.0.2/test/unit/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import sys
 import os
 import unittest
 import imp
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
 
-from mock import Mock, patch, call
+from unittest.mock import Mock, patch, call
 
 from testlib import get_fixture, random_string, random_int
 
 import pyeapi.client
 
 DEFAULT_CONFIG = {'connection:localhost': dict(transport='socket')}
```

### Comparing `pyeapi-1.0.0/test/unit/test_eapilib.py` & `pyeapi-1.0.2/test/unit/test_eapilib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import json
 
-from mock import Mock, patch
+from unittest.mock import Mock, patch
 
 import pyeapi.eapilib
 
 
 class TestEapiConnection(unittest.TestCase):
 
     def test_execute_valid_response(self):
```

### Comparing `pyeapi-1.0.0/test/unit/test_api_users.py` & `pyeapi-1.0.2/test/unit/test_api_users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/unit/test_api_ipinterfaces.py` & `pyeapi-1.0.2/test/unit/test_api_ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_stp.py` & `pyeapi-1.0.2/test/system/test_api_stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_switchports.py` & `pyeapi-1.0.2/test/system/test_api_switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_varp.py` & `pyeapi-1.0.2/test/system/test_api_varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_vlans.py` & `pyeapi-1.0.2/test/system/test_api_vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_ospf.py` & `pyeapi-1.0.2/test/system/test_api_ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_staticroute.py` & `pyeapi-1.0.2/test/system/test_api_staticroute.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,16 +79,15 @@
 class TestApiStaticroute(DutSystemTest):
 
     def test_create(self):
         # Validate the create function returns without an error
         # when creating routes with varying parameters included.
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing'])
+            dut.config(['no ip routing', 'ip routing'])
 
             for t_distance in DISTANCES:
                 for t_tag in TAGS:
                     for t_route_name in ROUTE_NAMES:
                         ip_dest = _ip_addr()
                         (next_hop, next_hop_ip) = _next_hop()
                         distance = t_distance
@@ -108,16 +107,15 @@
                         self.assertTrue(result)
 
     def test_get(self):
         # Validate the get function returns the exact value that
         # is passed in when the route exists on the switch.
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing'])
+            dut.config(['no ip routing', 'ip routing'])
 
             ip_dest = '1.2.3.0/24'
             next_hop = 'Ethernet1'
             next_hop_ip = '1.1.1.1'
             distance = 1
             tag = 1
             route_name = 'test1'
@@ -148,67 +146,51 @@
     def test_getall(self):
         # Validate the get_all function returns a list of entries
         # containing the matched parameters, and that parameters
         # are matched in full (i.e. name 'test1' does not match
         # name 'test10').
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing'])
-
+            dut.config(['no ip routing', 'ip routing'])
             # Declare a set of 3 routes with same ip dest and next hop.
             # Set different distance, tag and name for each route,
             # including values 1 and 10 in each, so the test will verify
             # that matching 1 does not also match 10.
             route1 = \
                 'ip route 1.2.3.0/24 Ethernet1 1.1.1.1 10 tag 1 name test1'
             route2 = \
                 'ip route 1.2.3.0/24 Ethernet1 1.1.1.1 1 tag 1 name test10'
             route3 = \
                 'ip route 1.2.3.0/24 Ethernet1 1.1.1.1 2 tag 10 name test1'
-
             dut.config([route1, route2, route3])
-
             routes = {
                 '1.2.3.0/24': {
                     'Ethernet1': {
                         '1.1.1.1': {
-                            10: {
-                                'tag': 1,
-                                'route_name': 'test1'
-                            },
-                            1: {
-                                'tag': 1,
-                                'route_name': 'test10'
-                            },
-                            2: {
-                                'tag': 10,
-                                'route_name': 'test1'
-                            }
+                            10: { 'tag': 1, 'route_name': 'test1' },
+                            1: { 'tag': 1, 'route_name': 'test10' },
+                            2: { 'tag': 10, 'route_name': 'test1' }
                         }
                     }
                 }
             }
-
             # Get the list of ip routes from the switch
             result = dut.api('staticroute').getall()
-
             # Assert that the result dict is equivalent to the routes dict
-            self.assertEqual(result, routes)
+            self.assertEqual(result['1.2.3.0/24'], routes['1.2.3.0/24'])
 
     def test_delete(self):
         # Validate the delete function returns without an error
         # when deleting routes with varying parameters included.
         # Note: the routes do not have to exist for the
         # delete command to succeed, but only that the command
         # does not error.
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing'])
+            dut.config(['no ip routing', 'ip routing'])
 
             for t_distance in DISTANCES:
                 for t_tag in TAGS:
                     for t_route_name in ROUTE_NAMES:
                         ip_dest = _ip_addr()
                         (next_hop, next_hop_ip) = _next_hop()
                         distance = t_distance
@@ -231,16 +213,15 @@
         # Validate the default function returns without an error
         # when deleting routes with varying parameters included.
         # Note: currently EOS functionality of 'default ip route ...'
         # is equivalent to 'no ip route ...', which is the delete
         # function.
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing'])
+            dut.config(['no ip routing', 'ip routing'])
 
             for t_distance in DISTANCES:
                 for t_tag in TAGS:
                     for t_route_name in ROUTE_NAMES:
                         ip_dest = _ip_addr()
                         (next_hop, next_hop_ip) = _next_hop()
                         distance = t_distance
@@ -260,30 +241,28 @@
                         self.assertTrue(result)
 
     def test_set_tag(self):
         # Validate the set_tag function returns without an error
         # when modifying the tag on an existing route
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing',
+            dut.config(['no ip routing', 'ip routing',
                         'ip route 1.2.3.0/24 Ethernet1 1.1.1.1 10 tag 99'])
 
             result = dut.api('staticroute').set_tag(
                 '1.2.3.0/24', 'Ethernet1', next_hop_ip='1.1.1.1',
                 distance=10, tag=3)
             self.assertTrue(result)
 
     def test_set_route_name(self):
         # Validate the set_route_name function returns without an error
         # when modifying the tag on an existing route
 
         for dut in self.duts:
-            dut.config(['no ip routing delete-static-routes',
-                        'ip routing',
+            dut.config(['no ip routing', 'ip routing',
                         'ip route 1.2.3.0/24 Ethernet1 1.1.1.1 1 name test99'])
 
             result = dut.api('staticroute').set_route_name(
                 '1.2.3.0/24', 'Ethernet1', next_hop_ip='1.1.1.1',
                 distance=1, route_name='test3')
             self.assertTrue(result)
```

### Comparing `pyeapi-1.0.0/test/system/test_api_system.py` & `pyeapi-1.0.2/test/system/test_api_system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_vrrp.py` & `pyeapi-1.0.2/test/system/test_api_vrrp.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,27 +113,24 @@
     def test_create(self):
         vrid = 99
         import copy
         vrrp_conf = copy.deepcopy(VR_CONFIG)
         # vrrp_conf = dict(VR_CONFIG)
         for dut in self.duts:
             interface = self._vlan_setup(dut)
-            dut.config(['interface %s' % interface,
-                        'no vrrp %d' % vrid,
-                        'exit'])
-
+            dut.config([f'interface {interface}', f'no vrrp {vrid}', 'exit'])
             response = dut.api('vrrp').create(interface, vrid, **vrrp_conf)
             self.assertIs(response, True)
-
             # Fix the configuration dict for proper output
             vrrp_conf = dut.api('vrrp').vrconf_format(vrrp_conf)
-
             response = dut.api('vrrp').get(interface)[vrid]
-
             self.maxDiff = None
+            # now delete dict items which vary between versions
+            for key in ( 'preempt_delay_min', 'preempt_delay_reload' ):
+                del vrrp_conf[ key ], response[ key ]
             self.assertEqual(response, vrrp_conf)
 
     def test_delete(self):
         vrid = 101
         for dut in self.duts:
             interface = self._vlan_setup(dut)
             if dut.version_number >= '4.23':
@@ -165,29 +162,24 @@
                             'vrrp %d shutdown' % vrid,
                             'exit'])
 
             response = dut.api('vrrp').delete(interface, vrid)
             self.assertIs(response, True)
 
     def test_update_with_create(self):
-        pass
         vrid = 103
         import copy
         vrrp_conf = copy.deepcopy(VR_CONFIG)
         # vrrp_conf = dict(VR_CONFIG)
         for dut in self.duts:
             interface = self._vlan_setup(dut)
-            dut.config(['interface %s' % interface,
-                        'no vrrp %d' % vrid,
-                        'exit'])
-
+            dut.config([f'interface {interface}', f'no vrrp {vrid}', 'exit'])
             # Create the inital vrrp on the interface
             response = dut.api('vrrp').create(interface, vrid, **vrrp_conf)
             self.assertIs(response, True)
-
             # Update some of the information on the vrrp
             vrrp_update = {
                 'primary_ip': '10.10.10.12',
                 'priority': 200,
                 'description': 'updated vrrp 10 on an interface',
                 'secondary_ip': ['10.10.10.13', '10.10.10.23'],
                 'ip_version': 2,
@@ -200,21 +192,21 @@
                 'delay_reload': 'default',
                 'track': [
                     {'name': 'Ethernet2', 'action': 'shutdown'},
                     {'name': 'Ethernet2', 'action': 'decrement', 'amount': 1},
                 ],
                 'bfd_ip': None,
             }
-
             response = dut.api('vrrp').create(interface, vrid, **vrrp_update)
             self.assertIs(response, True)
             vrrp_update = dut.api('vrrp').vrconf_format(vrrp_update)
-
             response = dut.api('vrrp').get(interface)[vrid]
-
+            # now delete dict items which vary between versions
+            for key in ( 'preempt_delay_min', 'preempt_delay_reload' ):
+                del vrrp_update[ key ], response[ key ]
             self.maxDiff = None
             self.assertEqual(response, vrrp_update)
 
     def test_set_enable(self):
         vrid = 104
         enable_cases = [
             {'value': True},
```

### Comparing `pyeapi-1.0.0/test/system/test_api_mlag.py` & `pyeapi-1.0.2/test/system/test_api_mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_acl.py` & `pyeapi-1.0.2/test/system/test_api_acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_ntp.py` & `pyeapi-1.0.2/test/system/test_api_ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_interfaces.py` & `pyeapi-1.0.2/test/system/test_api_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 import os
 import unittest
+from pyeapi.utils import CliVariants
 
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
 
 from testlib import random_string, random_int
 from systestlib import DutSystemTest, random_interface
-
+from time import sleep
 
 class TestResourceInterfaces(DutSystemTest):
 
     def test_get(self):
         for dut in self.duts:
             intf = random_interface(dut)
             dut.config(['default interface %s' % intf,
@@ -146,20 +147,23 @@
             with self.assertRaises(NotImplementedError):
                 dut.api('interfaces').set_encapsulation('Vlan1234',
                                                         1)
 
     def test_default(self):
         for dut in self.duts:
             intf = random_interface(dut)
+            intf_status = dut.run_commands('show interfaces %s' % intf)
+            intf_status = intf_status[0]['interfaces'][intf]['interfaceStatus']
             dut.config(['interface %s' % intf, 'shutdown'])
             result = dut.api('interfaces').default(intf)
+            sleep( 10 )  # if intf was 'connected', give it a time to come up
             self.assertTrue(result)
             config = dut.run_commands('show interfaces %s' % intf)
             config = config[0]['interfaces'][intf]
-            self.assertEqual(config['interfaceStatus'], 'connected')
+            self.assertEqual(config['interfaceStatus'], intf_status)
 
     def test_set_description(self):
         for dut in self.duts:
             text = random_string()
             intf = random_interface(dut)
             result = dut.api('interfaces').set_description(intf, text)
             self.assertTrue(result)
@@ -215,47 +219,39 @@
             dut.config('default interface %s' % intf)
             result = dut.api('interfaces').set_sflow(intf, default=True)
             self.assertTrue(result)
             config = dut.run_commands('show running-config interfaces %s' %
                                       intf, 'text')
             self.assertNotIn('no sflow enable', config[0]['output'])
 
+
     def test_set_vrf(self):
         for dut in self.duts:
             intf = random_interface(dut)
             dut.config('default interface %s' % intf)
             # Verify set_vrf returns False if no vrf by name is configured
             result = dut.api('interfaces').set_vrf(intf, 'test')
             self.assertFalse(result)
-            if dut.version_number >= '4.23':
-                dut.config('vrf instance test')
-            else:
-                dut.config('vrf definition test')
+            dut.config( CliVariants('vrf instance test', 'vrf definition test') )
             # Verify interface has vrf applied
             result = dut.api('interfaces').set_vrf(intf, 'test')
             self.assertTrue(result)
-            config = dut.run_commands('show running-config interfaces %s' %
-                                      intf, 'text')
-            if dut.version_number >= '4.23':
-                self.assertIn('vrf test', config[0]['output'])
-            else:
-                self.assertIn('vrf forwarding test', config[0]['output'])
+            config = dut.run_commands(
+                f'show running-config interfaces {intf}', 'text' )
+            self.assertIn('vrf test' if dut.version_number >= '4.23'
+                else 'vrf forwarding test', config[0]['output'])
             # Verify interface has vrf removed
             result = dut.api('interfaces').set_vrf(intf, 'test', disable=True)
             self.assertTrue(result)
-            config = dut.run_commands('show running-config interfaces %s' %
-                                      intf, 'text')
-            if dut.version_number >= '4.23':
-                self.assertIn('vrf test', config[0]['output'])
-                # Remove test vrf
-                dut.config('no vrf instance test')
-            else:
-                self.assertIn('vrf forwarding test', config[0]['output'])
-                # Remove test vrf
-                dut.config('no vrf definition test')
+            config = dut.run_commands(
+                f'show running-config interfaces {intf}', 'text' )
+            self.assertNotIn('vrf test' if dut.version_number >= '4.23'
+                else 'vrf forwarding test', config[0]['output'])
+            dut.config( CliVariants(
+                'no vrf instance test', 'no vrf definition test') )
 
 
 class TestPortchannelInterface(DutSystemTest):
 
     def test_get(self):
         for dut in self.duts:
             dut.config(['no interface Port-Channel1',
@@ -403,17 +399,17 @@
             commands = 'show running-config interfaces Port-Channel1'
             config = dut.run_commands(commands, 'text')
             self.assertIn('port-channel min-links %s' % minlinks,
                           config[0]['output'], 'dut=%s' % dut)
 
     def test_minimum_links_invalid_value(self):
         for dut in self.duts:
-            minlinks = random_int(17, 128)
-            result = dut.api('interfaces').set_minimum_links('Port-Channel1',
-                                                             minlinks)
+            minlinks = random_int(129, 256)  # some duts may support up to 128
+            result = dut.api(
+                'interfaces').set_minimum_links('Port-Channel1', minlinks)
             self.assertFalse(result)
 
     def test_create_and_delete_portchannel_sub_interface(self):
         for dut in self.duts:
             et1 = random_interface(dut)
             et2 = random_interface(dut, exclude=[et1])
 
@@ -504,14 +500,33 @@
 
     def contains(self, text, dut):
         self.assertIn(text, self.get_config(dut), 'dut=%s' % dut)
 
     def notcontains(self, text, dut):
         self.assertNotIn(text, self.get_config(dut), 'dut=%s' % dut)
 
+    def may_contain( self, text, dut, first=False, last=False ):
+        """handles multiple variants of cli, typically to handle deprecated
+        variants of the cli. The first and last calls in the variant sequence
+        must be initialized respectively. At least one call in the sequence
+        should result in a positive assertion
+        """
+        if first:
+            self.skip_rest = False
+        if self.skip_rest:
+            return
+        if last:
+            self.assertIn(text, self.get_config(dut), 'dut=%s' % dut)
+            return
+        try:
+            self.assertIn(text, self.get_config(dut), 'dut=%s' % dut)
+            self.skip_rest = True
+        except AssertionError:
+            pass
+
     def test_set_source_interface(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.set_source_interface('Vxlan1', 'Loopback0')
             self.assertTrue(instance)
             self.contains('vxlan source-interface Loopback0', dut)
@@ -536,29 +551,32 @@
 
     def test_set_multicast_group(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.set_multicast_group('Vxlan1', '239.10.10.10')
             self.assertTrue(instance)
-            self.contains('vxlan multicast-group 239.10.10.10', dut)
+            self.contains('vxlan multicast-group', dut)
+            self.contains('239.10.10.10', dut)
 
     def test_set_multicast_group_default(self):
         for dut in self.duts:
-            dut.config(['no interface Vxlan1', 'interface Vxlan1',
-                        'vxlan multicast-group 239.10.10.10'])
+            dut.config( ['no interface Vxlan1', 'interface Vxlan1',
+                CliVariants( 'vxlan multicast-group decap 239.10.10.10',
+                   'vxlan multicast-group 239.10.10.10') ])
             api = dut.api('interfaces')
             instance = api.set_multicast_group('Vxlan1', default=True)
             self.assertTrue(instance)
             self.contains('no vxlan multicast-group', dut)
 
     def test_set_multicast_group_negate(self):
         for dut in self.duts:
-            dut.config(['no interface Vxlan1', 'interface Vxlan1',
-                        'vxlan multicast-group 239.10.10.10'])
+            dut.config( ['no interface Vxlan1', 'interface Vxlan1',
+                CliVariants( 'vxlan multicast-group decap 239.10.10.10',
+                   'vxlan multicast-group 239.10.10.10') ])
             api = dut.api('interfaces')
             instance = api.set_multicast_group('Vxlan1', disable=True)
             self.assertTrue(instance)
             self.contains('no vxlan multicast-group', dut)
 
     '''commenting this one out as it will only parse on a  trident based DUT
     def test_set_multicast_decap(self):
@@ -631,20 +649,21 @@
 
     def test_update_vlan(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.update_vlan('Vxlan1', '10', '10')
             self.assertTrue(instance)
-            self.contains('vxlan vlan add 10 vni 10', dut)
+            self.may_contain('vxlan vlan 10 vni 10', dut, first=True)
+            self.may_contain('vxlan vlan add 10 vni 10', dut, last=True)
 
     def test_remove_vlan(self):
         for dut in self.duts:
             dut.config(['no interface Vxlan1', 'interface Vxlan1'])
             api = dut.api('interfaces')
             instance = api.remove_vlan('Vxlan1', '10')
             self.assertTrue(instance)
-            self.notcontains('vxlan vlan remove 10 vni 10', dut)
+            self.notcontains('vxlan vlan remove 10 vni 10 $', dut)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyeapi-1.0.0/test/system/test_api_vrfs.py` & `pyeapi-1.0.2/test/system/test_api_vrfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import unittest
 
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
 
 from testlib import random_string
 from systestlib import DutSystemTest
+from pyeapi.utils import CliVariants
 
 
 class TestApiVrfs(DutSystemTest):
 
     def test_get(self):
         for dut in self.duts:
             if dut.version_number >= '4.23':
@@ -56,29 +57,27 @@
             if dut.version_number >= '4.23':
                 dut.config(['no vrf instance blah'])
             else:
                 dut.config(['no vrf definition blah'])
 
     def test_getall(self):
         for dut in self.duts:
-            if dut.version_number >= '4.23':
-                dut.config(['no vrf instance blah', 'vrf instance blah',
-                            'no vrf instance second', 'vrf instance second'])
-            else:
-                dut.config(['no vrf definition blah', 'vrf definition blah',
-                            'no vrf definition second', 'vrf definition second'])
+            dut.config( CliVariants(
+                ['no vrf instance blah', 'vrf instance blah',
+                'no vrf instance second', 'vrf instance second'],
+                ['no vrf definition blah', 'vrf definition blah',
+                'no vrf definition second', 'vrf definition second']) )
             response = dut.api('vrfs').getall()
-            self.assertIsInstance(response, dict, 'dut=%s' % dut)
-            self.assertEqual(len(response), 2)
-            for vrf_name in ['blah', 'second']:
-                self.assertIn(vrf_name, response, 'dut=%s' % dut)
-            if dut.version_number >= '4.23':
-                dut.config(['no vrf instance blah', 'no vrf instance second'])
-            else:
-                dut.config(['no vrf definition blah', 'no vrf definition second'])
+            self.assertIsInstance( response, dict, f'dut={dut}' )
+            self.assertEqual( len(response), 2 )
+            for vrf_name in ( 'blah', 'second' ):
+                self.assertIn( vrf_name, response, f'dut={dut}' )
+            dut.config( CliVariants(
+                ['no vrf instance blah', 'no vrf instance second'],
+                ['no vrf definition blah', 'no vrf definition second']) )
 
     def test_create_and_return_true(self):
         for dut in self.duts:
             if dut.version_number >= '4.23':
                 dut.config(['no vrf instance blah', 'vrf instance blah'])
             else:
                 dut.config(['no vrf definition blah', 'vrf definition blah'])
```

### Comparing `pyeapi-1.0.0/test/system/test_api_routemaps.py` & `pyeapi-1.0.2/test/system/test_api_routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_client.py` & `pyeapi-1.0.2/test/system/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import os
 import unittest
 
 import sys
 sys.path.append(os.path.join(os.path.dirname(__file__), '../lib'))
 
 from testlib import random_int, random_string, get_fixture
-from mock import patch
+from unittest.mock import patch
 
 import pyeapi.client
 import pyeapi.eapilib
 
 
 class TestClient(unittest.TestCase):
 
@@ -113,15 +113,16 @@
             result = dut.run_commands('show version', 'json', send_enable=False)
             self.assertIsInstance(result, list, 'dut=%s' % dut)
             self.assertEqual(len(result), 1, 'dut=%s' % dut)
 
     def test_no_enable_single_command_no_auth(self):
         for dut in self.duts:
             with self.assertRaises(pyeapi.eapilib.CommandError):
-                dut.run_commands(['disable', 'show running-config'], 'json', send_enable=False)
+                dut.run_commands(['disable',
+                    'show running-config'], 'json', send_enable=False)
 
     def test_enable_multiple_commands(self):
         for dut in self.duts:
             commands = list()
             for i in range(1, random_int(10, 200)):
                 commands.append('show version')
             result = dut.run_commands(commands[:])
@@ -272,59 +273,52 @@
                 self.duts.append(pyeapi.client.connect_to(name))
 
         if not hasattr(self, 'assertRegex'):
             self.assertRegex = self.assertRegexpMatches
 
     def test_exception_trace(self):
         # Send commands that will return an error and validate the errors
-
         # General format of an error message:
-        rfmt = r'Error \[%d\]: CLI command \d+ of \d+ \'.*\' failed: %s \[%s\]'
+        rfmt = r'Error \[%d\]: CLI command \d+ of \d+ \'[^\']*\' failed: %s\[%s\]'
         # Design error tests
         cases = []
         # Send an incomplete command
-        cases.append(('show run', rfmt
-                      % (1002, 'invalid command',
-                         r'incomplete token \(at token \d+: \'.*\'\)')))
+        cases.append( ('show run', rfmt % (1002, r'invalid command \[[^[]+',
+            r'"Incomplete token \(at token \d+:[^\)]+\)"')))
         # Send a mangled command
-        cases.append(('shwo version', rfmt
-                      % (1002, 'invalid command',
-                         r'Invalid input \(at token \d+: \'.*\'\)')))
+        cases.append(('shwo version', rfmt % (1002, r'invalid command \[[^[]+',
+            r'"Invalid input \(at token \d+:[^\)]+\)"')))
         # Send a command that cannot be run through the api
         # note the command for reload looks to change in new EOS
         # in 4.15 the  reload now is replaced with 'force' if you are
         # testing some DUT running older code and this test fails
         # change the error message to the following:
         # To reload the machine over the API, please use 'reload now' instead
-        cases.append(('reload', rfmt
-                      % (1004, 'incompatible command',
-                         'Command not permitted via API access..*')))
+        cases.append(('reload', rfmt % (1004, r'incompatible command \[[^[]+',
+            r"'Command not permitted via API access\..*")))
         # Send a command that has insufficient priv
-        cases.append(('show running-config', rfmt
-                      % (1002, 'invalid command',
-                         r'Invalid input \(privileged mode required\)')))
-
+        cases.append(('show running-config', rfmt % (1002,
+            r'invalid command \[[^[]+',
+            r"'Invalid input \(privileged mode required\)'")))
         for dut in self.duts:
             for (cmd, regex) in cases:
                 try:
                     # Insert the error in list of valid commands
                     if cmd != "show running-config":
                         dut.enable(['show version', cmd, 'show hostname'],
                                    strict=True)
                     else:
                         dut.enable(['disable', 'show version', cmd],
                                    strict=True, send_enable=False)
 
                     self.fail('A CommandError should have been raised')
                 except pyeapi.eapilib.CommandError as exc:
                     # Validate the properties of the exception
-                    if cmd != 'show running-config':
-                        self.assertEqual(len(exc.trace), 4)
-                    else:
-                        self.assertEqual(len(exc.trace), 3)
+                    self.assertEqual( len(exc.trace),
+                        3 if cmd == 'show running-config' else 4 )
                     self.assertIsNotNone(exc.command_error)
                     self.assertIsNotNone(exc.output)
                     self.assertIsNotNone(exc.commands)
                     self.assertRegex(exc.message, regex)
 
 
 if __name__ == '__main__':
```

### Comparing `pyeapi-1.0.0/test/system/test_api_users.py` & `pyeapi-1.0.2/test/system/test_api_users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/system/test_api_ipinterfaces.py` & `pyeapi-1.0.2/test/system/test_api_ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/lib/testlib.py` & `pyeapi-1.0.2/test/lib/testlib.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 import os
 import random
 import string
 import unittest
 
-from mock import MagicMock as Mock
+from unittest.mock import MagicMock as Mock
+from pyeapi.utils import CliVariants
 
 from pyeapi.client import Node
 
 def get_fixtures_path():
     return os.path.join(os.path.dirname(__file__), '../fixtures')
 
 def get_fixture(filename):
@@ -90,15 +91,24 @@
         if cmds is not None:
             lcmds = len([cmds]) if isinstance(cmds, str) else len(cmds)
             self.mock_config.return_value = [{} for i in range(0, lcmds)]
 
         result = func(*fargs, **fkwargs)
 
         if cmds is not None:
-            self.node.config.assert_called_with(cmds)
+            # if config was called with CliVariants, then create all possible
+            # cli combinations with CliVariants and see if cmds is one of them
+            called_args = list( self.node.config.call_args )[ 0 ][ 0 ]
+            variants = [ x for x in called_args if isinstance(x, CliVariants) ]
+            if not variants:
+                self.node.config.assert_called_with(cmds)
+                return result
+            # process all variants
+            cli_variants = CliVariants.expand( called_args )
+            self.assertIn( cmds, cli_variants )
         else:
             self.assertEqual(self.node.config.call_count, 0)
 
         return result
 
     def eapi_positive_config_test(self, func, cmds=None, *args, **kwargs):
         result = self.eapi_config_test(func, cmds, *args, **kwargs)
```

### Comparing `pyeapi-1.0.0/test/lib/systestlib.py` & `pyeapi-1.0.2/test/lib/systestlib.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/show_interfaces.text` & `pyeapi-1.0.2/test/fixtures/show_interfaces.text`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/vxlan.json` & `pyeapi-1.0.2/test/fixtures/vxlan.json`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/show_interfaces.json` & `pyeapi-1.0.2/test/fixtures/show_interfaces.json`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.ospf` & `pyeapi-1.0.2/test/fixtures/running_config.ospf`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.text` & `pyeapi-1.0.2/test/fixtures/running_config.text`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/ipinterfaces.json` & `pyeapi-1.0.2/test/fixtures/ipinterfaces.json`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.routemaps` & `pyeapi-1.0.2/test/fixtures/running_config.routemaps`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.vxlan` & `pyeapi-1.0.2/test/fixtures/running_config.vxlan`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.vrf` & `pyeapi-1.0.2/test/fixtures/running_config.vrf`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.vrrp` & `pyeapi-1.0.2/test/fixtures/running_config.vrrp`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/test/fixtures/running_config.portchannel` & `pyeapi-1.0.2/test/fixtures/running_config.portchannel`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/Makefile` & `pyeapi-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/MANIFEST.in` & `pyeapi-1.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/.coveragerc` & `pyeapi-1.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/install.rst` & `pyeapi-1.0.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/subinterfaces.rst` & `pyeapi-1.0.2/docs/subinterfaces.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/index.rst` & `pyeapi-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/configfile.rst` & `pyeapi-1.0.2/docs/configfile.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/configsessions.rst` & `pyeapi-1.0.2/docs/configsessions.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-1.0.0.rst` & `pyeapi-1.0.2/docs/release-notes-1.0.0.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Release 1.0.0
 -------------
 
 2023-06-06
 
 - This is a Python3 (3.7 onwards) release only (Python2 is no longer supported)
-- Arista EOS 4.22 or later required
+- Arista EOS 4.22 or later required (for on-box use cases only)
 
 New Modules
 ^^^^^^^^^^^
 
 Enhancements
 ^^^^^^^^^^^^
```

### Comparing `pyeapi-1.0.0/docs/release-notes-0.4.0.rst` & `pyeapi-1.0.2/docs/release-notes-0.4.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/contribute.rst` & `pyeapi-1.0.2/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.6.0.rst` & `pyeapi-1.0.2/docs/release-notes-0.6.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes.rst` & `pyeapi-1.0.2/docs/release-notes.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Release Notes
 #############
 
 .. toctree::
     :maxdepth: 2
     :titlesonly:
 
+    release-notes-1.0.2.rst
     release-notes-1.0.0.rst
     release-notes-0.8.4.rst
     release-notes-0.8.3.rst
     release-notes-0.8.2.rst
     release-notes-0.8.1.rst
     release-notes-0.8.0.rst
     release-notes-0.7.0.rst
```

### Comparing `pyeapi-1.0.0/docs/support.rst` & `pyeapi-1.0.2/docs/support.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/Makefile` & `pyeapi-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/conf.py` & `pyeapi-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.7.0.rst` & `pyeapi-1.0.2/docs/release-notes-0.7.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/generate_modules.py` & `pyeapi-1.0.2/docs/generate_modules.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.5.0.rst` & `pyeapi-1.0.2/docs/release-notes-0.5.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/description.rst` & `pyeapi-1.0.2/docs/description.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/quickstart.rst` & `pyeapi-1.0.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/license.rst` & `pyeapi-1.0.2/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.8.2.rst` & `pyeapi-1.0.2/docs/release-notes-0.8.2.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.8.0.rst` & `pyeapi-1.0.2/docs/release-notes-0.8.0.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/docs/release-notes-0.8.1.rst` & `pyeapi-1.0.2/docs/release-notes-0.8.1.rst`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/README.md` & `pyeapi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi.egg-info/PKG-INFO` & `pyeapi-1.0.2/pyeapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeapi
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python Client for eAPI
 Home-page: https://github.com/arista-eosplus/pyeapi
 Author: Arista EOS+ CS
 Author-email: eosplus-dev@arista.com
 License: BSD-3
 Description: The Python Client for eAPI
         ==========================
@@ -29,9 +29,9 @@
 Keywords: networking arista eos eapi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System :: Networking
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `pyeapi-1.0.0/pyeapi.egg-info/SOURCES.txt` & `pyeapi-1.0.2/pyeapi.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -39,18 +39,42 @@
 docs/release-notes-0.7.0.rst
 docs/release-notes-0.8.0.rst
 docs/release-notes-0.8.1.rst
 docs/release-notes-0.8.2.rst
 docs/release-notes-0.8.3.rst
 docs/release-notes-0.8.4.rst
 docs/release-notes-1.0.0.rst
+docs/release-notes-1.0.2.rst
 docs/release-notes.rst
 docs/requirements.rst
 docs/subinterfaces.rst
 docs/support.rst
+docs/api_modules/_list_of_modules.rst
+docs/api_modules/abstract.rst
+docs/api_modules/acl.rst
+docs/api_modules/bgp.rst
+docs/api_modules/interfaces.rst
+docs/api_modules/ipinterfaces.rst
+docs/api_modules/mlag.rst
+docs/api_modules/ntp.rst
+docs/api_modules/ospf.rst
+docs/api_modules/routemaps.rst
+docs/api_modules/staticroute.rst
+docs/api_modules/stp.rst
+docs/api_modules/switchports.rst
+docs/api_modules/system.rst
+docs/api_modules/users.rst
+docs/api_modules/varp.rst
+docs/api_modules/vlans.rst
+docs/api_modules/vrfs.rst
+docs/api_modules/vrrp.rst
+docs/client_modules/_list_of_modules.rst
+docs/client_modules/client.rst
+docs/client_modules/eapilib.rst
+docs/client_modules/utils.rst
 examples/get_config.py
 examples/nodes.conf
 examples/simple.py
 examples/sysmac.py
 examples/vlans_api.py
 pyeapi/__init__.py
 pyeapi/client.py
```

### Comparing `pyeapi-1.0.0/pyeapi/client.py` & `pyeapi-1.0.2/pyeapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -658,14 +658,16 @@
         """
         commands = make_iterable(commands)
         commands = list(commands)
 
         # push the configure command onto the command stack
         commands.insert(0, 'configure terminal')
         response = self.run_commands(commands, **kwargs)
+        # after config change the _chunkify lru_cache has to be cleared
+        self._chunkify.cache_clear()
 
         if self.autorefresh:
             self.refresh()
 
         # pop the configure command output off the stack
         response.pop(0)
 
@@ -680,14 +682,16 @@
 
         commands = make_iterable(commands)
         commands = list(commands)
 
         # push the configure command onto the command stack
         commands.insert(0, 'configure session %s' % self._session_name)
         response = self.run_commands(commands, **kwargs)
+        # after config change the _chunkify lru_cache has to be cleared
+        self._chunkify.cache_clear()
 
         # pop the configure command output off the stack
         response.pop(0)
 
         return response
 
     @lru_cache(maxsize=None)
```

### Comparing `pyeapi-1.0.0/pyeapi/__init__.py` & `pyeapi-1.0.2/pyeapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 # OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 # IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-__version__ = '1.0.0'
+__version__ = '1.0.2'
 __author__ = 'Arista EOS+'
 
 
 from .client import load_config, connect, connect_to, config_for
 
 __all__ = ['load_config', 'connect', 'connect_to', 'config_for']
```

### Comparing `pyeapi-1.0.0/pyeapi/utils.py` & `pyeapi-1.0.2/pyeapi/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -239,14 +239,40 @@
     period for a deprecated cli)
 
     Instance must be initialized either with 2 or more str variants:
         ``CliVariants( 'new cli', 'legacy cli' )``,
     or with 2 or more sequences of cli (or a mix of list and str types), e.g.:
         ``CliVariants( ['new cli1', 'new cli2'], 'alt cli3', 'legacy cli4' )``
     """
+    @staticmethod
+    def expand( cmds ):
+        """ Expands cmds argument into a list of all CLI variants 
+        
+        The method returns a list of all full variant combinations present
+        in the the cmds arguement
+
+        Args:
+            cmds (list): a list made of str and CliVariants types 
+
+        Returns:
+            expanded list, e.g.:
+                expand( 'x', CliVariants( 'a', 'b'), 'y' )
+                will return: [ ['x', 'a', 'y'], ['x', 'b', 'y'] ]
+        """
+        assert isinstance(cmds, list), 'argument cmds must be list type'
+        if not cmds:
+            return [ [] ]
+        head = cmds[0]
+        tail = cmds[1:]
+        if isinstance( head, CliVariants ):
+            return [ v + e for v in head.variants
+                for e in CliVariants.expand( tail ) ]
+        else:
+            return [ [head] + e for e in CliVariants.expand(tail) ]
+
     def __init__(self, *cli):
         assert len( cli ) >= 2, 'must be initialized with 2 or more arguments'
         self.variants = [ v if not isinstance(v,
             str) and isinstance(v, Iterable) else [v] for v in cli ]
 
 
 def _interpolate_docstr( *tkns ):
```

### Comparing `pyeapi-1.0.0/pyeapi/api/abstract.py` & `pyeapi-1.0.2/pyeapi/api/abstract.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/interfaces.py` & `pyeapi-1.0.2/pyeapi/api/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         for the interface.  Valid values are on or off
 
 """
 
 import re
 
 from pyeapi.api import EntityCollection
-from pyeapi.utils import ProxyCall
+from pyeapi.utils import ProxyCall, CliVariants
 
 MIN_LINKS_RE = re.compile(r'(?<=\s{3}min-links\s)(?P<value>.+)$', re.M)
 
 DEFAULT_LACP_MODE = 'on'
 DEFAULT_LACP_FALLBACK = 'disabled'
 DEFAULT_LACP_FALLBACK_TIMEOUT = 90
 
@@ -880,16 +880,17 @@
         match = re.search(r'vxlan multicast-group '
                           r'([\d]{3}\.[\d]+\.[\d]+\.[\d]+)',
                           config)
         value = match.group(1) if match else self.DEFAULT_MCAST_GRP
         return dict(multicast_group=value)
 
     def _parse_multicast_decap(self, config):
-        value = 'vxlan multicast-group decap' in config
-        return dict(multicast_decap=bool(value))
+        val1 = 'vxlan multicast-group decap' in config
+        val2 = 'no vxlan multicast-group decap' in config
+        return dict( multicast_decap=bool(val1 ^ val2) )
 
     def _parse_udp_port(self, config):
         match = re.search(r'vxlan udp-port (\d+)', config)
         value = int(match.group(1))
         return dict(udp_port=value)
 
     def _parse_vlans(self, config):
@@ -952,18 +953,22 @@
            value(str): The value to configure the multicast-group to
            default(bool): Configures the mulitcast-group value to default
            disable(bool): Negates the multicast-group value
 
         Returns:
             True if the operation succeeds otherwise False
         """
-        string = 'vxlan multicast-group'
-        cmds = self.command_builder(string, value=value, default=default,
-                                    disable=disable)
-        return self.configure_interface(name, cmds)
+        string_dpr = 'vxlan multicast-group'
+        cmds_dpr = self.command_builder(string_dpr,
+            value=value, default=default, disable=disable)
+        string_new = 'vxlan multicast-group decap'
+        cmds_new = self.command_builder(string_new,
+            value=value, default=default, disable=disable)
+        return self.configure_interface(name,
+            CliVariants(cmds_new, cmds_dpr) )
 
     def set_multicast_decap(self, name, default=False,
                             disable=False):
         """Configures the Vxlan multicast-group decap feature
 
         EosVersion:
             4.15.0M
@@ -1076,15 +1081,17 @@
         Args:
             vlan (str, int): The vlan id to map to the vni
 
         Returns:
             True if the command completes successfully
 
         """
-        return self.configure_interface(name, 'vxlan vlan remove %s vni' % vid)
+        return self.configure_interface( name,
+            CliVariants(f'vxlan vlan remove {vid} vni $',
+                f'vxlan vlan remove {vid} vni') )
 
 
 INTERFACE_CLASS_MAP = {
     'Et': EthernetInterface,
     'Po': PortchannelInterface,
     'Vx': VxlanInterface
 }
```

### Comparing `pyeapi-1.0.0/pyeapi/api/system.py` & `pyeapi-1.0.2/pyeapi/api/system.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/users.py` & `pyeapi-1.0.2/pyeapi/api/users.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/bgp.py` & `pyeapi-1.0.2/pyeapi/api/bgp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/vrfs.py` & `pyeapi-1.0.2/pyeapi/api/vrfs.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/__init__.py` & `pyeapi-1.0.2/pyeapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/ntp.py` & `pyeapi-1.0.2/pyeapi/api/ntp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/mlag.py` & `pyeapi-1.0.2/pyeapi/api/mlag.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/acl.py` & `pyeapi-1.0.2/pyeapi/api/acl.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/ipinterfaces.py` & `pyeapi-1.0.2/pyeapi/api/ipinterfaces.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/routemaps.py` & `pyeapi-1.0.2/pyeapi/api/routemaps.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/vrrp.py` & `pyeapi-1.0.2/pyeapi/api/vrrp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/ospf.py` & `pyeapi-1.0.2/pyeapi/api/ospf.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/staticroute.py` & `pyeapi-1.0.2/pyeapi/api/staticroute.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/switchports.py` & `pyeapi-1.0.2/pyeapi/api/switchports.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/vlans.py` & `pyeapi-1.0.2/pyeapi/api/vlans.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/stp.py` & `pyeapi-1.0.2/pyeapi/api/stp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/api/varp.py` & `pyeapi-1.0.2/pyeapi/api/varp.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/pyeapi/eapilib.py` & `pyeapi-1.0.2/pyeapi/eapilib.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,22 +429,24 @@
             if self._auth:
                 self.transport.putheader(*self._auth)
             data = data.encode()
 
             self.transport.endheaders(message_body=data)
             response = self.transport.getresponse()
             response_content = response.read()
+            if isinstance( response_content, bytes ):
+                response_content = response_content.decode()
             _LOGGER.debug('Response: status:{status}, reason:{reason}'.format(
                           status=response.status,
                           reason=response.reason))
             _LOGGER.debug('Response content: {}'.format(response_content))
 
             if response.status == 401:
-                raise ConnectionError(str(self), '%s. %s' % (response.reason,
-                                                             response_content))
+                raise ConnectionError(str(self),
+                    f'{response.reason}. {response_content}')
 
             # Python 3.7 json.loads() works with bytes or strings,
             # thus no decoding is required
             decoded = json.loads(response_content)
             _LOGGER.debug('eapi_response: %s' % decoded)
 
             if 'error' in decoded:
```

### Comparing `pyeapi-1.0.0/setup.py` & `pyeapi-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyeapi-1.0.0/examples/vlans_api.py` & `pyeapi-1.0.2/examples/vlans_api.py`

 * *Files identical despite different names*

