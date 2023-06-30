# Comparing `tmp/pcdsdevices-7.4.0.tar.gz` & `tmp/pcdsdevices-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdsdevices-7.4.0.tar", last modified: Tue May  9 00:02:58 2023, max compression
+gzip compressed data, was "pcdsdevices-7.4.1.tar", last modified: Fri Jun 30 20:59:18 2023, max compression
```

## Comparing `pcdsdevices-7.4.0.tar` & `pcdsdevices-7.4.1.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)     1265 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/README.inc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.741744 pcdsdevices-7.4.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/base_classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/mv.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/presets.rst
--rw-r--r--   0 runner    (1001) docker     (122)    77002 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/signals.rst
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/sim_types.rst
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/tab.rst
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/ui.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/template-short.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/update_api_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/view-build.sh
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      168 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/make_ophyd_device
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.761744 pcdsdevices-7.4.0/pcdsdevices/
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/_html.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/analog_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/areadetector/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/cam.py
--rw-r--r--   0 runner    (1001) docker     (122)    19375 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/detectors.py
--rw-r--r--   0 runner    (1001) docker     (122)     6459 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/atm.py
--rw-r--r--   0 runner    (1001) docker     (122)    60210 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/attenuator.py
--rw-r--r--   0 runner    (1001) docker     (122)    12442 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    39229 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ccm.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/cvmi_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/delay_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    17619 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/device_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    30560 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/digitizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/doc_stubs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    51429 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/evr.py
--rw-r--r--   0 runner    (1001) docker     (122)    14511 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/fms.py
--rw-r--r--   0 runner    (1001) docker     (122)    16504 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/gauge.py
--rw-r--r--   0 runner    (1001) docker     (122)    22654 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/gon.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/happi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29150 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/inout.py
--rw-r--r--   0 runner    (1001) docker     (122)    64069 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ipm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/jet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lamp_motion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/lasers/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19804 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/btms_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    22910 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/btps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/counters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/dicon.py
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/ek9000.py
--rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/elliptec.py
--rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/qmini.py
--rw-r--r--   0 runner    (1001) docker     (122)    15417 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/rfof.py
--rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/thorlabsWFS.py
--rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/tuttifrutti.py
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/zoomtelescope.py
--rw-r--r--   0 runner    (1001) docker     (122)    21112 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lens.py
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lic.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/light_control.py
--rw-r--r--   0 runner    (1001) docker     (122)    74029 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lodcm.py
--rw-r--r--   0 runner    (1001) docker     (122)    16653 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lxe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/make_ophyd_device.py
--rw-r--r--   0 runner    (1001) docker     (122)    49040 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mirror.py
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/movablestand.py
--rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mpod.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8327 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mrco_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mv_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/piezo.py
--rw-r--r--   0 runner    (1001) docker     (122)    20301 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pim.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pmps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7358 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)    39960 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pump.py
--rw-r--r--   0 runner    (1001) docker     (122)     5607 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pv_positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/radiation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ref.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/rs_powersupply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/rtds_ebd.py
--rw-r--r--   0 runner    (1001) docker     (122)    11767 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11909 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)    58121 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sim.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/slits.py
--rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (122)    29013 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     6245 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/stopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sxr_test_absorber.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tags.py
--rw-r--r--   0 runner    (1001) docker     (122)    48269 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.777744 pcdsdevices-7.4.0/pcdsdevices/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_analog_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_atm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_attenuator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    14520 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_btms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10004 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ccm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_disconnected.py
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_evr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_gauge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8654 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_gon.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_inout.py
--rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ipm.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_jet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.777744 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/original.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/test
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lic.py
--rw-r--r--   0 runner    (1001) docker     (122)    19101 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lodcm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lxe.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_movablestand.py
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod.py
--rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pim.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pump.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     5738 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_slits.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10914 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    17153 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_timetool.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_valve.py
--rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_variety.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_wfs.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa
--rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/timetool.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/type_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/pcdsdevices/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    25452 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    18911 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4876 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    22407 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
--rw-r--r--   0 runner    (1001) docker     (122)    17847 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    41696 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    25557 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    60307 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/JJSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/LCP.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/Leviton1.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/LightControl.ui
--rw-r--r--   0 runner    (1001) docker     (122)    51167 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    34999 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    24349 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10488 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/Setra5000.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10138 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10236 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/at2l0_filters.json
--rw-r--r--   0 runner    (1001) docker     (122)    15242 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-camera-summary.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12171 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)    33295 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12410 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)     9784 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-summary.ui
--rw-r--r--   0 runner    (1001) docker     (122)    46416 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-dest.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-valves.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/detailed_tree.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/usb_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    27787 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23272 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/valve.py
--rw-r--r--   0 runner    (1001) docker     (122)     9015 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/variety.py
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/wfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.761744 pcdsdevices-7.4.0/pcdsdevices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8262 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.259711 pcdsdevices-7.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.227711 pcdsdevices-7.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.227711 pcdsdevices-7.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-06-30 20:59:18.259711 pcdsdevices-7.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.227711 pcdsdevices-7.4.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.227711 pcdsdevices-7.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.227711 pcdsdevices-7.4.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/README.inc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.223711 pcdsdevices-7.4.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.231711 pcdsdevices-7.4.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/base_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/mv.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/presets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    77336 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/sim_types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/tab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/ui.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.231711 pcdsdevices-7.4.1/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/update_api_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/docs-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      168 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/make_ophyd_device
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.239711 pcdsdevices-7.4.1/pcdsdevices/
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/analog_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.239711 pcdsdevices-7.4.1/pcdsdevices/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/areadetector/cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19375 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/areadetector/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6459 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/areadetector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60210 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12442 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39229 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/cvmi_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/delay_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17619 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30560 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/doc_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51429 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14511 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/fms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16504 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22654 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/gon.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.243711 pcdsdevices-7.4.1/pcdsdevices/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29150 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64069 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lamp_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.243711 pcdsdevices-7.4.1/pcdsdevices/lasers/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19804 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/btms_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22910 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/btps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/counters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/dicon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/ek9000.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/elliptec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/qmini.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15417 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/rfof.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/thorlabsWFS.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/tuttifrutti.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lasers/zoomtelescope.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21112 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/light_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74029 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16653 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/make_ophyd_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49040 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mpod.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8327 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mrco_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/mv_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/piezo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20301 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pmps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7358 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39960 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5607 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/radiation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/rs_powersupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/rtds_ebd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11767 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11909 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58121 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/sim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29013 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6245 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/stopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/sxr_test_absorber.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48269 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.251711 pcdsdevices-7.4.1/pcdsdevices/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_analog_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14520 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_btms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10004 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8654 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_gon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.251711 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens_sets/original.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens_sets/test
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lens_sets/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19101 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_mpod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5738 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10914 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17153 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/test_wfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/tests/xcslt8717_wpcalib_opa
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.259711 pcdsdevices-7.4.1/pcdsdevices/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AT1K2.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AT1K2.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AT2L0.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25452 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    18911 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4876 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22407 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    17847 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_filter.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffAxis.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffAxis.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    41696 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25557 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BtpsState.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/BtpsState.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    60307 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/JJSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/LCP.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/Leviton1.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/LightControl.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    51167 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/PowerSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    34999 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/PowerSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    27032 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/QminiSpectrometer.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10488 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/Setra5000.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10138 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/StatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/StatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10236 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/at2l0_filters.json
+-rw-r--r--   0 runner    (1001) docker     (122)    15242 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-camera-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12171 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    33295 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12410 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-range-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9784 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-range-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    46416 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-dest.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-tabs-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-tabs.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-valves.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/btps.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/ui/detailed_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/usb_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27787 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23272 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9015 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pcdsdevices/wfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 20:59:18.239711 pcdsdevices-7.4.1/pcdsdevices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8262 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-30 20:59:18.000000 pcdsdevices-7.4.1/pcdsdevices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-06-30 20:59:01.000000 pcdsdevices-7.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 20:59:18.259711 pcdsdevices-7.4.1/setup.cfg
```

### Comparing `pcdsdevices-7.4.0/.github/ISSUE_TEMPLATE.md` & `pcdsdevices-7.4.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `pcdsdevices-7.4.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/.github/workflows/standard.yml` & `pcdsdevices-7.4.1/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/.pre-commit-config.yaml` & `pcdsdevices-7.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/CONTRIBUTING.rst` & `pcdsdevices-7.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/LICENSE.md` & `pcdsdevices-7.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/PKG-INFO` & `pcdsdevices-7.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 7.4.0
+Version: 7.4.1
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.0 Summary: Ophyd Device
+Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.1 Summary: Ophyd Device
 definitions for LCLS Beamline components Author: SLAC National Accelerator
 Laboratory License: Copyright (c) 2023, The Board of Trustees of the Leland
 Stanford Junior University, through SLAC National Accelerator Laboratory
 (subject to receipt of any required approvals from the U.S. Dept. of Energy).
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: (1) Redistributions of source code must retain the above copyright notice,
```

