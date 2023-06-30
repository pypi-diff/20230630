# Comparing `tmp/napari-0.4.9rc2.tar.gz` & `tmp/napari-0.4.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/napari/napari/dist/tmpm0inza4g/napari-0.4.9rc2.tar", last modified: Wed Jun  9 04:20:57 2021, max compression
+gzip compressed data, was "/home/runner/work/napari/napari/dist/tmplopi93ob/napari-0.4.9rc3.tar", last modified: Thu Jun 10 21:36:23 2021, max compression
```

## Comparing `napari-0.4.9rc2.tar` & `napari-0.4.9rc3.tar`

### file list

```diff
@@ -1,782 +1,782 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (121)      731 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/ISSUE_TEMPLATE/task.md
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/auto_author_assign.yml
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/make_bundle.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/make_docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/make_release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/test_comprehensive.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/test_prereleases.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5948 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/test_pull_requests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/test_translations.yml
--rw-r--r--   0 runner    (1001) docker     (121)      599 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.github/workflows/test_typing.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      805 2021-06-09 04:20:26.000000 napari-0.4.9rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-06-09 04:20:26.000000 napari-0.4.9rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      646 2021-06-09 04:20:26.000000 napari-0.4.9rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      928 2021-06-09 04:20:26.000000 napari-0.4.9rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    11363 2021-06-09 04:20:57.000000 napari-0.4.9rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9829 2021-06-09 04:20:26.000000 napari-0.4.9rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-06-09 04:20:26.000000 napari-0.4.9rc2/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-06-09 04:20:26.000000 napari-0.4.9rc2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-06-09 04:20:26.000000 napari-0.4.9rc2/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      766 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    13446 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_plugin_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     5004 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_qt_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_qt_public_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_qt_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13830 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_qt_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_qt_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     7720 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/_tests/test_threading_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/containers/
--rw-r--r--   0 runner    (1001) docker     (121)      471 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_base_item_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_base_item_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     7227 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_layer_delegate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/containers/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      699 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_tests/test_qt_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4792 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/_tests/test_qt_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_layer_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_layer_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_list_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_list_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     8432 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2316 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/containers/qt_tree_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/dialogs/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/dialogs/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/_tests/test_preferences_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/_tests/test_qt_about_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/_tests/test_qt_plugin_report.py
--rw-r--r--   0 runner    (1001) docker     (121)    15305 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/preferences_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_about.py
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_about_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_modal.py
--rw-r--r--   0 runner    (1001) docker     (121)    14412 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)    18965 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_plugin_dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/qt_plugin_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/dialogs/screenshot_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/experimental/qt_chunk_receiver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4468 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/experimental/qt_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/layer_controls/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_image_base_layer_.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_image_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_labels_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_shapes_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_tracks_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_colormap_combobox.py
--rw-r--r--   0 runner    (1001) docker     (121)    11578 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_image_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_image_controls_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    20276 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_labels_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4079 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_layer_controls_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_layer_controls_container.py
--rw-r--r--   0 runner    (1001) docker     (121)    13381 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_points_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)    17807 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_shapes_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_surface_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)     8034 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_tracks_controls.py
--rw-r--r--   0 runner    (1001) docker     (121)    11226 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/layer_controls/qt_vectors_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/perf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/perf/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/_tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/qt_debug_menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     4371 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/qt_event_tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5929 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/perf/qt_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qprogress.py
--rw-r--r--   0 runner    (1001) docker     (121)    13072 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)    54429 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/qt_resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14188 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/_icons.py
--rw-r--r--   0 runner    (1001) docker     (121)     4942 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/qt_resources/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/_tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/_tests/test_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/qt_resources/styles/
--rw-r--r--   0 runner    (1001) docker     (121)    13371 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/styles/00_base.qss
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/styles/01_buttons.qss
--rw-r--r--   0 runner    (1001) docker     (121)    12856 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_resources/styles/02_custom.qss
--rw-r--r--   0 runner    (1001) docker     (121)    35932 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qt_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)    32415 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/qthreading.py
--rw-r--r--   0 runner    (1001) docker     (121)     9734 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_dims.py
--rw-r--r--   0 runner    (1001) docker     (121)     4855 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_highlight_preview.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_large_int_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     5442 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_play.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_range_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_range_slider_popup.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_scrollbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     4801 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_size_preview.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/_tests/test_theme_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_activity_dock.py
--rw-r--r--   0 runner    (1001) docker     (121)    10020 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_color_swatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5197 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_dict_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    13458 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_dims.py
--rw-r--r--   0 runner    (1001) docker     (121)    26923 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_dims_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_eliding_label.py
--rw-r--r--   0 runner    (1001) docker     (121)    15831 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_highlight_preview.py
--rw-r--r--   0 runner    (1001) docker     (121)     5453 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_large_int_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_mode_buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)    14946 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_plugin_sorter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)    17007 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_range_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)    10013 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_range_slider_popup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_scrollbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_size_preview.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_splash_screen.py
--rw-r--r--   0 runner    (1001) docker     (121)     5173 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_theme_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_viewer_buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)    10668 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_viewer_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_qt/widgets/qt_welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_adding_removing.py
--rw-r--r--   0 runner    (1001) docker     (121)     8414 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)      959 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_function_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_import_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_notebook_display.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_numpy_like.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5433 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_view_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17070 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/test_with_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6056 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2829 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/lfu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/lru.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/rr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5830 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/ttl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     5580 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    18147 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     5862 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/filesize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5099 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4959 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5020 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4487 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     6058 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5295 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5589 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4524 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po
--rw-r--r--   0 runner    (1001) docker     (121)     7136 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/number.py
--rw-r--r--   0 runner    (1001) docker     (121)    15811 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/time.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/experimental/vendor.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/form.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/signal.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21476 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-09 04:20:56.000000 napari-0.4.9rc2/napari/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_image_rendering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_big_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4281 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_calls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_multiscale.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_points_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_scale_bar_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_text_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/_vispy_tracks_shader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/experimental/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     9289 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/_tests/test_vispy_tiled_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    11904 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/texture_atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/tile_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/tile_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    15066 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/tiled_image_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/experimental/vispy_tiled_image_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/image.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/markers.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/utils_gl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/vendored/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/_vispy/vendored/filters/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/filters/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    10630 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/filters/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    18878 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    11325 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    28584 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vendored/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_axes_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     5911 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_base_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6172 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_image_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_points_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9332 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_scale_bar_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_shapes_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_surface_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_text_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_tracks_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/vispy_vectors_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/_vispy/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/
--rw-r--r--   0 runner    (1001) docker     (121)      864 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_add_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5551 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_dims.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    16319 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_layers_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     7931 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_multichannel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_prune_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_scale_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     5296 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_viewer_image_io.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_viewer_labels_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    22806 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_viewer_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_viewer_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_tests/test_world_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_viewer_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_viewer_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/_viewer_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)    12343 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/dims.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/chunk/
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10249 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5010 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7353 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_delay_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     5903 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12149 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7014 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_pool_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     7384 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/chunk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/monitor/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7311 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/monitor/_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6675 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/monitor/_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/monitor/_service.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/monitor/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/components/experimental/remote/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/remote/_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/remote/_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/experimental/remote/_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    11850 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/layerlist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/scale_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (121)    45931 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/components/viewer_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9781 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8649 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/test_dask_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/test_layer_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/base/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/base/_base_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    40393 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/base/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/image/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4146 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_slice_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_image_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/image/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_big_image_timing.py
--rw-r--r--   0 runner    (1001) docker     (121)    18898 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_image_slice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13319 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_multiscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     5018 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/_tests/test_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/image/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_chunk_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_chunked_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_chunked_slice_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_image_location.py
--rw-r--r--   0 runner    (1001) docker     (121)    18308 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_octree_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7887 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_octree_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/image/experimental/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_tests/test_octree_import.py
--rw-r--r--   0 runner    (1001) docker     (121)      717 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/_tests/test_octree_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    14176 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)    17238 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     8144 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_intersection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_tile_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6021 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/experimental/octree_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    29227 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/image/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/intensity_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/labels/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_labels_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_labels_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_labels_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_labels_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/labels/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    28236 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)     9587 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    45909 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/labels/labels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/points/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2483 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_points_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_points_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_points_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_points_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/points/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    52030 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_tests/test_points_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    11026 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/_tests/test_points_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    59154 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/points/points.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/shapes/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    33618 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shape_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_key_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/_polgyon_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/_tests/test_shapes_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/line.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/path.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)    14757 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_models/shape.py
--rw-r--r--   0 runner    (1001) docker     (121)    18382 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    34298 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_shapes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/test_shape_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    65676 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    18137 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    99277 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/shapes/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/surface/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/surface/_surface_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/surface/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6886 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/surface/_tests/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (121)    14504 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/surface/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/tracks/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/tracks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/tracks/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5372 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/tracks/_tests/test_tracks.py
--rw-r--r--   0 runner    (1001) docker     (121)    14755 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/tracks/_track_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19066 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/tracks/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_color_manager_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7745 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_link_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/utils/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    22207 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_color_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_color_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_color_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_link_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8288 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_stack_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     7746 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_tests/test_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_text_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22140 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/color_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/color_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5100 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/color_transformations.py
--rw-r--r--   0 runner    (1001) docker     (121)     9746 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/stack_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12783 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/vectors/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/layers/vectors/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)    18537 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/vectors/_tests/test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4922 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/vectors/_vector_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    26503 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/layers/vectors/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11611 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    18052 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_skimage_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/plugins/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_builtin_get_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_builtin_write_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_hook_specifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_plugin_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_plugins_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_reader_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/_tests/test_save_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    19210 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/hook_specifications.py
--rw-r--r--   0 runner    (1001) docker     (121)    14824 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/plugins/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/qt/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/qt/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/qt/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/2D.svg
--rw-r--r--   0 runner    (1001) docker     (121)      923 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/3D.svg
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/add.svg
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/check.svg
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/chevron_down.svg
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/chevron_left.svg
--rw-r--r--   0 runner    (1001) docker     (121)      682 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/chevron_up.svg
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/circle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/console.svg
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/copy_to_clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/delete.svg
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/delete_shape.svg
--rw-r--r--   0 runner    (1001) docker     (121)      753 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/direct.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/down_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/drop_down.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/erase.svg
--rw-r--r--   0 runner    (1001) docker     (121)      653 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/fill.svg
--rw-r--r--   0 runner    (1001) docker     (121)      817 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/grid.svg
--rw-r--r--   0 runner    (1001) docker     (121)      740 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/info.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/left_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/line.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/logo_silhouette.svg
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/long_left_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/long_right_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/minus.svg
--rw-r--r--   0 runner    (1001) docker     (121)      800 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/move_back.svg
--rw-r--r--   0 runner    (1001) docker     (121)      759 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/move_front.svg
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_image.svg
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_labels.svg
--rw-r--r--   0 runner    (1001) docker     (121)      582 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_points.svg
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_shapes.svg
--rw-r--r--   0 runner    (1001) docker     (121)      475 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_surface.svg
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_tracks.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/new_vectors.svg
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/paint.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/path.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/picker.svg
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/plus.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/polygon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/pop_out.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/rectangle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/right_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/roll.svg
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/select.svg
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/shuffle.svg
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/square.svg
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/step_left.svg
--rw-r--r--   0 runner    (1001) docker     (121)      452 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/step_right.svg
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/transpose.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/up_arrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/vertex_insert.svg
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/vertex_remove.svg
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/visibility.svg
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/visibility_off.svg
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/warning.svg
--rw-r--r--   0 runner    (1001) docker     (121)      731 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/icons/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (121)   361616 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/loading.gif
--rw-r--r--   0 runner    (1001) docker     (121)   178219 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2160 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_appdirs.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)    11887 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_magicgui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_octree.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_register.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9900 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     8475 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5638 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_magicgui.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_theme.py
--rw-r--r--   0 runner    (1001) docker     (121)    15028 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_translations.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     5705 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_testsupport.py
--rw-r--r--   0 runner    (1001) docker     (121)     6570 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/_units.py
--rw-r--r--   0 runner    (1001) docker     (121)    14457 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/action_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/colormaps/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/colors_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/test_categorical_colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/test_categorical_colormap_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/test_color_to_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/test_colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/_tests/test_colormaps.py
--rw-r--r--   0 runner    (1001) docker     (121)    51895 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/bop_colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/categorical_colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/categorical_colormap_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/colorbars.py
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)    21320 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/colormap_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16139 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/standardize_color.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66616 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/_cm.py
--rw-r--r--   0 runner    (1001) docker     (121)    90444 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/_cm_listed.py
--rw-r--r--   0 runner    (1001) docker     (121)    35000 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/_color_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    12440 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/cm.py
--rw-r--r--   0 runner    (1001) docker     (121)    29428 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/colorconv.py
--rw-r--r--   0 runner    (1001) docker     (121)    67470 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/colormaps/vendored/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6459 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/dask_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/events/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/events/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)    15869 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_evented_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     8166 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_evented_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_evented_set.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/_tests/test_typed_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/events/containers/
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13767 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_evented_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    16432 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_selectable_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6440 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     8203 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/containers/_typed.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    36351 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8889 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/evented_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/events/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     9334 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16432 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    14414 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    14176 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/notebook_display.py
--rw-r--r--   0 runner    (1001) docker     (121)     9268 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/perf/
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     6723 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_patcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_stat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6987 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_timers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/perf/_trace_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/settings/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18119 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/settings/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     7832 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/settings/_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/settings/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6071 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/settings/_tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/status_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/stubgen.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/temporary_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/transforms/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/_tests/test_transform_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/_tests/test_transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9641 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/_tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     9132 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17813 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/transforms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    20062 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/translations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/tree/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari/utils/tree/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/tree/_tests/test_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/tree/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/tree/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4981 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/view_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-06-09 04:20:26.000000 napari-0.4.9rc2/napari/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11363 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    26293 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 04:20:40.000000 napari-0.4.9rc2/napari.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-09 04:20:57.000000 napari-0.4.9rc2/napari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-06-09 04:20:26.000000 napari-0.4.9rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2021-06-09 04:20:57.000000 napari-0.4.9rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-06-09 04:20:26.000000 napari-0.4.9rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2021-06-09 04:20:26.000000 napari-0.4.9rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/ISSUE_TEMPLATE/task.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/auto_author_assign.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/make_bundle.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3677 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/make_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/make_release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6549 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/test_comprehensive.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/test_prereleases.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5948 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/test_pull_requests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/test_translations.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.github/workflows/test_typing.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1721 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2021-06-10 21:35:58.000000 napari-0.4.9rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-06-10 21:35:58.000000 napari-0.4.9rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2021-06-10 21:35:58.000000 napari-0.4.9rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2021-06-10 21:35:58.000000 napari-0.4.9rc3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    11363 2021-06-10 21:36:23.000000 napari-0.4.9rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9829 2021-06-10 21:35:58.000000 napari-0.4.9rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1808 2021-06-10 21:35:58.000000 napari-0.4.9rc3/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2021-06-10 21:35:58.000000 napari-0.4.9rc3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-06-10 21:35:58.000000 napari-0.4.9rc3/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    13446 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6686 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_plugin_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5004 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_qt_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_qt_public_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_qt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13830 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_qt_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_qt_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7720 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2882 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/_tests/test_threading_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/containers/
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_base_item_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5028 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_base_item_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7227 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_layer_delegate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/containers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3620 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_tests/test_qt_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4792 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/_tests/test_qt_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_layer_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2557 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_layer_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3198 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_list_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8432 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2316 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/containers/qt_tree_view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/dialogs/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/_tests/test_preferences_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/_tests/test_qt_about_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/_tests/test_qt_plugin_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15305 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/preferences_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4467 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_about.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5303 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_about_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_modal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14412 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18965 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_plugin_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7486 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/qt_plugin_report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/dialogs/screenshot_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/experimental/qt_chunk_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4468 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/experimental/qt_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/layer_controls/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4046 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_image_base_layer_.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_image_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_labels_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_shapes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_tracks_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_colormap_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11578 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_image_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11062 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_image_controls_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20276 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_labels_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4079 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_layer_controls_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4184 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_layer_controls_container.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13381 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_points_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17807 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_shapes_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_surface_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8034 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_tracks_controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11226 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/layer_controls/qt_vectors_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/perf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/perf/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2660 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/_tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/qt_debug_menu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4371 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/qt_event_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5929 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/perf/qt_performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4235 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qprogress.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13072 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54429 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/qt_resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14188 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/_icons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4942 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/qt_resources/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/_tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/_tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/qt_resources/styles/
+-rw-r--r--   0 runner    (1001) docker     (121)    13371 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/styles/00_base.qss
+-rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/styles/01_buttons.qss
+-rw-r--r--   0 runner    (1001) docker     (121)    12856 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_resources/styles/02_custom.qss
+-rw-r--r--   0 runner    (1001) docker     (121)    35876 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qt_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32415 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/qthreading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9734 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9392 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_dims.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4855 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6041 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_highlight_preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_large_int_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5442 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_play.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3621 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_range_slider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_range_slider_popup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_scrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4801 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_size_preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/_tests/test_theme_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_activity_dock.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10020 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_color_swatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5197 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_dict_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13458 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_dims.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26923 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_dims_slider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_eliding_label.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15831 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_highlight_preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5453 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_large_int_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_mode_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14946 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_plugin_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17007 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_range_slider.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10013 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_range_slider_popup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_scrollbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10240 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_size_preview.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_splash_screen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5173 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_theme_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11152 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_viewer_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10668 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_viewer_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_qt/widgets/qt_welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4210 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_adding_removing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8414 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4571 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1928 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_function_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_notebook_display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_numpy_like.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5433 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_view_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8658 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17070 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/test_with_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6056 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2829 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/lfu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/lru.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/rr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5830 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/ttl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     5580 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18147 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)     5862 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/filesize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5099 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5028 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4959 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5122 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5348 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5020 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4487 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4873 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5285 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     6058 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5295 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4641 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5589 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4886 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/humanize.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     4524 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po
+-rw-r--r--   0 runner    (1001) docker     (121)     7136 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/number.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15811 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/experimental/vendor.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/form.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/signal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21476 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_image_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_big_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_calls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5269 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_multiscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_points_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_scale_bar_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_text_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4407 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/_vispy_tracks_shader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/experimental/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     9289 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/_tests/test_vispy_tiled_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11904 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/texture_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/tile_grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4162 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/tile_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15066 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/tiled_image_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11052 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/experimental/vispy_tiled_image_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/markers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/utils_gl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/vendored/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/_vispy/vendored/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/filters/base_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10630 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/filters/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18878 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11325 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28584 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vendored/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_axes_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5911 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6172 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7137 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_image_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6303 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_points_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9332 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_scale_bar_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_shapes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_surface_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_text_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_tracks_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/vispy_vectors_layer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/_vispy/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_add_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5551 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_dims.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16319 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_layers_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7931 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_multichannel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_prune_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_scale_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5296 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_viewer_image_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_viewer_labels_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22806 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_viewer_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_viewer_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3489 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_tests/test_world_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_viewer_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3082 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_viewer_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/_viewer_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/axes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12343 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/dims.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/chunk/
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3921 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10249 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5010 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7353 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_delay_queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5903 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12149 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7014 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4696 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_pool_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7384 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/chunk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/monitor/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7311 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/monitor/_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6675 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/monitor/_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5287 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/monitor/_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/monitor/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/components/experimental/remote/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2547 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/remote/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/remote/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1826 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/experimental/remote/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11850 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/layerlist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/scale_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45931 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/components/viewer_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9781 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3031 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8649 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/test_dask_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1817 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/test_layer_save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2214 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/base/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/base/_base_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40393 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/base/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/image/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2440 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4146 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_slice_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3098 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_image_view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/image/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_big_image_timing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18898 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_image_slice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13319 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_multiscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5018 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/_tests/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/image/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_chunk_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_chunked_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_chunked_slice_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_image_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18308 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_octree_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7887 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_octree_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/image/experimental/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_tests/test_octree_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/_tests/test_octree_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14176 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5182 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17238 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8144 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6915 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_level.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3184 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_tile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6021 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/experimental/octree_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29227 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4217 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/intensity_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/labels/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2451 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_labels_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2881 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_labels_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_labels_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3593 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_labels_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/labels/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    29378 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9587 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45940 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/labels/labels.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/points/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2483 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_points_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_points_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4105 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_points_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_points_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/points/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    52030 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_tests/test_points_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11026 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/_tests/test_points_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59154 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/points/points.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/shapes/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3099 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33618 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shape_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_key_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/_polgyon_base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     4433 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/_tests/test_shapes_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3554 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14757 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_models/shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18382 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34298 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_shapes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/test_shape_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65676 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3569 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18137 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    99277 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/shapes/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/surface/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/surface/_surface_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/surface/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     6886 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/surface/_tests/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14504 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/surface/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/tracks/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/tracks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/tracks/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     5372 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/tracks/_tests/test_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14755 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/tracks/_track_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19066 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/tracks/tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_color_manager_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7745 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_link_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/utils/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    22207 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_color_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_color_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_link_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8288 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_stack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5447 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7746 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_tests/test_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_text_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22140 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/color_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4771 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/color_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5100 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/color_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9746 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/stack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12783 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/vectors/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/layers/vectors/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)    18537 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/vectors/_tests/test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4922 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/vectors/_vector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26503 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/layers/vectors/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11611 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18052 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_skimage_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/plugins/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_builtin_get_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_builtin_write_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3188 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_hook_specifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_plugin_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2716 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_plugins_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_reader_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2571 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/_tests/test_save_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19210 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/hook_specifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14824 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/plugins/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/qt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/qt/progress.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/qt/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/2D.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/3D.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/add.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/check.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/chevron_left.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/console.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/copy_to_clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/delete_shape.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/direct.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/down_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/drop_down.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/erase.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/fill.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/grid.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/info.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/left_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/line.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/logo_silhouette.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/long_left_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/long_right_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/move_back.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/move_front.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_image.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_labels.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_points.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_shapes.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_surface.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_tracks.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/new_vectors.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/paint.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/path.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/picker.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/polygon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/pop_out.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/rectangle.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/right_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/roll.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/select.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/shuffle.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/square.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/step_left.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/step_right.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/transpose.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/up_arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/vertex_insert.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/vertex_remove.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/visibility.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/visibility_off.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/warning.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/icons/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   361616 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (121)   178219 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2160 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11887 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_magicgui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2598 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_octree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2542 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_register.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9900 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8475 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5638 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_magicgui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4884 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4677 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15028 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_translations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5705 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_testsupport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6570 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/_units.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15280 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/action_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3315 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/colors_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4990 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/test_categorical_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/test_categorical_colormap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/test_color_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/test_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5806 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/_tests/test_colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51895 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/bop_colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/categorical_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2788 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/categorical_colormap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/colorbars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3448 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21320 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/colormap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16139 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/standardize_color.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66616 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/_cm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    90444 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/_cm_listed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35000 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/_color_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12440 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/cm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29428 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/colorconv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67470 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/colormaps/vendored/colors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/dask_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/events/
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/events/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15869 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_evented_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8166 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_evented_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3204 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_evented_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/_tests/test_typed_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/events/containers/
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13767 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_evented_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16432 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3713 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_selectable_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_selection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6440 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8203 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/containers/_typed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36351 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8889 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/evented_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9334 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16432 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14414 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14176 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2314 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/notebook_display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9268 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/perf/
+-rw-r--r--   0 runner    (1001) docker     (121)     2071 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4844 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6723 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_stat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6987 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_timers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/perf/_trace_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18119 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/settings/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7832 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/settings/_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/settings/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     6071 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/settings/_tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/status_messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/temporary_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/transforms/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3405 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/_tests/test_transform_chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/_tests/test_transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9641 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/_tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9132 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17813 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/transforms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20062 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/translations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/tree/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari/utils/tree/_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/tree/_tests/test_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3103 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/tree/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4981 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/view_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4197 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2021-06-10 21:35:58.000000 napari-0.4.9rc3/napari/window.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11363 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    26293 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-10 21:36:08.000000 napari-0.4.9rc3/napari.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-10 21:36:23.000000 napari-0.4.9rc3/napari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2690 2021-06-10 21:35:58.000000 napari-0.4.9rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-06-10 21:36:23.000000 napari-0.4.9rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2021-06-10 21:35:58.000000 napari-0.4.9rc3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2021-06-10 21:35:58.000000 napari-0.4.9rc3/tox.ini
```

### Comparing `napari-0.4.9rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `napari-0.4.9rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `napari-0.4.9rc3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/PULL_REQUEST_TEMPLATE.md` & `napari-0.4.9rc3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/make_bundle.yml` & `napari-0.4.9rc3/.github/workflows/make_bundle.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/make_docs.yml` & `napari-0.4.9rc3/.github/workflows/make_docs.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/make_release.yml` & `napari-0.4.9rc3/.github/workflows/make_release.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/test_comprehensive.yml` & `napari-0.4.9rc3/.github/workflows/test_comprehensive.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/test_prereleases.yml` & `napari-0.4.9rc3/.github/workflows/test_prereleases.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/test_pull_requests.yml` & `napari-0.4.9rc3/.github/workflows/test_pull_requests.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/test_translations.yml` & `napari-0.4.9rc3/.github/workflows/test_translations.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.github/workflows/test_typing.yml` & `napari-0.4.9rc3/.github/workflows/test_typing.yml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.gitignore` & `napari-0.4.9rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/.pre-commit-config.yaml` & `napari-0.4.9rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/LICENSE` & `napari-0.4.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/MANIFEST.in` & `napari-0.4.9rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/Makefile` & `napari-0.4.9rc3/Makefile`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/PKG-INFO` & `napari-0.4.9rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari
-Version: 0.4.9rc2
+Version: 0.4.9rc3
 Summary: n-dimensional array viewer in Python
 Home-page: https://napari.org
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD 3-Clause
 Download-URL: https://github.com/napari/napari
 Platform: UNKNOWN
```

### Comparing `napari-0.4.9rc2/README.md` & `napari-0.4.9rc3/README.md`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/asv.conf.json` & `napari-0.4.9rc3/asv.conf.json`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/__init__.py` & `napari-0.4.9rc3/napari/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/__init__.pyi` & `napari-0.4.9rc3/napari/__init__.pyi`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/__main__.py` & `napari-0.4.9rc3/napari/__main__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_lazy.py` & `napari-0.4.9rc3/napari/_lazy.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/__init__.py` & `napari-0.4.9rc3/napari/_qt/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_constants.py` & `napari-0.4.9rc3/napari/_qt/_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_app.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_app.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_plugin_widgets.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_plugin_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_progress.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_qt_notifications.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_qt_notifications.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_qt_utils.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_qt_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_qt_viewer.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_qt_viewer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_qt_window.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_qt_window.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_threading.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/_tests/test_threading_progress.py` & `napari-0.4.9rc3/napari/_qt/_tests/test_threading_progress.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_base_item_model.py` & `napari-0.4.9rc3/napari/_qt/containers/_base_item_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_base_item_view.py` & `napari-0.4.9rc3/napari/_qt/containers/_base_item_view.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_factory.py` & `napari-0.4.9rc3/napari/_qt/containers/_factory.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_layer_delegate.py` & `napari-0.4.9rc3/napari/_qt/containers/_layer_delegate.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_tests/test_factory.py` & `napari-0.4.9rc3/napari/_qt/containers/_tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_tests/test_qt_list.py` & `napari-0.4.9rc3/napari/_qt/containers/_tests/test_qt_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/_tests/test_qt_tree.py` & `napari-0.4.9rc3/napari/_qt/containers/_tests/test_qt_tree.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_layer_list.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_layer_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_layer_model.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_layer_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_list_model.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_list_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_list_view.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_list_view.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_tree_model.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_tree_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/containers/qt_tree_view.py` & `napari-0.4.9rc3/napari/_qt/containers/qt_tree_view.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/_tests/test_qt_about_key_bindings.py` & `napari-0.4.9rc3/napari/_qt/dialogs/_tests/test_qt_about_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/_tests/test_qt_plugin_report.py` & `napari-0.4.9rc3/napari/_qt/dialogs/_tests/test_qt_plugin_report.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/preferences_dialog.py` & `napari-0.4.9rc3/napari/_qt/dialogs/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_about.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_about.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_about_key_bindings.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_about_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_modal.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_modal.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_notification.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_notification.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_plugin_dialog.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_plugin_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/qt_plugin_report.py` & `napari-0.4.9rc3/napari/_qt/dialogs/qt_plugin_report.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/dialogs/screenshot_dialog.py` & `napari-0.4.9rc3/napari/_qt/dialogs/screenshot_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/experimental/qt_chunk_receiver.py` & `napari-0.4.9rc3/napari/_qt/experimental/qt_chunk_receiver.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/experimental/qt_poll.py` & `napari-0.4.9rc3/napari/_qt/experimental/qt_poll.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_image_base_layer_.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_image_base_layer_.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_image_layer.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_image_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_labels_layer.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_labels_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_shapes_layer.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_shapes_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/_tests/test_qt_tracks_layer.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/_tests/test_qt_tracks_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_colormap_combobox.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_colormap_combobox.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_image_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_image_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_image_controls_base.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_image_controls_base.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_labels_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_labels_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_layer_controls_base.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_layer_controls_base.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_layer_controls_container.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_layer_controls_container.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_points_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_points_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_shapes_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_shapes_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_surface_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_surface_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_tracks_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_tracks_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/layer_controls/qt_vectors_controls.py` & `napari-0.4.9rc3/napari/_qt/layer_controls/qt_vectors_controls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/perf/_tests/test_perf.py` & `napari-0.4.9rc3/napari/_qt/perf/_tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/perf/qt_debug_menu.py` & `napari-0.4.9rc3/napari/_qt/perf/qt_debug_menu.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/perf/qt_event_tracing.py` & `napari-0.4.9rc3/napari/_qt/perf/qt_event_tracing.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/perf/qt_performance.py` & `napari-0.4.9rc3/napari/_qt/perf/qt_performance.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qprogress.py` & `napari-0.4.9rc3/napari/_qt/qprogress.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_event_loop.py` & `napari-0.4.9rc3/napari/_qt/qt_event_loop.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_main_window.py` & `napari-0.4.9rc3/napari/_qt/qt_main_window.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/__init__.py` & `napari-0.4.9rc3/napari/_qt/qt_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/_icons.py` & `napari-0.4.9rc3/napari/_qt/qt_resources/_icons.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/_svg.py` & `napari-0.4.9rc3/napari/_qt/qt_resources/_svg.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/_tests/test_svg.py` & `napari-0.4.9rc3/napari/_qt/qt_resources/_tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/styles/00_base.qss` & `napari-0.4.9rc3/napari/_qt/qt_resources/styles/00_base.qss`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/styles/01_buttons.qss` & `napari-0.4.9rc3/napari/_qt/qt_resources/styles/01_buttons.qss`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_resources/styles/02_custom.qss` & `napari-0.4.9rc3/napari/_qt/qt_resources/styles/02_custom.qss`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/qt_viewer.py` & `napari-0.4.9rc3/napari/_qt/qt_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,16 +270,15 @@
         # bind shortcuts stored in SETTINGS last.
         self._bind_shortcuts()
 
     def _bind_shortcuts(self):
         """Bind shortcuts stored in SETTINGS to actions."""
 
         for action, shortcuts in SETTINGS.shortcuts.shortcuts.items():