### Comparing `pcdsdevices-7.4.0/README.md` & `pcdsdevices-7.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/conda-recipe/meta.yaml` & `pcdsdevices-7.4.1/conda-recipe/meta.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     - pyepics >=3.4.2
     - pytmc >=2.7.0
     - pyyaml
     - schema
     - scipy
   run_constrained:
     - pmgr >=2.0.2
-    - pyqt <5.15
     - typhos >=2.4.0
     # Note: these should be removed once a newer xraylib is available on conda-forge
     # or moved to pcdscalc after testing
     - sqlalchemy <2.0.0
     - xraydb <4.5.0
 
 test:
```

### Comparing `pcdsdevices-7.4.0/docs/Makefile` & `pcdsdevices-7.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/pre-release-notes.sh` & `pcdsdevices-7.4.1/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/release_notes.py` & `pcdsdevices-7.4.1/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/README.inc` & `pcdsdevices-7.4.1/docs/source/README.inc`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/_templates/autosummary/class.rst` & `pcdsdevices-7.4.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/_templates/autosummary/module.rst` & `pcdsdevices-7.4.1/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/api.rst` & `pcdsdevices-7.4.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/base_classes.rst` & `pcdsdevices-7.4.1/docs/source/base_classes.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/conf.py` & `pcdsdevices-7.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/mv.rst` & `pcdsdevices-7.4.1/docs/source/mv.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/presets.rst` & `pcdsdevices-7.4.1/docs/source/presets.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/releases.rst` & `pcdsdevices-7.4.1/docs/source/releases.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 Release History
 ###############
 
 
+v7.4.1 (2023-06-30)
+===================
+
+Device Updates
+--------------
+- QminiSpectrometer: Added some new PVs and modified others related to recent
+  IOC changes. Embedded UI was updated to reflect this.
+
+Maintenance
+-----------
+- unpin pyqt, with the hope of supporting py3.11
+
+Contributors
+------------
+- slactjohnson
+- tangkong
+
+
 v7.4.0 (2023-05-08)
 ===================
 
 Device Updates
 --------------
 - `IMS` class:
```

### Comparing `pcdsdevices-7.4.0/docs/source/signals.rst` & `pcdsdevices-7.4.1/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/tab.rst` & `pcdsdevices-7.4.1/docs/source/tab.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/source/upcoming_release_notes/template-full.rst` & `pcdsdevices-7.4.1/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/docs/update_api_list.py` & `pcdsdevices-7.4.1/docs/update_api_list.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/__init__.py` & `pcdsdevices-7.4.1/pcdsdevices/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/_html.py` & `pcdsdevices-7.4.1/pcdsdevices/_html.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/analog_signals.py` & `pcdsdevices-7.4.1/pcdsdevices/analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/areadetector/cam.py` & `pcdsdevices-7.4.1/pcdsdevices/areadetector/cam.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/areadetector/detectors.py` & `pcdsdevices-7.4.1/pcdsdevices/areadetector/detectors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/areadetector/plugins.py` & `pcdsdevices-7.4.1/pcdsdevices/areadetector/plugins.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/atm.py` & `pcdsdevices-7.4.1/pcdsdevices/atm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/attenuator.py` & `pcdsdevices-7.4.1/pcdsdevices/attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/beam_stats.py` & `pcdsdevices-7.4.1/pcdsdevices/beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ccm.py` & `pcdsdevices-7.4.1/pcdsdevices/ccm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/crix_motion.py` & `pcdsdevices-7.4.1/pcdsdevices/crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/cvmi_motion.py` & `pcdsdevices-7.4.1/pcdsdevices/cvmi_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/dc_devices.py` & `pcdsdevices-7.4.1/pcdsdevices/dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/delay_generator.py` & `pcdsdevices-7.4.1/pcdsdevices/delay_generator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/device.py` & `pcdsdevices-7.4.1/pcdsdevices/device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/device_types.py` & `pcdsdevices-7.4.1/pcdsdevices/device_types.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/digitizers.py` & `pcdsdevices-7.4.1/pcdsdevices/digitizers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/doc_stubs.py` & `pcdsdevices-7.4.1/pcdsdevices/doc_stubs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/energy_monitor.py` & `pcdsdevices-7.4.1/pcdsdevices/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/epics_motor.py` & `pcdsdevices-7.4.1/pcdsdevices/epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/evr.py` & `pcdsdevices-7.4.1/pcdsdevices/evr.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/fms.py` & `pcdsdevices-7.4.1/pcdsdevices/fms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/gauge.py` & `pcdsdevices-7.4.1/pcdsdevices/gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/gon.py` & `pcdsdevices-7.4.1/pcdsdevices/gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/happi/containers.py` & `pcdsdevices-7.4.1/pcdsdevices/happi/containers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/inout.py` & `pcdsdevices-7.4.1/pcdsdevices/inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/interface.py` & `pcdsdevices-7.4.1/pcdsdevices/interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ipm.py` & `pcdsdevices-7.4.1/pcdsdevices/ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/jet.py` & `pcdsdevices-7.4.1/pcdsdevices/jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lamp_motion.py` & `pcdsdevices-7.4.1/pcdsdevices/lamp_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/btms_config.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/btms_config.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/btps.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/btps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/counters.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/counters.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/dicon.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/dicon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/ek9000.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/ek9000.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/elliptec.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/elliptec.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/qmini.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/qmini.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
                      write_pv=':SET_TRIG_DELAY', kind='config')
     trig_pin = Cpt(EpicsSignal, ':TRIG_PIN_RBV', write_pv=':SET_TRIG_PIN',
                    kind='config')
     trig_edge = Cpt(EpicsSignal, ':TRIG_EDGE_RBV', write_pv=':SET_TRIG_EDGE',
                     kind='config')
     trig_enable = Cpt(EpicsSignal, ':GET_TRIG_ENABLE',
                       write_pv=':SET_TRIG_ENABLE', kind='config')