-            if action in action_manager._shortcuts:
-                action_manager.unbind_shortcut(action)
+            action_manager.unbind_shortcut(action)
             for shortcut in shortcuts:
                 action_manager.bind_shortcut(action, shortcut)
 
     def _create_canvas(self) -> None:
         """Create the canvas and hook up events."""
         self.canvas = VispyCanvas(
             keys=None,
```

### Comparing `napari-0.4.9rc2/napari/_qt/qthreading.py` & `napari-0.4.9rc3/napari/_qt/qthreading.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/utils.py` & `napari-0.4.9rc3/napari/_qt/utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_buttons.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_buttons.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_dims.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_dims.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_dock_widget.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_highlight_preview.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_highlight_preview.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_large_int_spinbox.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_large_int_spinbox.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_play.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_play.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_range_slider.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_range_slider.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_range_slider_popup.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_range_slider_popup.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/_tests/test_qt_size_preview.py` & `napari-0.4.9rc3/napari/_qt/widgets/_tests/test_qt_size_preview.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_color_swatch.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_color_swatch.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_dict_table.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_dict_table.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_dims.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_dims.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_dims_slider.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_dims_slider.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_eliding_label.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_eliding_label.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_highlight_preview.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_highlight_preview.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_large_int_spinbox.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_large_int_spinbox.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_mode_buttons.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_mode_buttons.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_plugin_sorter.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_plugin_sorter.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_progress_bar.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_progress_bar.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_range_slider.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_range_slider.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_range_slider_popup.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_range_slider_popup.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_scrollbar.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_scrollbar.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_size_preview.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_size_preview.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_theme_sample.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_theme_sample.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_viewer_buttons.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_viewer_buttons.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_viewer_dock_widget.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_viewer_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_qt/widgets/qt_welcome.py` & `napari-0.4.9rc3/napari/_qt/widgets/qt_welcome.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_adding_removing.py` & `napari-0.4.9rc3/napari/_tests/test_adding_removing.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_advanced.py` & `napari-0.4.9rc3/napari/_tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_cli.py` & `napari-0.4.9rc3/napari/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_draw.py` & `napari-0.4.9rc3/napari/_tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_dtypes.py` & `napari-0.4.9rc3/napari/_tests/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_examples.py` & `napari-0.4.9rc3/napari/_tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_function_widgets.py` & `napari-0.4.9rc3/napari/_tests/test_function_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_import_time.py` & `napari-0.4.9rc3/napari/_tests/test_import_time.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_key_bindings.py` & `napari-0.4.9rc3/napari/_tests/test_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_mouse_bindings.py` & `napari-0.4.9rc3/napari/_tests/test_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_notebook_display.py` & `napari-0.4.9rc3/napari/_tests/test_notebook_display.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_numpy_like.py` & `napari-0.4.9rc3/napari/_tests/test_numpy_like.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_pytest_plugin.py` & `napari-0.4.9rc3/napari/_tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_view_layers.py` & `napari-0.4.9rc3/napari/_tests/test_view_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_viewer.py` & `napari-0.4.9rc3/napari/_tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/test_with_screenshot.py` & `napari-0.4.9rc3/napari/_tests/test_with_screenshot.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_tests/utils.py` & `napari-0.4.9rc3/napari/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/CHANGELOG.rst` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/LICENSE` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/abc.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/abc.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/cache.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/cache.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/decorators.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/decorators.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/func.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/func.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/keys.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/keys.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/lfu.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/lfu.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/lru.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/lru.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/rr.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/rr.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/cachetools/ttl.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/cachetools/ttl.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/Makefile` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/conf.py` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/cachetools/docs/index.rst` & `napari-0.4.9rc3/napari/_vendor/experimental/cachetools/docs/index.rst`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/LICENCE` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/LICENCE`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/README.md` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/README.md`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/__init__.py` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/filesize.py` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/filesize.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/i18n.py` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/i18n.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/vi_VI/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/number.py` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/number.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/experimental/humanize/src/humanize/time.py` & `napari-0.4.9rc3/napari/_vendor/experimental/humanize/src/humanize/time.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/LICENSE` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/defaults.py` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/defaults.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/form.py` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/form.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/signal.py` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/signal.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/utils.py` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vendor/qt_json_builder/qt_jsonschema_form/widgets.py` & `napari-0.4.9rc3/napari/_vendor/qt_json_builder/qt_jsonschema_form/widgets.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/__init__.py` & `napari-0.4.9rc3/napari/_vispy/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_image_rendering.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_image_rendering.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_utils.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_big_images.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_big_images.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_calls.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_calls.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_camera.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_camera.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_multiscale.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_multiscale.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_scale_bar_visual.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_scale_bar_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_tests/test_vispy_text_visual.py` & `napari-0.4.9rc3/napari/_vispy/_tests/test_vispy_text_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_text_utils.py` & `napari-0.4.9rc3/napari/_vispy/_text_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/_vispy_tracks_shader.py` & `napari-0.4.9rc3/napari/_vispy/_vispy_tracks_shader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/_tests/test_vispy_tiled_image.py` & `napari-0.4.9rc3/napari/_vispy/experimental/_tests/test_vispy_tiled_image.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/texture_atlas.py` & `napari-0.4.9rc3/napari/_vispy/experimental/texture_atlas.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/tile_grid.py` & `napari-0.4.9rc3/napari/_vispy/experimental/tile_grid.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/tile_set.py` & `napari-0.4.9rc3/napari/_vispy/experimental/tile_set.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/tiled_image_visual.py` & `napari-0.4.9rc3/napari/_vispy/experimental/tiled_image_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/experimental/vispy_tiled_image_layer.py` & `napari-0.4.9rc3/napari/_vispy/experimental/vispy_tiled_image_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/markers.py` & `napari-0.4.9rc3/napari/_vispy/markers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/quaternion.py` & `napari-0.4.9rc3/napari/_vispy/quaternion.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/utils.py` & `napari-0.4.9rc3/napari/_vispy/utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/utils_gl.py` & `napari-0.4.9rc3/napari/_vispy/utils_gl.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vendored/filters/base_filter.py` & `napari-0.4.9rc3/napari/_vispy/vendored/filters/base_filter.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vendored/filters/mesh.py` & `napari-0.4.9rc3/napari/_vispy/vendored/filters/mesh.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vendored/image.py` & `napari-0.4.9rc3/napari/_vispy/vendored/image.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vendored/mesh.py` & `napari-0.4.9rc3/napari/_vispy/vendored/mesh.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vendored/volume.py` & `napari-0.4.9rc3/napari/_vispy/vendored/volume.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_axes_visual.py` & `napari-0.4.9rc3/napari/_vispy/vispy_axes_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_base_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_base_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_camera.py` & `napari-0.4.9rc3/napari/_vispy/vispy_camera.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_canvas.py` & `napari-0.4.9rc3/napari/_vispy/vispy_canvas.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_image_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_image_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_points_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_points_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_scale_bar_visual.py` & `napari-0.4.9rc3/napari/_vispy/vispy_scale_bar_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_shapes_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_shapes_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_surface_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_surface_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_text_visual.py` & `napari-0.4.9rc3/napari/_vispy/vispy_text_visual.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_tracks_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_tracks_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/vispy_vectors_layer.py` & `napari-0.4.9rc3/napari/_vispy/vispy_vectors_layer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/_vispy/volume.py` & `napari-0.4.9rc3/napari/_vispy/volume.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/__init__.py` & `napari-0.4.9rc3/napari/components/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_add_layers.py` & `napari-0.4.9rc3/napari/components/_tests/test_add_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_dims.py` & `napari-0.4.9rc3/napari/components/_tests/test_dims.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_grid.py` & `napari-0.4.9rc3/napari/components/_tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_layers_list.py` & `napari-0.4.9rc3/napari/components/_tests/test_layers_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_multichannel.py` & `napari-0.4.9rc3/napari/components/_tests/test_multichannel.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_prune_kwargs.py` & `napari-0.4.9rc3/napari/components/_tests/test_prune_kwargs.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_viewer_image_io.py` & `napari-0.4.9rc3/napari/components/_tests/test_viewer_image_io.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_viewer_labels_io.py` & `napari-0.4.9rc3/napari/components/_tests/test_viewer_labels_io.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_viewer_model.py` & `napari-0.4.9rc3/napari/components/_tests/test_viewer_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_viewer_mouse_bindings.py` & `napari-0.4.9rc3/napari/components/_tests/test_viewer_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_tests/test_world_coordinates.py` & `napari-0.4.9rc3/napari/components/_tests/test_world_coordinates.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_viewer_constants.py` & `napari-0.4.9rc3/napari/components/_viewer_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_viewer_key_bindings.py` & `napari-0.4.9rc3/napari/components/_viewer_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/_viewer_mouse_bindings.py` & `napari-0.4.9rc3/napari/components/_viewer_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/axes.py` & `napari-0.4.9rc3/napari/components/axes.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/camera.py` & `napari-0.4.9rc3/napari/components/camera.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/cursor.py` & `napari-0.4.9rc3/napari/components/cursor.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/dims.py` & `napari-0.4.9rc3/napari/components/dims.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_cache.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_cache.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_loader.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tables.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tables.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_tests/test_loader.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_commands/_utils.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_commands/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_delay_queue.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_delay_queue.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_info.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_info.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_loader.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_pool.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_pool.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_pool_group.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_pool_group.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_request.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_request.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_tests/test_chunk.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_tests/test_loader.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/chunk/_utils.py` & `napari-0.4.9rc3/napari/components/experimental/chunk/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/commands.py` & `napari-0.4.9rc3/napari/components/experimental/commands.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/monitor/_api.py` & `napari-0.4.9rc3/napari/components/experimental/monitor/_api.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/monitor/_monitor.py` & `napari-0.4.9rc3/napari/components/experimental/monitor/_monitor.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/monitor/_service.py` & `napari-0.4.9rc3/napari/components/experimental/monitor/_service.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/monitor/_utils.py` & `napari-0.4.9rc3/napari/components/experimental/monitor/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/remote/_commands.py` & `napari-0.4.9rc3/napari/components/experimental/remote/_commands.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/remote/_manager.py` & `napari-0.4.9rc3/napari/components/experimental/remote/_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/experimental/remote/_messages.py` & `napari-0.4.9rc3/napari/components/experimental/remote/_messages.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/grid.py` & `napari-0.4.9rc3/napari/components/grid.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/layerlist.py` & `napari-0.4.9rc3/napari/components/layerlist.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/scale_bar.py` & `napari-0.4.9rc3/napari/components/scale_bar.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/text_overlay.py` & `napari-0.4.9rc3/napari/components/text_overlay.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/components/viewer_model.py` & `napari-0.4.9rc3/napari/components/viewer_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/conftest.py` & `napari-0.4.9rc3/napari/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/__init__.py` & `napari-0.4.9rc3/napari/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_source.py` & `napari-0.4.9rc3/napari/layers/_source.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_tests/test_dask_layers.py` & `napari-0.4.9rc3/napari/layers/_tests/test_dask_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_tests/test_layer_save.py` & `napari-0.4.9rc3/napari/layers/_tests/test_layer_save.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_tests/test_serialize.py` & `napari-0.4.9rc3/napari/layers/_tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_tests/test_source.py` & `napari-0.4.9rc3/napari/layers/_tests/test_source.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/_tests/test_utils.py` & `napari-0.4.9rc3/napari/layers/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/base/_base_constants.py` & `napari-0.4.9rc3/napari/layers/base/_base_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/base/base.py` & `napari-0.4.9rc3/napari/layers/base/base.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_constants.py` & `napari-0.4.9rc3/napari/layers/image/_image_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_loader.py` & `napari-0.4.9rc3/napari/layers/image/_image_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_slice.py` & `napari-0.4.9rc3/napari/layers/image/_image_slice.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_slice_data.py` & `napari-0.4.9rc3/napari/layers/image/_image_slice_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_utils.py` & `napari-0.4.9rc3/napari/layers/image/_image_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_image_view.py` & `napari-0.4.9rc3/napari/layers/image/_image_view.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_big_image_timing.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_big_image_timing.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_image.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_image_slice.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_image_slice.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_image_utils.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_multiscale.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_multiscale.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/_tests/test_volume.py` & `napari-0.4.9rc3/napari/layers/image/_tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_chunk_set.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_chunk_set.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_chunked_image_loader.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_chunked_image_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_chunked_slice_data.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_chunked_slice_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_image_location.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_image_location.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_octree_loader.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_octree_loader.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_octree_slice.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_octree_slice.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_tests/test_location.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_tests/test_location.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/_tests/test_octree_util.py` & `napari-0.4.9rc3/napari/layers/image/experimental/_tests/test_octree_util.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_chunk.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_chunk.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_image.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_image.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_intersection.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_intersection.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_level.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_level.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_tile_builder.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_tile_builder.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/experimental/octree_util.py` & `napari-0.4.9rc3/napari/layers/image/experimental/octree_util.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/image/image.py` & `napari-0.4.9rc3/napari/layers/image/image.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/intensity_mixin.py` & `napari-0.4.9rc3/napari/layers/intensity_mixin.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_labels_constants.py` & `napari-0.4.9rc3/napari/layers/labels/_labels_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_labels_key_bindings.py` & `napari-0.4.9rc3/napari/layers/labels/_labels_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_labels_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/labels/_labels_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_labels_utils.py` & `napari-0.4.9rc3/napari/layers/labels/_labels_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_tests/test_labels.py` & `napari-0.4.9rc3/napari/layers/labels/_tests/test_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import itertools
+from tempfile import TemporaryDirectory
 
 import numpy as np
 import pandas as pd
 import pytest
+import tensorstore as ts
 import xarray as xr
+import zarr
 from numpy.core.numerictypes import issubdtype
 from numpy.testing import assert_array_almost_equal, assert_raises
 from skimage import data
 
 from napari._tests.utils import check_layer_world_data_extent
 from napari.layers import Labels
 from napari.utils import Colormap
@@ -919,7 +922,39 @@
     label_array[0, :, :] = [[0, 1], [2, 3]]
     layer = Labels(label_array)
     assert len(layer._all_vals) == layer.num_colors
 
     layer.show_selected_label = True
     layer.selected_label = int(5e6)
     assert layer._all_vals.size < 1026
+
+
+def test_fill_tensorstore():
+    labels = np.zeros((5, 7, 8, 9), dtype=int)
+    labels[1, 2:4, 4:6, 4:6] = 1
+    labels[1, 3:5, 5:7, 6:8] = 2
+    labels[2, 3:5, 5:7, 6:8] = 3
+    with TemporaryDirectory(suffix='.zarr') as fout:
+        labels_temp = zarr.open(
+            fout,
+            mode='w',
+            shape=labels.shape,
+            dtype=np.uint32,
+            chunks=(1, 1, 8, 9),
+        )
+        labels_temp[:] = labels
+        labels_ts_spec = {
+            'driver': 'zarr',
+            'kvstore': {'driver': 'file', 'path': fout},
+            'path': '',
+            'metadata': {
+                'dtype': labels_temp.dtype.str,
+                'order': labels_temp.order,
+                'shape': labels.shape,
+            },
+        }
+        data = ts.open(labels_ts_spec, create=False, open=True).result()
+        layer = Labels(data)
+        layer.n_edit_dimensions = 3
+        layer.fill((1, 4, 6, 7), 4)
+        modified_labels = np.where(labels == 2, 4, labels)
+        np.testing.assert_array_equal(modified_labels, np.asarray(data))
```

### Comparing `napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_pyramid.py` & `napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_pyramid.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/_tests/test_labels_utils.py` & `napari-0.4.9rc3/napari/layers/labels/_tests/test_labels_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/labels/labels.py` & `napari-0.4.9rc3/napari/layers/labels/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1051,26 +1051,26 @@
         # If requested fill location is outside data shape then return
         if np.any(np.less(int_coord, 0)) or np.any(
             np.greater_equal(int_coord, self.data.shape)
         ):
             return
 
         # If requested new label doesn't change old label then return
-        old_label = self.data[int_coord]
+        old_label = np.asarray(self.data[int_coord]).item()
         if old_label == new_label or (
             self.preserve_labels and old_label != self._background_label
         ):
             return
 
         dims_to_fill = self._dims_order[-self.n_edit_dimensions :]
         data_slice_list = list(int_coord)
         for dim in dims_to_fill:
             data_slice_list[dim] = slice(None)
         data_slice = tuple(data_slice_list)
-        labels = self.data[data_slice]
+        labels = np.asarray(self.data[data_slice])
         slice_coord = tuple(int_coord[d] for d in dims_to_fill)
 
         matches = labels == old_label
         if self.contiguous:
             # if contiguous replace only selected connected component
             labeled_matches, num_features = ndi.label(matches)
             if num_features != 1:
```

### Comparing `napari-0.4.9rc2/napari/layers/points/_points_constants.py` & `napari-0.4.9rc3/napari/layers/points/_points_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/_points_key_bindings.py` & `napari-0.4.9rc3/napari/layers/points/_points_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/_points_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/points/_points_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/_points_utils.py` & `napari-0.4.9rc3/napari/layers/points/_points_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/_tests/test_points.py` & `napari-0.4.9rc3/napari/layers/points/_tests/test_points.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/_tests/test_points_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/points/_tests/test_points_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/points/points.py` & `napari-0.4.9rc3/napari/layers/points/points.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_mesh.py` & `napari-0.4.9rc3/napari/layers/shapes/_mesh.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shape_list.py` & `napari-0.4.9rc3/napari/layers/shapes/_shape_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_constants.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_key_bindings.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/_polgyon_base.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/_polgyon_base.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/_tests/test_shapes_models.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/_tests/test_shapes_models.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/ellipse.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/ellipse.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/line.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/line.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/path.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/path.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/polygon.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/polygon.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/rectangle.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/rectangle.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_models/shape.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_models/shape.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_shapes_utils.py` & `napari-0.4.9rc3/napari/layers/shapes/_shapes_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_tests/test_shape_list.py` & `napari-0.4.9rc3/napari/layers/shapes/_tests/test_shape_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes.py` & `napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_key_bindings.py` & `napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_mouse_bindings.py` & `napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/_tests/test_shapes_utils.py` & `napari-0.4.9rc3/napari/layers/shapes/_tests/test_shapes_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/shapes/shapes.py` & `napari-0.4.9rc3/napari/layers/shapes/shapes.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/surface/_surface_constants.py` & `napari-0.4.9rc3/napari/layers/surface/_surface_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/surface/_tests/test_surface.py` & `napari-0.4.9rc3/napari/layers/surface/_tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/surface/surface.py` & `napari-0.4.9rc3/napari/layers/surface/surface.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/tracks/_tests/test_tracks.py` & `napari-0.4.9rc3/napari/layers/tracks/_tests/test_tracks.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/tracks/_track_utils.py` & `napari-0.4.9rc3/napari/layers/tracks/_track_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/tracks/tracks.py` & `napari-0.4.9rc3/napari/layers/tracks/tracks.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_link_layers.py` & `napari-0.4.9rc3/napari/layers/utils/_link_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_color_manager.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_color_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_color_manager_utils.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_color_manager_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_color_transforms.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_color_transforms.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_layer_utils.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_layer_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_link_layers.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_link_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_stack_utils.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_stack_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_text.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_text.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_tests/test_text_utils.py` & `napari-0.4.9rc3/napari/layers/utils/_tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_text_constants.py` & `napari-0.4.9rc3/napari/layers/utils/_text_constants.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/_text_utils.py` & `napari-0.4.9rc3/napari/layers/utils/_text_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/color_manager.py` & `napari-0.4.9rc3/napari/layers/utils/color_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/color_manager_utils.py` & `napari-0.4.9rc3/napari/layers/utils/color_manager_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/color_transformations.py` & `napari-0.4.9rc3/napari/layers/utils/color_transformations.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/layer_utils.py` & `napari-0.4.9rc3/napari/layers/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/stack_utils.py` & `napari-0.4.9rc3/napari/layers/utils/stack_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/utils/text.py` & `napari-0.4.9rc3/napari/layers/utils/text.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/vectors/_tests/test_vectors.py` & `napari-0.4.9rc3/napari/layers/vectors/_tests/test_vectors.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/vectors/_vector_utils.py` & `napari-0.4.9rc3/napari/layers/vectors/_vector_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/layers/vectors/vectors.py` & `napari-0.4.9rc3/napari/layers/vectors/vectors.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_builtins.py` & `napari-0.4.9rc3/napari/plugins/_builtins.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_plugin_manager.py` & `napari-0.4.9rc3/napari/plugins/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_skimage_data.py` & `napari-0.4.9rc3/napari/plugins/_skimage_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_builtin_get_writer.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_builtin_get_writer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_builtin_write_layers.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_builtin_write_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_exceptions.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_hook_specifications.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_hook_specifications.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_plugin_widgets.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_plugin_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_plugins_misc.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_plugins_misc.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_pypi.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_pypi.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_reader_plugins.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_reader_plugins.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_sample_data.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/_tests/test_save_layers.py` & `napari-0.4.9rc3/napari/plugins/_tests/test_save_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/exceptions.py` & `napari-0.4.9rc3/napari/plugins/exceptions.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/hook_specifications.py` & `napari-0.4.9rc3/napari/plugins/hook_specifications.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/io.py` & `napari-0.4.9rc3/napari/plugins/io.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/plugins/pypi.py` & `napari-0.4.9rc3/napari/plugins/pypi.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/qt/__init__.py` & `napari-0.4.9rc3/napari/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/qt/threading.py` & `napari-0.4.9rc3/napari/qt/threading.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/__init__.py` & `napari-0.4.9rc3/napari/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/_icons.py` & `napari-0.4.9rc3/napari/resources/_icons.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/2D.svg` & `napari-0.4.9rc3/napari/resources/icons/2D.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/3D.svg` & `napari-0.4.9rc3/napari/resources/icons/3D.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/add.svg` & `napari-0.4.9rc3/napari/resources/icons/add.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/chevron_down.svg` & `napari-0.4.9rc3/napari/resources/icons/chevron_down.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/chevron_left.svg` & `napari-0.4.9rc3/napari/resources/icons/chevron_left.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/chevron_up.svg` & `napari-0.4.9rc3/napari/resources/icons/chevron_up.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/console.svg` & `napari-0.4.9rc3/napari/resources/icons/console.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/copy_to_clipboard.svg` & `napari-0.4.9rc3/napari/resources/icons/copy_to_clipboard.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/delete.svg` & `napari-0.4.9rc3/napari/resources/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/delete_shape.svg` & `napari-0.4.9rc3/napari/resources/icons/delete_shape.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/direct.svg` & `napari-0.4.9rc3/napari/resources/icons/direct.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/ellipse.svg` & `napari-0.4.9rc3/napari/resources/icons/ellipse.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/fill.svg` & `napari-0.4.9rc3/napari/resources/icons/fill.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/grid.svg` & `napari-0.4.9rc3/napari/resources/icons/grid.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/home.svg` & `napari-0.4.9rc3/napari/resources/icons/home.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/line.svg` & `napari-0.4.9rc3/napari/resources/icons/line.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/logo_silhouette.svg` & `napari-0.4.9rc3/napari/resources/icons/logo_silhouette.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/long_left_arrow.svg` & `napari-0.4.9rc3/napari/resources/icons/long_left_arrow.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/move_back.svg` & `napari-0.4.9rc3/napari/resources/icons/move_back.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/move_front.svg` & `napari-0.4.9rc3/napari/resources/icons/move_front.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/new_image.svg` & `napari-0.4.9rc3/napari/resources/icons/new_image.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/new_labels.svg` & `napari-0.4.9rc3/napari/resources/icons/new_labels.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/new_points.svg` & `napari-0.4.9rc3/napari/resources/icons/new_points.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/new_tracks.svg` & `napari-0.4.9rc3/napari/resources/icons/new_tracks.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/new_vectors.svg` & `napari-0.4.9rc3/napari/resources/icons/new_vectors.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/paint.svg` & `napari-0.4.9rc3/napari/resources/icons/paint.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/path.svg` & `napari-0.4.9rc3/napari/resources/icons/path.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/picker.svg` & `napari-0.4.9rc3/napari/resources/icons/picker.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/plus.svg` & `napari-0.4.9rc3/napari/resources/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/polygon.svg` & `napari-0.4.9rc3/napari/resources/icons/polygon.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/pop_out.svg` & `napari-0.4.9rc3/napari/resources/icons/pop_out.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/rectangle.svg` & `napari-0.4.9rc3/napari/resources/icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/roll.svg` & `napari-0.4.9rc3/napari/resources/icons/roll.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/select.svg` & `napari-0.4.9rc3/napari/resources/icons/select.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/shuffle.svg` & `napari-0.4.9rc3/napari/resources/icons/shuffle.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/step_left.svg` & `napari-0.4.9rc3/napari/resources/icons/step_left.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/transpose.svg` & `napari-0.4.9rc3/napari/resources/icons/transpose.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/vertex_insert.svg` & `napari-0.4.9rc3/napari/resources/icons/vertex_insert.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/vertex_remove.svg` & `napari-0.4.9rc3/napari/resources/icons/vertex_remove.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/visibility.svg` & `napari-0.4.9rc3/napari/resources/icons/visibility.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/visibility_off.svg` & `napari-0.4.9rc3/napari/resources/icons/visibility_off.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/warning.svg` & `napari-0.4.9rc3/napari/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/icons/zoom.svg` & `napari-0.4.9rc3/napari/resources/icons/zoom.svg`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/loading.gif` & `napari-0.4.9rc3/napari/resources/loading.gif`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/resources/logo.png` & `napari-0.4.9rc3/napari/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/types.py` & `napari-0.4.9rc3/napari/types.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_appdirs.py` & `napari-0.4.9rc3/napari/utils/_appdirs.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_dtype.py` & `napari-0.4.9rc3/napari/utils/_dtype.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_magicgui.py` & `napari-0.4.9rc3/napari/utils/_magicgui.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_octree.py` & `napari-0.4.9rc3/napari/utils/_octree.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_register.py` & `napari-0.4.9rc3/napari/utils/_register.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_dtype.py` & `napari-0.4.9rc3/napari/utils/_tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_info.py` & `napari-0.4.9rc3/napari/utils/_tests/test_info.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_interactions.py` & `napari-0.4.9rc3/napari/utils/_tests/test_interactions.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_io.py` & `napari-0.4.9rc3/napari/utils/_tests/test_io.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_key_bindings.py` & `napari-0.4.9rc3/napari/utils/_tests/test_key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_magicgui.py` & `napari-0.4.9rc3/napari/utils/_tests/test_magicgui.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_misc.py` & `napari-0.4.9rc3/napari/utils/_tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_naming.py` & `napari-0.4.9rc3/napari/utils/_tests/test_naming.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_notification_manager.py` & `napari-0.4.9rc3/napari/utils/_tests/test_notification_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_status.py` & `napari-0.4.9rc3/napari/utils/_tests/test_status.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_theme.py` & `napari-0.4.9rc3/napari/utils/_tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tests/test_translations.py` & `napari-0.4.9rc3/napari/utils/_tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_testsupport.py` & `napari-0.4.9rc3/napari/utils/_testsupport.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_tracebacks.py` & `napari-0.4.9rc3/napari/utils/_tracebacks.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/_units.py` & `napari-0.4.9rc3/napari/utils/_units.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/action_manager.py` & `napari-0.4.9rc3/napari/utils/action_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from inspect import signature
 from typing import TYPE_CHECKING, Callable, Dict, List, Set, Tuple, Union
 
 from .interactions import Shortcut
 from .key_bindings import KeymapProvider
@@ -352,27 +353,47 @@
         Parameters
         ----------
         name : str
             name of the action in the form `packagename:name` to unbind.
 
         Returns
         -------
-
         shortcut: str | None
-            previously bound shortcut.
+            Previously bound shortcut or None if not such shortcuts was bound,
+            or  no such action exists.
+
+        Warns
+        -----
+        UserWarning:
+            When trying to unbind an action unknown form the action manager,
+            this warning will be emitted.
+
         """
-        action = self._actions[name]
+        action = self._actions.get(name, None)
+        if action is None:
+            warnings.warn(
+                trans._(
+                    "Attempting to unbind an action which does not exists ({name}), "
+                    "this may have no effects. This can happen if your settings are out of "
+                    "date, if you upgraded napari, upgraded or deactivated a plugin, or made "
+                    "a typo in in your custom keybinding.",
+                    name=name,
+                ),
+                UserWarning,
+                stacklevel=2,
+            )
+
         shortcuts = self._shortcuts.get(name)
         if shortcuts:
-            if hasattr(action.keymapprovider, 'bind_key'):
+            if action and hasattr(action.keymapprovider, 'bind_key'):
                 for shortcut in shortcuts:
                     action.keymapprovider.bind_key(shortcut)(None)
             del self._shortcuts[name]
         self._update_gui_elements(name)
-        return shortcut
+        return shortcuts
 
     def _get_layer_shortcuts(self, layers):
         """
         Get shortcuts filterd by the given layers.
 
         Parameters
         ----------
```

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/colors_data.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/colors_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/test_categorical_colormap.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/test_categorical_colormap.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/test_categorical_colormap_utils.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/test_categorical_colormap_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/test_color_to_array.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/test_color_to_array.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/test_colormap.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/_tests/test_colormaps.py` & `napari-0.4.9rc3/napari/utils/colormaps/_tests/test_colormaps.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/bop_colors.py` & `napari-0.4.9rc3/napari/utils/colormaps/bop_colors.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/categorical_colormap.py` & `napari-0.4.9rc3/napari/utils/colormaps/categorical_colormap.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/categorical_colormap_utils.py` & `napari-0.4.9rc3/napari/utils/colormaps/categorical_colormap_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/colorbars.py` & `napari-0.4.9rc3/napari/utils/colormaps/colorbars.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/colormap.py` & `napari-0.4.9rc3/napari/utils/colormaps/colormap.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/colormap_utils.py` & `napari-0.4.9rc3/napari/utils/colormaps/colormap_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/standardize_color.py` & `napari-0.4.9rc3/napari/utils/colormaps/standardize_color.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/_cm.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/_cm.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/_cm_listed.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/_cm_listed.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/_color_data.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/_color_data.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/cm.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/cm.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/colorconv.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/colorconv.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/colormaps/vendored/colors.py` & `napari-0.4.9rc3/napari/utils/colormaps/vendored/colors.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/config.py` & `napari-0.4.9rc3/napari/utils/config.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/dask_utils.py` & `napari-0.4.9rc3/napari/utils/dask_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/__init__.py` & `napari-0.4.9rc3/napari/utils/events/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/_tests/test_evented_list.py` & `napari-0.4.9rc3/napari/utils/events/_tests/test_evented_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/_tests/test_evented_model.py` & `napari-0.4.9rc3/napari/utils/events/_tests/test_evented_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/_tests/test_evented_set.py` & `napari-0.4.9rc3/napari/utils/events/_tests/test_evented_set.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/_tests/test_selection.py` & `napari-0.4.9rc3/napari/utils/events/_tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/_tests/test_typed_list.py` & `napari-0.4.9rc3/napari/utils/events/_tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_evented_list.py` & `napari-0.4.9rc3/napari/utils/events/containers/_evented_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_nested_list.py` & `napari-0.4.9rc3/napari/utils/events/containers/_nested_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_selectable_list.py` & `napari-0.4.9rc3/napari/utils/events/containers/_selectable_list.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_selection.py` & `napari-0.4.9rc3/napari/utils/events/containers/_selection.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_set.py` & `napari-0.4.9rc3/napari/utils/events/containers/_set.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/containers/_typed.py` & `napari-0.4.9rc3/napari/utils/events/containers/_typed.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/custom_types.py` & `napari-0.4.9rc3/napari/utils/events/custom_types.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/event.py` & `napari-0.4.9rc3/napari/utils/events/event.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/event_utils.py` & `napari-0.4.9rc3/napari/utils/events/event_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/events/evented_model.py` & `napari-0.4.9rc3/napari/utils/events/evented_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/history.py` & `napari-0.4.9rc3/napari/utils/history.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/info.py` & `napari-0.4.9rc3/napari/utils/info.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/interactions.py` & `napari-0.4.9rc3/napari/utils/interactions.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/io.py` & `napari-0.4.9rc3/napari/utils/io.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/key_bindings.py` & `napari-0.4.9rc3/napari/utils/key_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/misc.py` & `napari-0.4.9rc3/napari/utils/misc.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/mouse_bindings.py` & `napari-0.4.9rc3/napari/utils/mouse_bindings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/naming.py` & `napari-0.4.9rc3/napari/utils/naming.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/notebook_display.py` & `napari-0.4.9rc3/napari/utils/notebook_display.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/notifications.py` & `napari-0.4.9rc3/napari/utils/notifications.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/__init__.py` & `napari-0.4.9rc3/napari/utils/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_config.py` & `napari-0.4.9rc3/napari/utils/perf/_config.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_event.py` & `napari-0.4.9rc3/napari/utils/perf/_event.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_patcher.py` & `napari-0.4.9rc3/napari/utils/perf/_patcher.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_stat.py` & `napari-0.4.9rc3/napari/utils/perf/_stat.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_timers.py` & `napari-0.4.9rc3/napari/utils/perf/_timers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/perf/_trace_file.py` & `napari-0.4.9rc3/napari/utils/perf/_trace_file.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/settings/_defaults.py` & `napari-0.4.9rc3/napari/utils/settings/_defaults.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/settings/_manager.py` & `napari-0.4.9rc3/napari/utils/settings/_manager.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/settings/_tests/test_settings.py` & `napari-0.4.9rc3/napari/utils/settings/_tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/shortcuts.py` & `napari-0.4.9rc3/napari/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/status_messages.py` & `napari-0.4.9rc3/napari/utils/status_messages.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/stubgen.py` & `napari-0.4.9rc3/napari/utils/stubgen.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/temporary_file.py` & `napari-0.4.9rc3/napari/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/theme.py` & `napari-0.4.9rc3/napari/utils/theme.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/transforms/_tests/test_transform_chain.py` & `napari-0.4.9rc3/napari/utils/transforms/_tests/test_transform_chain.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/transforms/_tests/test_transform_utils.py` & `napari-0.4.9rc3/napari/utils/transforms/_tests/test_transform_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/transforms/_tests/test_transforms.py` & `napari-0.4.9rc3/napari/utils/transforms/_tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/transforms/transform_utils.py` & `napari-0.4.9rc3/napari/utils/transforms/transform_utils.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/transforms/transforms.py` & `napari-0.4.9rc3/napari/utils/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/translations.py` & `napari-0.4.9rc3/napari/utils/translations.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/tree/_tests/test_tree_model.py` & `napari-0.4.9rc3/napari/utils/tree/_tests/test_tree_model.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/tree/group.py` & `napari-0.4.9rc3/napari/utils/tree/group.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/tree/node.py` & `napari-0.4.9rc3/napari/utils/tree/node.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/utils/validators.py` & `napari-0.4.9rc3/napari/utils/validators.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/view_layers.py` & `napari-0.4.9rc3/napari/view_layers.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/viewer.py` & `napari-0.4.9rc3/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari/window.py` & `napari-0.4.9rc3/napari/window.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 :class:`napari._qt.qt_main_window.Window` class.  In the future, this module
 could serve to define a window Protocol that a backend would need to implement
 to server as a graphical user interface for napari.
 """
 
 __all__ = ['Window']
 
+from .utils.translations import trans
+
 try:
     from ._qt import Window
-    from .utils.translations import trans
 
 except ImportError:
 
     class Window:  # type: ignore
         def __init__(self, *args, **kwargs):
             pass
```

### Comparing `napari-0.4.9rc2/napari.egg-info/PKG-INFO` & `napari-0.4.9rc3/napari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari
-Version: 0.4.9rc2
+Version: 0.4.9rc3
 Summary: n-dimensional array viewer in Python
 Home-page: https://napari.org
 Author: napari team
 Author-email: napari-steering-council@googlegroups.com
 License: BSD 3-Clause
 Download-URL: https://github.com/napari/napari
 Platform: UNKNOWN
```

### Comparing `napari-0.4.9rc2/napari.egg-info/SOURCES.txt` & `napari-0.4.9rc3/napari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/napari.egg-info/requires.txt` & `napari-0.4.9rc3/napari.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 pandas
 xarray
 fsspec
 zarr
 scikit-image>=0.18.1
 pooch>=1.3.0
 semgrep
-tensorstore>=0.1.10
+tensorstore!=0.1.11,>=0.1.10
 torch>=1.7
 
 [pyqt]
 PyQt5!=5.15.0,>=5.12.3
 
 [pyqt5]
 PyQt5!=5.15.0,>=5.12.3
@@ -86,9 +86,9 @@
 pandas
 xarray
 fsspec
 zarr
 scikit-image>=0.18.1
 pooch>=1.3.0
 semgrep
-tensorstore>=0.1.10
+tensorstore!=0.1.11,>=0.1.10
 torch>=1.7
```

### Comparing `napari-0.4.9rc2/pyproject.toml` & `napari-0.4.9rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-0.4.9rc2/setup.cfg` & `napari-0.4.9rc3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 	pandas
 	xarray
 	fsspec
 	zarr
 	scikit-image>=0.18.1
 	pooch>=1.3.0
 	semgrep
-	tensorstore>=0.1.10
+	tensorstore>=0.1.10,!=0.1.11
 	torch>=1.7
 release = 
 	PyGithub>=1.44.1
 	twine>=3.1.1
 	pygithub
 dev = 
 	pre-commit>=2.9.0
```

### Comparing `napari-0.4.9rc2/tox.ini` & `napari-0.4.9rc3/tox.ini`

 * *Files identical despite different names*