-    scan_rate = Cpt(EpicsSignal, ':GET_SPECTRUM.SCAN', kind='config')
+    acquisition_mode = Cpt(EpicsSignal, ':SOFT_TRIGGER_MODE', kind='config')
+    exposures_to_average = Cpt(EpicsSignal, ':SET_AVG_CNT', kind='config')
+    force_trig = Cpt(EpicsSignal, ':START_EXPOSURE.PROC', kind='config')
+    set_metadata(force_trig, dict(variety='command-proc', value=1))
     reset = Cpt(EpicsSignal, ':CLEAR_SPECTROMETER', kind='config')
     set_metadata(reset, dict(variety='command-proc', value=1))
     spectrum = Cpt(EpicsSignalRO, ':SPECTRUM', kind='normal')
     wavelengths = Cpt(EpicsSignalRO, ':WAVELENGTHS', kind='normal')
 
     model = Cpt(EpicsSignalRO, ':MODEL_CODE', kind='config')
     set_metadata(model, dict(variety='scalar', display_format='hex'))
```

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/rfof.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/rfof.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/thorlabsWFS.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/thorlabsWFS.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/tuttifrutti.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/tuttifrutti.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lasers/zoomtelescope.py` & `pcdsdevices-7.4.1/pcdsdevices/lasers/zoomtelescope.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lens.py` & `pcdsdevices-7.4.1/pcdsdevices/lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lic.py` & `pcdsdevices-7.4.1/pcdsdevices/lic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/light_control.py` & `pcdsdevices-7.4.1/pcdsdevices/light_control.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lodcm.py` & `pcdsdevices-7.4.1/pcdsdevices/lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/lxe.py` & `pcdsdevices-7.4.1/pcdsdevices/lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/make_ophyd_device.py` & `pcdsdevices-7.4.1/pcdsdevices/make_ophyd_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/mirror.py` & `pcdsdevices-7.4.1/pcdsdevices/mirror.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/movablestand.py` & `pcdsdevices-7.4.1/pcdsdevices/movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/mpod.py` & `pcdsdevices-7.4.1/pcdsdevices/mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/mpod_apalis.py` & `pcdsdevices-7.4.1/pcdsdevices/mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/mps.py` & `pcdsdevices-7.4.1/pcdsdevices/mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/mrco_motion.py` & `pcdsdevices-7.4.1/pcdsdevices/mrco_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/piezo.py` & `pcdsdevices-7.4.1/pcdsdevices/piezo.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pim.py` & `pcdsdevices-7.4.1/pcdsdevices/pim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pmps.py` & `pcdsdevices-7.4.1/pcdsdevices/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pneumatic.py` & `pcdsdevices-7.4.1/pcdsdevices/pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/positioner.py` & `pcdsdevices-7.4.1/pcdsdevices/positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pseudopos.py` & `pcdsdevices-7.4.1/pcdsdevices/pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pulsepicker.py` & `pcdsdevices-7.4.1/pcdsdevices/pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pump.py` & `pcdsdevices-7.4.1/pcdsdevices/pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/pv_positioner.py` & `pcdsdevices-7.4.1/pcdsdevices/pv_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/radiation.py` & `pcdsdevices-7.4.1/pcdsdevices/radiation.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ref.py` & `pcdsdevices-7.4.1/pcdsdevices/ref.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/rs_powersupply.py` & `pcdsdevices-7.4.1/pcdsdevices/rs_powersupply.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/rtds_ebd.py` & `pcdsdevices-7.4.1/pcdsdevices/rtds_ebd.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/sample_delivery.py` & `pcdsdevices-7.4.1/pcdsdevices/sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/sensors.py` & `pcdsdevices-7.4.1/pcdsdevices/sensors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/sequencer.py` & `pcdsdevices-7.4.1/pcdsdevices/sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/signal.py` & `pcdsdevices-7.4.1/pcdsdevices/signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/sim.py` & `pcdsdevices-7.4.1/pcdsdevices/sim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/slits.py` & `pcdsdevices-7.4.1/pcdsdevices/slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/spectrometer.py` & `pcdsdevices-7.4.1/pcdsdevices/spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/state.py` & `pcdsdevices-7.4.1/pcdsdevices/state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/stopper.py` & `pcdsdevices-7.4.1/pcdsdevices/stopper.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/sxr_test_absorber.py` & `pcdsdevices-7.4.1/pcdsdevices/sxr_test_absorber.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/targets.py` & `pcdsdevices-7.4.1/pcdsdevices/targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/conftest.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_analog_signals.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_attenuator.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_beam_stats.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_btms.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_btms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_ccm.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_ccm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_crix_motion.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_dc_devices.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_device.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_disconnected.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_disconnected.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_entrypoints.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_epics_motor.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_gauge.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_gon.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_inout.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_interface.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_ipm.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_jet.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_lens.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_lodcm.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_lxe.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_mirror.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_movablestand.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod_apalis.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_mps.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_pim.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_pim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_pneumatic.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_positioner.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_pseudopos.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_pulsepicker.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_pump.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_sample_delivery.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_sequencer.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_signal.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_slits.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_spectrometer.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_state.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_targets.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_timetool.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_utils.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_valve.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/test_variety.py` & `pcdsdevices-7.4.1/pcdsdevices/tests/test_variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa` & `pcdsdevices-7.4.1/pcdsdevices/tests/xcslt8717_wpcalib_opa`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/timetool.py` & `pcdsdevices-7.4.1/pcdsdevices/timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/type_hints.py` & `pcdsdevices-7.4.1/pcdsdevices/type_hints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AT1K2.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AT1K2.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AT2L0.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorCalculator_filter.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffAxis.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffAxis.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BeckhoffSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BtpsState.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/BtpsState.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/JJSlits.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/JJSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/LCP.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/LCP.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/Leviton1.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/Leviton1.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/LightControl.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/LightControl.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/PowerSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/PowerSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/QminiSpectrometer.embedded.ui`

 * *Files 3% similar despite different names*

#### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/QminiSpectrometer.embedded.ui`

```diff
@@ -122,15 +122,15 @@
             <bool>true</bool>
           </property>
           <property name="sceneRect">
             <rectf>
               <x>0.000000000000000</x>
               <y>0.000000000000000</y>
               <width>522.000000000000000</width>
-              <height>279.000000000000000</height>
+              <height>280.000000000000000</height>
             </rectf>
           </property>
           <property name="alignment">
             <set>Qt::AlignBottom|Qt::AlignLeading|Qt::AlignLeft</set>
           </property>
           <property name="renderHints">
             <set>QPainter::TextAntialiasing</set>
@@ -166,39 +166,39 @@
             <bool>false</bool>
           </property>
           <property name="xLabels">
             <stringlist>
               <string>Wavelength</string>
             </stringlist>
           </property>
-          <property name="yLabels">
-            <stringlist>
-              <string>Spectrum</string>
-            </stringlist>
-          </property>
           <property name="showLegend">
             <bool>false</bool>
           </property>
           <property name="mouseEnabledX" stdset="0">
             <bool>true</bool>
           </property>
           <property name="mouseEnabledY" stdset="0">
             <bool>true</bool>
           </property>
           <property name="curves">
             <stringlist>
-              <string>{&quot;y_channel&quot;: &quot;ca://$prefix:SPECTRUM&quot;, &quot;x_channel&quot;: &quot;ca://$prefix:WAVELENGTHS&quot;, &quot;name&quot;: &quot;&quot;, &quot;color&quot;: &quot;#0055ff&quot;, &quot;lineStyle&quot;: 1, &quot;lineWidth&quot;: 1, &quot;symbol&quot;: null, &quot;symbolSize&quot;: 10, &quot;redraw_mode&quot;: 1}</string>
+              <string>{&quot;y_channel&quot;: &quot;ca://$prefix:SPECTRUM&quot;, &quot;x_channel&quot;: &quot;ca://$prefix:WAVELENGTHS&quot;, &quot;plot_style&quot;: null, &quot;name&quot;: &quot;&quot;, &quot;color&quot;: &quot;#0055ff&quot;, &quot;lineStyle&quot;: 1, &quot;lineWidth&quot;: 1, &quot;symbol&quot;: null, &quot;symbolSize&quot;: 10, &quot;yAxisName&quot;: &quot;Axis 1&quot;, &quot;barWidth&quot;: null, &quot;upperThreshold&quot;: null, &quot;lowerThreshold&quot;: null, &quot;thresholdColor&quot;: &quot;white&quot;, &quot;redraw_mode&quot;: 1}</string>
             </stringlist>
           </property>
           <property name="autoRangeX">
             <bool>true</bool>
           </property>
           <property name="autoRangeY">
             <bool>true</bool>
           </property>
+          <property name="yLabels" stdset="0">
+            <stringlist>
+              <string>Spectrum</string>
+            </stringlist>
+          </property>
         </widget>
       </item>
       <item>
         <spacer name="verticalSpacer">
           <property name="orientation">
             <enum>Qt::Vertical</enum>
           </property>
@@ -222,16 +222,16 @@
             <bool>true</bool>
           </property>
           <widget class="QWidget" name="Parameters_scroll">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>520</width>
-                <height>251</height>
+                <width>571</width>
+                <height>236</height>
               </rect>
             </property>
             <property name="sizePolicy">
               <sizepolicy hsizetype="Preferred" vsizetype="MinimumExpanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
@@ -307,21 +307,39 @@
                             <height>18</height>
                           </size>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>Status</string>
+                          <string>ca://$prefix:STATUS</string>
                         </property>
                         <property name="textFormat">
                           <enum>Qt::PlainText</enum>
                         </property>
+                        <property name="precision" stdset="0">
+                          <number>0</number>
+                        </property>
+                        <property name="showUnits" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="precisionFromPV" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="alarmSensitiveContent" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="alarmSensitiveBorder" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="PyDMToolTip" stdset="0">
+                          <string/>
+                        </property>
                         <property name="channel" stdset="0">
-                          <string>ca://${prefix}:STATUS</string>
+                          <string>ca://$prefix:STATUS</string>
                         </property>
                       </widget>
                     </item>
                     <item row="1" column="0">
                       <widget class="QLabel" name="scan_rate_label">
                         <property name="text">
                           <string>Scan Rate</string>
@@ -330,34 +348,61 @@
                     </item>
                     <item row="1" column="1">
                       <widget class="PyDMLabel" name="scan_rate">
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>Scan_Rate</string>
+                          <string>ca://$prefix:SOFT_TRIGGER_MODE</string>
+                        </property>
+                        <property name="precision" stdset="0">
+                          <number>0</number>
+                        </property>
+                        <property name="showUnits" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="precisionFromPV" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="alarmSensitiveContent" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="alarmSensitiveBorder" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="PyDMToolTip" stdset="0">
+                          <string/>
                         </property>
                         <property name="channel" stdset="0">
-                          <string>ca://$prefix:GET_SPECTRUM.SCAN</string>
+                          <string>ca://$prefix:SOFT_TRIGGER_MODE</string>
                         </property>
                       </widget>
                     </item>
                     <item row="2" column="1">
                       <widget class="PyDMEnumComboBox" name="PyDMEnumComboBox">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
+                        <property name="alarmSensitiveContent" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="alarmSensitiveBorder" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="PyDMToolTip" stdset="0">
+                          <string/>
+                        </property>
                         <property name="channel" stdset="0">
-                          <string>ca://$prefix:GET_SPECTRUM.SCAN</string>
+                          <string>ca://$prefix:SOFT_TRIGGER_MODE</string>
                         </property>
                       </widget>
                     </item>
                     <item row="3" column="0">
                       <widget class="QLabel" name="trig_enable_label">
                         <property name="text">
                           <string>Trig Enable</string>
@@ -366,15 +411,15 @@
                     </item>
                     <item row="3" column="1">
                       <widget class="PyDMLabel" name="trig_enable">
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>Trig_Enable</string>
+                          <string>ca://$prefix:SET_TRIG_ENABLE</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:SET_TRIG_ENABLE</string>
                         </property>
                       </widget>
                     </item>
                     <item row="4" column="1">
@@ -402,15 +447,33 @@
                     </item>
                     <item row="5" column="1">
                       <widget class="PyDMLabel" name="temperature">
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>Temperature</string>
+                          <string/>
+                        </property>
+                        <property name="precision" stdset="0">
+                          <number>0</number>
+                        </property>
+                        <property name="showUnits" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="precisionFromPV" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="alarmSensitiveContent" stdset="0">
+                          <bool>false</bool>
+                        </property>
+                        <property name="alarmSensitiveBorder" stdset="0">
+                          <bool>true</bool>
+                        </property>
+                        <property name="PyDMToolTip" stdset="0">
+                          <string/>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:TEMP</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
@@ -478,15 +541,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>fit_on</string>
+                          <string>ca://$prefix:FIT_ON</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:FIT_ON</string>
                         </property>
                       </widget>
                     </item>
                     <item row="3" column="0">
@@ -510,15 +573,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>w0_guess</string>
+                          <string>ca://$prefix:W0_GUESS</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:W0_GUESS</string>
                         </property>
                       </widget>
                     </item>
                     <item row="4" column="0">
@@ -548,15 +611,15 @@
                             <height>18</height>
                           </size>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>w0_fit</string>
+                          <string>ca://$prefix:W0_FIT</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:W0_FIT</string>
                         </property>
                       </widget>
                     </item>
                     <item row="5" column="0">
@@ -580,15 +643,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>width</string>
+                          <string>ca://$prefix:WIDTH</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:WIDTH</string>
                         </property>
                       </widget>
                     </item>
                     <item row="6" column="0">
@@ -612,15 +675,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>amplitude</string>
+                          <string>ca://$prefix:AMPLITUDE</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:AMPLITUDE</string>
                         </property>
                       </widget>
                     </item>
                     <item row="7" column="0">
@@ -644,15 +707,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>fwhm</string>
+                          <string>ca://$prefix:FWHM</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:FWHM</string>
                         </property>
                       </widget>
                     </item>
                     <item row="8" column="0">
@@ -676,15 +739,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>stdev</string>
+                          <string>ca://$prefix:STDEV</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:STDEV</string>
                         </property>
                       </widget>
                     </item>
                     <item row="9" column="0">
@@ -708,15 +771,15 @@
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
                           <string/>
                         </property>
                         <property name="text">
-                          <string>chisq</string>
+                          <string>ca://$prefix:CHISQ</string>
                         </property>
                         <property name="channel" stdset="0">
                           <string>ca://$prefix:CHISQ</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
```

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/Setra5000.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/Setra5000.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/StatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/StatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-camera-summary.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-camera-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-config.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-overview.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-config.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-range-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-summary.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-range-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-dest.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-dest.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs-config.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-tabs-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-tabs.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-valves.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps-source-valves.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/btps.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/btps.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/ui/detailed_tree.ui` & `pcdsdevices-7.4.1/pcdsdevices/ui/detailed_tree.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/usb_encoder.py` & `pcdsdevices-7.4.1/pcdsdevices/usb_encoder.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/utils.py` & `pcdsdevices-7.4.1/pcdsdevices/utils.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/valve.py` & `pcdsdevices-7.4.1/pcdsdevices/valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/variety.py` & `pcdsdevices-7.4.1/pcdsdevices/variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/version.py` & `pcdsdevices-7.4.1/pcdsdevices/version.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices/wfs.py` & `pcdsdevices-7.4.1/pcdsdevices/wfs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pcdsdevices.egg-info/PKG-INFO` & `pcdsdevices-7.4.1/pcdsdevices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 7.4.0
+Version: 7.4.1
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.0 Summary: Ophyd Device
+Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.1 Summary: Ophyd Device
 definitions for LCLS Beamline components Author: SLAC National Accelerator
 Laboratory License: Copyright (c) 2023, The Board of Trustees of the Leland
 Stanford Junior University, through SLAC National Accelerator Laboratory
 (subject to receipt of any required approvals from the U.S. Dept. of Energy).
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: (1) Redistributions of source code must retain the above copyright notice,
```

### Comparing `pcdsdevices-7.4.0/pcdsdevices.egg-info/SOURCES.txt` & `pcdsdevices-7.4.1/pcdsdevices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.0/pyproject.toml` & `pcdsdevices-7.4.1/pyproject.toml`

 * *Files identical despite different names*

