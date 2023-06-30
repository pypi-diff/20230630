# Comparing `tmp/rummage-4.8.tar.gz` & `tmp/rummage-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rummage-4.8.tar", last modified: Sun Nov 17 15:38:17 2019, max compression
+gzip compressed data, was "dist/rummage-4.9.tar", last modified: Sun Jan 19 19:59:45 2020, max compression
```

## Comparing `rummage-4.8.tar` & `rummage-4.9.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/
--rw-r--r--   0 runner    (1001) docker     (115)      120 2019-11-17 15:38:08.000000 rummage-4.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (115)     1097 2019-11-17 15:38:08.000000 rummage-4.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (115)      523 2019-11-17 15:38:08.000000 rummage-4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)     4853 2019-11-17 15:38:17.000000 rummage-4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     3546 2019-11-17 15:38:08.000000 rummage-4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/internal_theme/
--rw-r--r--   0 runner    (1001) docker     (115)      130 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/404.html
--rw-r--r--   0 runner    (1001) docker     (115)     2192 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/internal_theme/css/
--rw-r--r--   0 runner    (1001) docker     (115)    29320 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/internal_theme/js/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (115)       26 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/main.html
--rw-r--r--   0 runner    (1001) docker     (115)      347 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/nav.html
--rw-r--r--   0 runner    (1001) docker     (115)      192 2019-11-17 15:38:08.000000 rummage-4.8/docs/internal_theme/sitemap.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/src/markdown/
--rw-r--r--   0 runner    (1001) docker     (115)    21882 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/changelog.md
--rw-r--r--   0 runner    (1001) docker     (115)     3847 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/contributing.md
--rw-r--r--   0 runner    (1001) docker     (115)     8740 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/extras.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/src/markdown/images/
--rw-r--r--   0 runner    (1001) docker     (115)    11948 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/chain_button.png
--rw-r--r--   0 runner    (1001) docker     (115)    59485 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/chain_mode.png
--rw-r--r--   0 runner    (1001) docker     (115)    48842 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/chains.png
--rw-r--r--   0 runner    (1001) docker     (115)   217500 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/content_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)    17769 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/file_pattern.png
--rw-r--r--   0 runner    (1001) docker     (115)   250916 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/files_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)   169845 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/html_export.png
--rw-r--r--   0 runner    (1001) docker     (115)    44736 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/limit_search_panel.png
--rw-r--r--   0 runner    (1001) docker     (115)    45680 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/load_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    26592 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/plugin_input.png
--rw-r--r--   0 runner    (1001) docker     (115)    13786 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/plugin_toggle.png
--rw-r--r--   0 runner    (1001) docker     (115)    13254 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/regex_buttons.png
--rw-r--r--   0 runner    (1001) docker     (115)    70694 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/regex_tester.png
--rw-r--r--   0 runner    (1001) docker     (115)    19024 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/rummage.png
--rw-r--r--   0 runner    (1001) docker     (115)    34022 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/save_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    21673 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/search_replace_inputs.png
--rw-r--r--   0 runner    (1001) docker     (115)    43205 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/search_replace_panel.png
--rw-r--r--   0 runner    (1001) docker     (115)   142134 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/search_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)    36090 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_backup.png
--rw-r--r--   0 runner    (1001) docker     (115)    63105 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_editor.png
--rw-r--r--   0 runner    (1001) docker     (115)    45332 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_encoding.png
--rw-r--r--   0 runner    (1001) docker     (115)    23171 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_export.png
--rw-r--r--   0 runner    (1001) docker     (115)    43099 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_general.png
--rw-r--r--   0 runner    (1001) docker     (115)    44211 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_history.png
--rw-r--r--   0 runner    (1001) docker     (115)    24429 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_import.png
--rw-r--r--   0 runner    (1001) docker     (115)    49424 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_notify.png
--rw-r--r--   0 runner    (1001) docker     (115)    53154 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/settings_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    73241 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/thunar-basic.png
--rw-r--r--   0 runner    (1001) docker     (115)    70780 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/thunar-conditions.png
--rw-r--r--   0 runner    (1001) docker     (115)    39465 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/images/thunar-custom.png
--rwxr-xr-x   0 runner    (1001) docker     (115)      695 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/index.md
--rwxr-xr-x   0 runner    (1001) docker     (115)     8971 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/installation.md
--rw-r--r--   0 runner    (1001) docker     (115)     1444 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/license.md
--rw-r--r--   0 runner    (1001) docker     (115)    12882 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/preferences.md
--rw-r--r--   0 runner    (1001) docker     (115)    15428 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/search.md
--rwxr-xr-x   0 runner    (1001) docker     (115)    12881 2019-11-17 15:38:08.000000 rummage-4.8/docs/src/markdown/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/docs/theme/
--rw-r--r--   0 runner    (1001) docker     (115)     1168 2019-11-17 15:38:08.000000 rummage-4.8/docs/theme/extra-0b9b22dd13.js
--rw-r--r--   0 runner    (1001) docker     (115)     7064 2019-11-17 15:38:08.000000 rummage-4.8/docs/theme/extra-30d8e6755c.css
--rw-r--r--   0 runner    (1001) docker     (115)  1774936 2019-11-17 15:38:08.000000 rummage-4.8/gui.fbp
--rw-r--r--   0 runner    (1001) docker     (115)     2490 2019-11-17 15:38:08.000000 rummage-4.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (115)       46 2019-11-17 15:38:08.000000 rummage-4.8/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (115)       15 2019-11-17 15:38:08.000000 rummage-4.8/requirements/extras.txt
--rw-r--r--   0 runner    (1001) docker     (115)       68 2019-11-17 15:38:08.000000 rummage-4.8/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (115)      142 2019-11-17 15:38:08.000000 rummage-4.8/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (115)        6 2019-11-17 15:38:08.000000 rummage-4.8/requirements/setup.txt
--rw-r--r--   0 runner    (1001) docker     (115)       78 2019-11-17 15:38:08.000000 rummage-4.8/requirements/test-project.txt
--rw-r--r--   0 runner    (1001) docker     (115)       32 2019-11-17 15:38:08.000000 rummage-4.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2019-11-17 15:38:08.000000 rummage-4.8/requirements/tools.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/
--rw-r--r--   0 runner    (1001) docker     (115)       89 2019-11-17 15:38:08.000000 rummage-4.8/rummage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2525 2019-11-17 15:38:08.000000 rummage-4.8/rummage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/
--rw-r--r--   0 runner    (1001) docker     (115)       22 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6967 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/
--rw-r--r--   0 runner    (1001) docker     (115)       19 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/actions/
--rw-r--r--   0 runner    (1001) docker     (115)       15 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/actions/checksum/
--rw-r--r--   0 runner    (1001) docker     (115)     3466 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2429 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/checksum/sum_hashes.py
--rw-r--r--   0 runner    (1001) docker     (115)    33392 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/checksum/tiger.py
--rw-r--r--   0 runner    (1001) docker     (115)    52458 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/checksum/whirlpool.py
--rw-r--r--   0 runner    (1001) docker     (115)     3224 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/export_csv.py
--rw-r--r--   0 runner    (1001) docker     (115)     8285 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/export_html.py
--rw-r--r--   0 runner    (1001) docker     (115)     3376 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/fileops.py
--rw-r--r--   0 runner    (1001) docker     (115)     2928 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/sanitize_json.py
--rw-r--r--   0 runner    (1001) docker     (115)     1287 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/actions/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/app/
--rw-r--r--   0 runner    (1001) docker     (115)       11 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    16875 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/app/custom_app.py
--rw-r--r--   0 runner    (1001) docker     (115)     1187 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/app/platform_window_focus.py
--rw-r--r--   0 runner    (1001) docker     (115)     4586 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/app/rummage_app.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/controls/
--rw-r--r--   0 runner    (1001) docker     (115)       24 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    14169 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/autocomplete_combo.py
--rw-r--r--   0 runner    (1001) docker     (115)     3064 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/collapsible_pane.py
--rw-r--r--   0 runner    (1001) docker     (115)     9581 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/custom_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (115)     3175 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/date_picker.py
--rw-r--r--   0 runner    (1001) docker     (115)    13130 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/dynamic_lists.py
--rw-r--r--   0 runner    (1001) docker     (115)     2616 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/encoding_list.py
--rw-r--r--   0 runner    (1001) docker     (115)     1604 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/file_picker.py
--rw-r--r--   0 runner    (1001) docker     (115)     2737 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/load_search_list.py
--rw-r--r--   0 runner    (1001) docker     (115)     2949 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/pick_button.py
--rw-r--r--   0 runner    (1001) docker     (115)    32687 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/result_lists.py
--rw-r--r--   0 runner    (1001) docker     (115)     2398 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/search_chain_list.py
--rw-r--r--   0 runner    (1001) docker     (115)     3059 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/search_error_list.py
--rw-r--r--   0 runner    (1001) docker     (115)     1409 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/time_picker.py
--rw-r--r--   0 runner    (1001) docker     (115)    10469 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/controls/webview.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/data/
--rw-r--r--   0 runner    (1001) docker     (115)     2569 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      388 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/arrow_down.png
--rw-r--r--   0 runner    (1001) docker     (115)      428 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/arrow_left.png
--rw-r--r--   0 runner    (1001) docker     (115)      412 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/arrow_right.png
--rw-r--r--   0 runner    (1001) docker     (115)      353 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/arrow_up.png
--rw-r--r--   0 runner    (1001) docker     (115)     1558 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/binary.png
--rw-r--r--   0 runner    (1001) docker     (115)     1341 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/doc.png
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/data/docs/
--rw-r--r--   0 runner    (1001) docker     (115)      628 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/404.html
--rw-r--r--   0 runner    (1001) docker     (115)    30223 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/changelog.html
--rw-r--r--   0 runner    (1001) docker     (115)     6697 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/contributing.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/data/docs/css/
--rw-r--r--   0 runner    (1001) docker     (115)    29320 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (115)    16789 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/extras.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/data/docs/images/
--rw-r--r--   0 runner    (1001) docker     (115)    11948 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/chain_button.png
--rw-r--r--   0 runner    (1001) docker     (115)    59485 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/chain_mode.png
--rw-r--r--   0 runner    (1001) docker     (115)    48842 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/chains.png
--rw-r--r--   0 runner    (1001) docker     (115)   217500 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/content_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)    17769 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/file_pattern.png
--rw-r--r--   0 runner    (1001) docker     (115)   250916 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/files_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)   169845 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/html_export.png
--rw-r--r--   0 runner    (1001) docker     (115)    44736 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/limit_search_panel.png
--rw-r--r--   0 runner    (1001) docker     (115)    45680 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/load_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    26592 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/plugin_input.png
--rw-r--r--   0 runner    (1001) docker     (115)    13786 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/plugin_toggle.png
--rw-r--r--   0 runner    (1001) docker     (115)    13254 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/regex_buttons.png
--rw-r--r--   0 runner    (1001) docker     (115)    70694 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/regex_tester.png
--rw-r--r--   0 runner    (1001) docker     (115)    19024 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/rummage.png
--rw-r--r--   0 runner    (1001) docker     (115)    34022 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/save_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    21673 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/search_replace_inputs.png
--rw-r--r--   0 runner    (1001) docker     (115)    43205 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/search_replace_panel.png
--rw-r--r--   0 runner    (1001) docker     (115)   142134 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/search_tab.png
--rw-r--r--   0 runner    (1001) docker     (115)    36090 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_backup.png
--rw-r--r--   0 runner    (1001) docker     (115)    63105 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_editor.png
--rw-r--r--   0 runner    (1001) docker     (115)    45332 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_encoding.png
--rw-r--r--   0 runner    (1001) docker     (115)    23171 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_export.png
--rw-r--r--   0 runner    (1001) docker     (115)    43099 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_general.png
--rw-r--r--   0 runner    (1001) docker     (115)    44211 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_history.png
--rw-r--r--   0 runner    (1001) docker     (115)    24429 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_import.png
--rw-r--r--   0 runner    (1001) docker     (115)    49424 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_notify.png
--rw-r--r--   0 runner    (1001) docker     (115)    53154 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/settings_search.png
--rw-r--r--   0 runner    (1001) docker     (115)    73241 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/thunar-basic.png
--rw-r--r--   0 runner    (1001) docker     (115)    70780 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/thunar-conditions.png
--rw-r--r--   0 runner    (1001) docker     (115)    39465 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/images/thunar-custom.png
--rw-r--r--   0 runner    (1001) docker     (115)     2073 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (115)    13313 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/installation.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/data/docs/js/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (115)     2365 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/license.html
--rw-r--r--   0 runner    (1001) docker     (115)    19622 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/preferences.html
--rw-r--r--   0 runner    (1001) docker     (115)    22859 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (115)     1064 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/sitemap.html
--rw-r--r--   0 runner    (1001) docker     (115)    23659 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/docs/usage.html
--rw-r--r--   0 runner    (1001) docker     (115)     2073 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/error.png
--rw-r--r--   0 runner    (1001) docker     (115)      892 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/glass.png
--rw-r--r--   0 runner    (1001) docker     (115)     2396 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/results.css
--rw-r--r--   0 runner    (1001) docker     (115)  1140921 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage.icns
--rw-r--r--   0 runner    (1001) docker     (115)    80645 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage.ico
--rw-r--r--   0 runner    (1001) docker     (115)    19024 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage.png
--rw-r--r--   0 runner    (1001) docker     (115)    19289 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage_dialog.png
--rw-r--r--   0 runner    (1001) docker     (115)   435743 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage_hires.png
--rw-r--r--   0 runner    (1001) docker     (115)   150826 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage_large.png
--rw-r--r--   0 runner    (1001) docker     (115)    51596 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage_medium.png
--rw-r--r--   0 runner    (1001) docker     (115)     4286 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/rummage_tray.ico
--rw-r--r--   0 runner    (1001) docker     (115)    17430 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/data/sorttable.js
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (115)       15 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4705 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/checksum_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     4680 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/column_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     8110 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/delete_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     7014 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/edit_search_chain_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     1734 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/error_text_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     3901 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/export_settings_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     2816 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/file_ext_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     2692 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/generic_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (115)     2314 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/html_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)    14893 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/import_settings_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     7077 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/load_search_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)    94027 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/msg_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (115)     3210 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/overwrite_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)    26851 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/regex_test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)    90420 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/rummage_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     7609 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/save_search_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     4157 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/search_chain_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     2889 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/search_error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)    24283 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/settings_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)     5902 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/dialogs/support_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (115)   117183 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/
--rw-r--r--   0 runner    (1001) docker     (115)      978 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/localization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/locale/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/locale/en_US/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (115)    33292 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/rummage.po
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/locale/ru_RU/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (115)    39225 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/rummage.po
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/notify/
--rw-r--r--   0 runner    (1001) docker     (115)     3592 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3452 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/notify_growl.py
--rw-r--r--   0 runner    (1001) docker     (115)     3207 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/notify_linux.py
--rw-r--r--   0 runner    (1001) docker     (115)     5380 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/notify_osx.py
--rw-r--r--   0 runner    (1001) docker     (115)    10090 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/notify_windows.py
--rw-r--r--   0 runner    (1001) docker     (115)      513 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/notify/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/settings/
--rw-r--r--   0 runner    (1001) docker     (115)    48884 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/gui/util/
--rw-r--r--   0 runner    (1001) docker     (115)     4137 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2018 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/util/images.py
--rw-r--r--   0 runner    (1001) docker     (115)   155796 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/util/png.py
--rw-r--r--   0 runner    (1001) docker     (115)    10803 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/gui/util/rgba.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage/lib/rumcore/
--rw-r--r--   0 runner    (1001) docker     (115)    56036 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/rumcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    16154 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/rumcore/text_decode.py
--rw-r--r--   0 runner    (1001) docker     (115)     1344 2019-11-17 15:38:08.000000 rummage-4.8/rummage/lib/rumcore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     4853 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     8119 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       82 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (115)      167 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)        8 2019-11-17 15:38:17.000000 rummage-4.8/rummage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)      551 2019-11-17 15:38:17.000000 rummage-4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     3336 2019-11-17 15:38:08.000000 rummage-4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (115)       24 2019-11-17 15:38:08.000000 rummage-4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    36532 2019-11-17 15:38:08.000000 rummage-4.8/tests/test_rumcore.py
--rw-r--r--   0 runner    (1001) docker     (115)    23541 2019-11-17 15:38:08.000000 rummage-4.8/tests/test_text_decode.py
--rw-r--r--   0 runner    (1001) docker     (115)     3969 2019-11-17 15:38:08.000000 rummage-4.8/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (115)     1640 2019-11-17 15:38:08.000000 rummage-4.8/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-11-17 15:38:17.000000 rummage-4.8/tools/
--rw-r--r--   0 runner    (1001) docker     (115)       13 2019-11-17 15:38:08.000000 rummage-4.8/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4212 2019-11-17 15:38:08.000000 rummage-4.8/tools/gen_docs.py
--rw-r--r--   0 runner    (1001) docker     (115)      602 2019-11-17 15:38:08.000000 rummage-4.8/tools/gui_patch.py
--rw-r--r--   0 runner    (1001) docker     (115)      829 2019-11-17 15:38:08.000000 rummage-4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/
+-rw-r--r--   0 runner    (1001) docker     (115)      120 2020-01-19 19:59:40.000000 rummage-4.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (115)     1097 2020-01-19 19:59:40.000000 rummage-4.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (115)      523 2020-01-19 19:59:40.000000 rummage-4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)     5097 2020-01-19 19:59:45.000000 rummage-4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     3774 2020-01-19 19:59:40.000000 rummage-4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/internal_theme/
+-rw-r--r--   0 runner    (1001) docker     (115)      130 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/404.html
+-rw-r--r--   0 runner    (1001) docker     (115)     2192 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/internal_theme/css/
+-rw-r--r--   0 runner    (1001) docker     (115)    29320 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/internal_theme/js/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (115)       26 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/main.html
+-rw-r--r--   0 runner    (1001) docker     (115)      347 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/nav.html
+-rw-r--r--   0 runner    (1001) docker     (115)      192 2020-01-19 19:59:40.000000 rummage-4.9/docs/internal_theme/sitemap.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/src/markdown/
+-rw-r--r--   0 runner    (1001) docker     (115)    21998 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (115)     3847 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (115)     8740 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/extras.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/src/markdown/images/
+-rw-r--r--   0 runner    (1001) docker     (115)    11948 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/chain_button.png
+-rw-r--r--   0 runner    (1001) docker     (115)    59485 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/chain_mode.png
+-rw-r--r--   0 runner    (1001) docker     (115)    48842 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/chains.png
+-rw-r--r--   0 runner    (1001) docker     (115)   217500 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/content_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)    17769 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/file_pattern.png
+-rw-r--r--   0 runner    (1001) docker     (115)   250916 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/files_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)   169845 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/html_export.png
+-rw-r--r--   0 runner    (1001) docker     (115)    44736 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/limit_search_panel.png
+-rw-r--r--   0 runner    (1001) docker     (115)    45680 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/load_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    26592 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/plugin_input.png
+-rw-r--r--   0 runner    (1001) docker     (115)    13786 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/plugin_toggle.png
+-rw-r--r--   0 runner    (1001) docker     (115)    13254 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/regex_buttons.png
+-rw-r--r--   0 runner    (1001) docker     (115)    70694 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/regex_tester.png
+-rw-r--r--   0 runner    (1001) docker     (115)    19024 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/rummage.png
+-rw-r--r--   0 runner    (1001) docker     (115)    34022 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/save_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    21673 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/search_replace_inputs.png
+-rw-r--r--   0 runner    (1001) docker     (115)    43205 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/search_replace_panel.png
+-rw-r--r--   0 runner    (1001) docker     (115)   142134 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/search_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)    36090 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_backup.png
+-rw-r--r--   0 runner    (1001) docker     (115)    63105 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_editor.png
+-rw-r--r--   0 runner    (1001) docker     (115)    45332 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_encoding.png
+-rw-r--r--   0 runner    (1001) docker     (115)    23171 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_export.png
+-rw-r--r--   0 runner    (1001) docker     (115)    43099 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_general.png
+-rw-r--r--   0 runner    (1001) docker     (115)    44211 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_history.png
+-rw-r--r--   0 runner    (1001) docker     (115)    24429 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_import.png
+-rw-r--r--   0 runner    (1001) docker     (115)    49424 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_notify.png
+-rw-r--r--   0 runner    (1001) docker     (115)    53154 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/settings_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    73241 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/thunar-basic.png
+-rw-r--r--   0 runner    (1001) docker     (115)    70780 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/thunar-conditions.png
+-rw-r--r--   0 runner    (1001) docker     (115)    39465 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/images/thunar-custom.png
+-rwxr-xr-x   0 runner    (1001) docker     (115)      695 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (115)     8971 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/installation.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1444 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/license.md
+-rw-r--r--   0 runner    (1001) docker     (115)    12882 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/preferences.md
+-rw-r--r--   0 runner    (1001) docker     (115)    15428 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/search.md
+-rwxr-xr-x   0 runner    (1001) docker     (115)    12881 2020-01-19 19:59:40.000000 rummage-4.9/docs/src/markdown/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/docs/theme/
+-rw-r--r--   0 runner    (1001) docker     (115)     1168 2020-01-19 19:59:40.000000 rummage-4.9/docs/theme/extra-0b9b22dd13.js
+-rw-r--r--   0 runner    (1001) docker     (115)     7064 2020-01-19 19:59:40.000000 rummage-4.9/docs/theme/extra-30d8e6755c.css
+-rw-r--r--   0 runner    (1001) docker     (115)  1774936 2020-01-19 19:59:40.000000 rummage-4.9/gui.fbp
+-rw-r--r--   0 runner    (1001) docker     (115)     3102 2020-01-19 19:59:40.000000 rummage-4.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (115)       46 2020-01-19 19:59:40.000000 rummage-4.9/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       15 2020-01-19 19:59:40.000000 rummage-4.9/requirements/extras.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       68 2020-01-19 19:59:40.000000 rummage-4.9/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      140 2020-01-19 19:59:40.000000 rummage-4.9/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        6 2020-01-19 19:59:40.000000 rummage-4.9/requirements/setup.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       76 2020-01-19 19:59:40.000000 rummage-4.9/requirements/test-project.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       32 2020-01-19 19:59:40.000000 rummage-4.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        9 2020-01-19 19:59:40.000000 rummage-4.9/requirements/tools.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/
+-rw-r--r--   0 runner    (1001) docker     (115)       89 2020-01-19 19:59:40.000000 rummage-4.9/rummage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2525 2020-01-19 19:59:40.000000 rummage-4.9/rummage/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/
+-rw-r--r--   0 runner    (1001) docker     (115)       22 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6967 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/
+-rw-r--r--   0 runner    (1001) docker     (115)       19 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/actions/
+-rw-r--r--   0 runner    (1001) docker     (115)       15 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/actions/checksum/
+-rw-r--r--   0 runner    (1001) docker     (115)     3466 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2429 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/checksum/sum_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (115)    33392 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/checksum/tiger.py
+-rw-r--r--   0 runner    (1001) docker     (115)    52458 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/checksum/whirlpool.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3224 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8285 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/export_html.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3376 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2928 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/sanitize_json.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1287 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/actions/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/app/
+-rw-r--r--   0 runner    (1001) docker     (115)       11 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16875 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/app/custom_app.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1187 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/app/platform_window_focus.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4586 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/app/rummage_app.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/controls/
+-rw-r--r--   0 runner    (1001) docker     (115)       24 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    14169 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/autocomplete_combo.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3064 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/collapsible_pane.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9581 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/custom_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3175 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/date_picker.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13130 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/dynamic_lists.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2616 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/encoding_list.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1604 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/file_picker.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2737 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/load_search_list.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2949 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/pick_button.py
+-rw-r--r--   0 runner    (1001) docker     (115)    32687 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/result_lists.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2398 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/search_chain_list.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3059 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/search_error_list.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1409 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/time_picker.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10469 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/controls/webview.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (115)     2569 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      388 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/arrow_down.png
+-rw-r--r--   0 runner    (1001) docker     (115)      428 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/arrow_left.png
+-rw-r--r--   0 runner    (1001) docker     (115)      412 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/arrow_right.png
+-rw-r--r--   0 runner    (1001) docker     (115)      353 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/arrow_up.png
+-rw-r--r--   0 runner    (1001) docker     (115)     1558 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/binary.png
+-rw-r--r--   0 runner    (1001) docker     (115)     1341 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/doc.png
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/data/docs/
+-rw-r--r--   0 runner    (1001) docker     (115)      628 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/404.html
+-rw-r--r--   0 runner    (1001) docker     (115)    30427 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/changelog.html
+-rw-r--r--   0 runner    (1001) docker     (115)     6697 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/contributing.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/data/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (115)    29320 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (115)    16789 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/extras.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/data/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (115)    11948 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/chain_button.png
+-rw-r--r--   0 runner    (1001) docker     (115)    59485 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/chain_mode.png
+-rw-r--r--   0 runner    (1001) docker     (115)    48842 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/chains.png
+-rw-r--r--   0 runner    (1001) docker     (115)   217500 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/content_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)    17769 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/file_pattern.png
+-rw-r--r--   0 runner    (1001) docker     (115)   250916 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/files_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)   169845 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/html_export.png
+-rw-r--r--   0 runner    (1001) docker     (115)    44736 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/limit_search_panel.png
+-rw-r--r--   0 runner    (1001) docker     (115)    45680 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/load_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    26592 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/plugin_input.png
+-rw-r--r--   0 runner    (1001) docker     (115)    13786 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/plugin_toggle.png
+-rw-r--r--   0 runner    (1001) docker     (115)    13254 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/regex_buttons.png
+-rw-r--r--   0 runner    (1001) docker     (115)    70694 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/regex_tester.png
+-rw-r--r--   0 runner    (1001) docker     (115)    19024 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/rummage.png
+-rw-r--r--   0 runner    (1001) docker     (115)    34022 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/save_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    21673 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/search_replace_inputs.png
+-rw-r--r--   0 runner    (1001) docker     (115)    43205 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/search_replace_panel.png
+-rw-r--r--   0 runner    (1001) docker     (115)   142134 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/search_tab.png
+-rw-r--r--   0 runner    (1001) docker     (115)    36090 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_backup.png
+-rw-r--r--   0 runner    (1001) docker     (115)    63105 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_editor.png
+-rw-r--r--   0 runner    (1001) docker     (115)    45332 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_encoding.png
+-rw-r--r--   0 runner    (1001) docker     (115)    23171 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_export.png
+-rw-r--r--   0 runner    (1001) docker     (115)    43099 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_general.png
+-rw-r--r--   0 runner    (1001) docker     (115)    44211 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_history.png
+-rw-r--r--   0 runner    (1001) docker     (115)    24429 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_import.png
+-rw-r--r--   0 runner    (1001) docker     (115)    49424 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_notify.png
+-rw-r--r--   0 runner    (1001) docker     (115)    53154 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/settings_search.png
+-rw-r--r--   0 runner    (1001) docker     (115)    73241 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/thunar-basic.png
+-rw-r--r--   0 runner    (1001) docker     (115)    70780 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/thunar-conditions.png
+-rw-r--r--   0 runner    (1001) docker     (115)    39465 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/images/thunar-custom.png
+-rw-r--r--   0 runner    (1001) docker     (115)     2073 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (115)    13313 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/installation.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/data/docs/js/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (115)     2365 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/license.html
+-rw-r--r--   0 runner    (1001) docker     (115)    19622 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/preferences.html
+-rw-r--r--   0 runner    (1001) docker     (115)    22859 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (115)     1064 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (115)    23659 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/docs/usage.html
+-rw-r--r--   0 runner    (1001) docker     (115)     2073 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/error.png
+-rw-r--r--   0 runner    (1001) docker     (115)      892 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/glass.png
+-rw-r--r--   0 runner    (1001) docker     (115)     2396 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/results.css
+-rw-r--r--   0 runner    (1001) docker     (115)  1140921 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage.icns
+-rw-r--r--   0 runner    (1001) docker     (115)    80645 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage.ico
+-rw-r--r--   0 runner    (1001) docker     (115)    19024 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage.png
+-rw-r--r--   0 runner    (1001) docker     (115)    19289 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (115)   435743 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage_hires.png
+-rw-r--r--   0 runner    (1001) docker     (115)   150826 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage_large.png
+-rw-r--r--   0 runner    (1001) docker     (115)    51596 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage_medium.png
+-rw-r--r--   0 runner    (1001) docker     (115)     4286 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/rummage_tray.ico
+-rw-r--r--   0 runner    (1001) docker     (115)    17430 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/data/sorttable.js
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (115)       15 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4705 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/checksum_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4680 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/column_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8110 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/delete_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7014 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/edit_search_chain_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1734 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/error_text_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3901 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/export_settings_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2816 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/file_ext_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2692 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/generic_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2314 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/html_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)    14893 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/import_settings_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7077 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/load_search_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)    94027 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/msg_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3210 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/overwrite_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)    26851 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/regex_test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)    90420 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/rummage_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7609 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/save_search_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4157 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/search_chain_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2889 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/search_error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)    24283 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/settings_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5906 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/dialogs/support_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (115)   117183 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/
+-rw-r--r--   0 runner    (1001) docker     (115)      978 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/localization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/locale/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/locale/en_US/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (115)    33292 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/rummage.po
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/locale/ru_RU/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (115)    39225 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/rummage.po
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/notify/
+-rw-r--r--   0 runner    (1001) docker     (115)     3592 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3452 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/notify_growl.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3207 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/notify_linux.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5380 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/notify_osx.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10090 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/notify_windows.py
+-rw-r--r--   0 runner    (1001) docker     (115)      513 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/notify/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/settings/
+-rw-r--r--   0 runner    (1001) docker     (115)    48884 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/gui/util/
+-rw-r--r--   0 runner    (1001) docker     (115)     4137 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2018 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/util/images.py
+-rw-r--r--   0 runner    (1001) docker     (115)   155796 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/util/png.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10803 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/gui/util/rgba.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage/lib/rumcore/
+-rw-r--r--   0 runner    (1001) docker     (115)    56036 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/rumcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16154 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/rumcore/text_decode.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1344 2020-01-19 19:59:40.000000 rummage-4.9/rummage/lib/rumcore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     5097 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     8119 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       82 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (115)      165 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        8 2020-01-19 19:59:45.000000 rummage-4.9/rummage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      551 2020-01-19 19:59:45.000000 rummage-4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     3336 2020-01-19 19:59:40.000000 rummage-4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)       24 2020-01-19 19:59:40.000000 rummage-4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    36532 2020-01-19 19:59:40.000000 rummage-4.9/tests/test_rumcore.py
+-rw-r--r--   0 runner    (1001) docker     (115)    23541 2020-01-19 19:59:40.000000 rummage-4.9/tests/test_text_decode.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3969 2020-01-19 19:59:40.000000 rummage-4.9/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1640 2020-01-19 19:59:40.000000 rummage-4.9/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-19 19:59:45.000000 rummage-4.9/tools/
+-rw-r--r--   0 runner    (1001) docker     (115)       13 2020-01-19 19:59:40.000000 rummage-4.9/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4212 2020-01-19 19:59:40.000000 rummage-4.9/tools/gen_docs.py
+-rw-r--r--   0 runner    (1001) docker     (115)      602 2020-01-19 19:59:40.000000 rummage-4.9/tools/gui_patch.py
+-rw-r--r--   0 runner    (1001) docker     (115)      829 2020-01-19 19:59:40.000000 rummage-4.9/tox.ini
```

### Comparing `rummage-4.8/LICENSE.md` & `rummage-4.9/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT license.
 
-Copyright (c) 2013 - 2019 Isaac Muse <isaacmuse@gmail.com>
+Copyright (c) 2013 - 2020 Isaac Muse <isaacmuse@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `rummage-4.8/MANIFEST.in` & `rummage-4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rummage-4.8/PKG-INFO` & `rummage-4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: rummage
-Version: 4.8
+Version: 4.9
 Summary: A GUI search and replace app.
 Home-page: https://github.com/facelessuser/Rummage
 Author: Isaac Muse
 Author-email: Isaac.Muse@gmail.com
 License: MIT License
-Description: [![Build][github-ci-image]][github-ci-link]
+Description: [![Gitter][gitter-image]][gitter-link]
+        [![Build][github-ci-image]][github-ci-link]
         [![Unix Build Status][travis-image]][travis-link]
         [![Windows Build Status][appveyor-image]][appveyor-link]
         [![Coverage][codecov-image]][codecov-link]
-        [![Requirements Status][requires-image]][requires-link]
         [![PyPI Version][pypi-image]][pypi-link]
+        [![PyPI - Python Version][python-image]][pypi-link]
         ![License][license-image-mit]
         
         Rummage
         =======
         
         Rummage is a cross platform search and replace tool. Rummage crawls directories and searches for specified patterns (either regular expression or literal) and can optionally replace those targets with desired text.
         
@@ -27,42 +28,43 @@
         
         ![Rummage Files](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/files_tab.png)
         
         ![Rummage Content](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/content_tab.png)
         
         # Documentation
         
-        http://facelessuser.github.io/Rummage/
+        https://facelessuser.github.io/Rummage/
         
         License
         =======
         
         Rummage is released under the MIT license.
         
-        Copyright (c) 2013 - 2019 Isaac Muse <isaacmuse@gmail.com>
+        Copyright (c) 2013 - 2020 Isaac Muse <isaacmuse@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         [github-ci-image]: https://github.com/facelessuser/Rummage/workflows/build/badge.svg
         [github-ci-link]: https://github.com/facelessuser/Rummage/actions?workflow=build
-        [travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=Unix%20Build
+        [travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=travis&logo=travis%20ci&logoColor=cccccc
         [travis-link]: https://travis-ci.org/facelessuser/Rummage
-        [appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=Windows%20Build
+        [appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=appveyor&logo=appveyor&logoColor=cccccc
         [appveyor-link]: https://ci.appveyor.com/project/facelessuser/Rummage
         [license-image]: https://img.shields.io/badge/license-MIT-blue.svg
-        [codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg
+        [codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg?logo=codecov&logoColor=cccccc
         [codecov-link]: http://codecov.io/github/facelessuser/Rummage?branch=master
-        [requires-image]: https://img.shields.io/requires/github/facelessuser/Rummage/master.svg
-        [requires-link]: https://requires.io/github/facelessuser/Rummage/requirements/?branch=master
-        [pypi-image]: https://img.shields.io/pypi/v/Rummage.svg
+        [gitter-image]: https://img.shields.io/gitter/room/facelessuser/Rummage.svg?logo=gitter&color=fuchsia&logoColor=cccccc
+        [gitter-link]: https://gitter.im/facelessuser/Rummage
+        [pypi-image]: https://img.shields.io/pypi/v/Rummage.svg?logo=pypi&logoColor=cccccc
         [pypi-link]: https://pypi.python.org/pypi/Rummage
+        [python-image]: https://img.shields.io/pypi/pyversions/Rummage?logo=python&logoColor=cccccc
         [license-image-mit]: https://img.shields.io/badge/license-MIT-blue.svg
         
 Keywords: grep search find replace gui
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rummage-4.8/README.md` & `rummage-4.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+[![Gitter][gitter-image]][gitter-link]
 [![Build][github-ci-image]][github-ci-link]
 [![Unix Build Status][travis-image]][travis-link]
 [![Windows Build Status][appveyor-image]][appveyor-link]
 [![Coverage][codecov-image]][codecov-link]
-[![Requirements Status][requires-image]][requires-link]
 [![PyPI Version][pypi-image]][pypi-link]
+[![PyPI - Python Version][python-image]][pypi-link]
 ![License][license-image-mit]
 
 Rummage
 =======
 
 Rummage is a cross platform search and replace tool. Rummage crawls directories and searches for specified patterns (either regular expression or literal) and can optionally replace those targets with desired text.
 
@@ -19,36 +20,37 @@
 
 ![Rummage Files](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/files_tab.png)
 
 ![Rummage Content](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/content_tab.png)
 
 # Documentation
 
-http://facelessuser.github.io/Rummage/
+https://facelessuser.github.io/Rummage/
 
 License
 =======
 
 Rummage is released under the MIT license.
 
-Copyright (c) 2013 - 2019 Isaac Muse <isaacmuse@gmail.com>
+Copyright (c) 2013 - 2020 Isaac Muse <isaacmuse@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 [github-ci-image]: https://github.com/facelessuser/Rummage/workflows/build/badge.svg
 [github-ci-link]: https://github.com/facelessuser/Rummage/actions?workflow=build
-[travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=Unix%20Build
+[travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=travis&logo=travis%20ci&logoColor=cccccc
 [travis-link]: https://travis-ci.org/facelessuser/Rummage
-[appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=Windows%20Build
+[appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=appveyor&logo=appveyor&logoColor=cccccc
 [appveyor-link]: https://ci.appveyor.com/project/facelessuser/Rummage
 [license-image]: https://img.shields.io/badge/license-MIT-blue.svg
-[codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg
+[codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg?logo=codecov&logoColor=cccccc
 [codecov-link]: http://codecov.io/github/facelessuser/Rummage?branch=master
-[requires-image]: https://img.shields.io/requires/github/facelessuser/Rummage/master.svg
-[requires-link]: https://requires.io/github/facelessuser/Rummage/requirements/?branch=master
-[pypi-image]: https://img.shields.io/pypi/v/Rummage.svg
+[gitter-image]: https://img.shields.io/gitter/room/facelessuser/Rummage.svg?logo=gitter&color=fuchsia&logoColor=cccccc
+[gitter-link]: https://gitter.im/facelessuser/Rummage
+[pypi-image]: https://img.shields.io/pypi/v/Rummage.svg?logo=pypi&logoColor=cccccc
 [pypi-link]: https://pypi.python.org/pypi/Rummage
+[python-image]: https://img.shields.io/pypi/pyversions/Rummage?logo=python&logoColor=cccccc
 [license-image-mit]: https://img.shields.io/badge/license-MIT-blue.svg
```

### Comparing `rummage-4.8/docs/internal_theme/base.html` & `rummage-4.9/docs/internal_theme/base.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/internal_theme/css/theme.css` & `rummage-4.9/docs/internal_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/changelog.md` & `rummage-4.9/docs/src/markdown/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 4.9.0
+
+- **NEW**: Require `wcmatch` 5.1.0+, `bracex` 1.4.0, and `backrefs` `1.3.0` to include latest bug fixes.
+
 ## 4.8.0
 
 - **NEW**: Supports installing extras via `pip install rummage[extras]`.
 - **FIX**: Fix for notification sound display in settings dialog.
 - **FIX**: Fix notification sound not playing on Linux when configured.
 
 ## 4.7.1
```

### Comparing `rummage-4.8/docs/src/markdown/contributing.md` & `rummage-4.9/docs/src/markdown/contributing.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/extras.md` & `rummage-4.9/docs/src/markdown/extras.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/chain_button.png` & `rummage-4.9/docs/src/markdown/images/chain_button.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/chain_mode.png` & `rummage-4.9/docs/src/markdown/images/chain_mode.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/chains.png` & `rummage-4.9/docs/src/markdown/images/chains.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/content_tab.png` & `rummage-4.9/docs/src/markdown/images/content_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/file_pattern.png` & `rummage-4.9/docs/src/markdown/images/file_pattern.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/files_tab.png` & `rummage-4.9/docs/src/markdown/images/files_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/html_export.png` & `rummage-4.9/docs/src/markdown/images/html_export.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/limit_search_panel.png` & `rummage-4.9/docs/src/markdown/images/limit_search_panel.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/load_search.png` & `rummage-4.9/docs/src/markdown/images/load_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/plugin_input.png` & `rummage-4.9/docs/src/markdown/images/plugin_input.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/plugin_toggle.png` & `rummage-4.9/docs/src/markdown/images/plugin_toggle.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/regex_buttons.png` & `rummage-4.9/docs/src/markdown/images/regex_buttons.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/regex_tester.png` & `rummage-4.9/docs/src/markdown/images/regex_tester.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/rummage.png` & `rummage-4.9/docs/src/markdown/images/rummage.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/save_search.png` & `rummage-4.9/docs/src/markdown/images/save_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/search_replace_inputs.png` & `rummage-4.9/docs/src/markdown/images/search_replace_inputs.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/search_replace_panel.png` & `rummage-4.9/docs/src/markdown/images/search_replace_panel.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/search_tab.png` & `rummage-4.9/docs/src/markdown/images/search_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_backup.png` & `rummage-4.9/docs/src/markdown/images/settings_backup.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_editor.png` & `rummage-4.9/docs/src/markdown/images/settings_editor.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_encoding.png` & `rummage-4.9/docs/src/markdown/images/settings_encoding.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_export.png` & `rummage-4.9/docs/src/markdown/images/settings_export.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_general.png` & `rummage-4.9/docs/src/markdown/images/settings_general.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_history.png` & `rummage-4.9/docs/src/markdown/images/settings_history.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_import.png` & `rummage-4.9/docs/src/markdown/images/settings_import.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_notify.png` & `rummage-4.9/docs/src/markdown/images/settings_notify.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/settings_search.png` & `rummage-4.9/docs/src/markdown/images/settings_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/thunar-basic.png` & `rummage-4.9/docs/src/markdown/images/thunar-basic.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/thunar-conditions.png` & `rummage-4.9/docs/src/markdown/images/thunar-conditions.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/images/thunar-custom.png` & `rummage-4.9/docs/src/markdown/images/thunar-custom.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/index.md` & `rummage-4.9/docs/src/markdown/index.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/installation.md` & `rummage-4.9/docs/src/markdown/installation.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/license.md` & `rummage-4.9/docs/src/markdown/license.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # License
 
 MIT license.
 
-Copyright (c) 2013 - 2019 Isaac Muse <isaacmuse@gmail.com>
+Copyright (c) 2013 - 2020 Isaac Muse <isaacmuse@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `rummage-4.8/docs/src/markdown/preferences.md` & `rummage-4.9/docs/src/markdown/preferences.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/search.md` & `rummage-4.9/docs/src/markdown/search.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/src/markdown/usage.md` & `rummage-4.9/docs/src/markdown/usage.md`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/theme/extra-0b9b22dd13.js` & `rummage-4.9/docs/theme/extra-0b9b22dd13.js`

 * *Files identical despite different names*

### Comparing `rummage-4.8/docs/theme/extra-30d8e6755c.css` & `rummage-4.9/docs/theme/extra-30d8e6755c.css`

 * *Files identical despite different names*

### Comparing `rummage-4.8/gui.fbp` & `rummage-4.9/gui.fbp`

 * *Files identical despite different names*

### Comparing `rummage-4.8/mkdocs.yml` & `rummage-4.9/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 site_name: Rummage Documentation
 site_url: https://facelessuser.github.io/Rummage
 repo_url: https://github.com/facelessuser/Rummage
 edit_uri: tree/master/docs/src/markdown
 site_description: A search and replace tool written in Python.
 copyright: |
-  Copyright &copy; 2013 - 2019 <a href="https://github.com/facelessuser">Isaac Muse</a>
-  <br><span class="md-footer-custom-text">emoji provided free by <a href="https://github.com/twitter/twemoji">Twemoji</a></span>
+  Copyright &copy; 2013 - 2020 <a href="https://github.com/facelessuser">Isaac Muse</a>
+  <br><span class="md-footer-custom-text">emoji provided free by </span>
+  <a href="https://github.com/twitter/twemoji">Twemoji</a>
 
 docs_dir: docs/src/markdown
 theme:
   name: material
   custom_dir: docs/theme
   palette:
     primary: blue
@@ -41,26 +42,42 @@
   - markdown.extensions.attr_list:
   - markdown.extensions.def_list:
   - markdown.extensions.tables:
   - markdown.extensions.abbr:
   - markdown.extensions.footnotes:
   - pymdownx.extrarawhtml:
   - pymdownx.superfences:
+      preserve_tabs: true
+      custom_fences: 
+        - name: flow
+          class: uml-flowchart
+          format: !!python/name:pymdownx.superfences.fence_code_format
+        - name: sequence
+          class: uml-sequence-diagram
+          format: !!python/name:pymdownx.superfences.fence_code_format
+        - name: math
+          class: arithmatex
+          format: !!python/name:pymdownx.arithmatex.fence_mathjax_format
   - pymdownx.highlight:
       css_class: codehilite
       extend_pygments_lang:
         - name: php-inline
           lang: php
           options:
             startinline: true
         - name: pycon3
           lang: pycon
           options:
             python3: true
+      linenums_style: pymdownx-inline
   - pymdownx.inlinehilite:
+      custom_inline:
+        - name: math
+          class: arithmatex
+          format: !!python/name:pymdownx.arithmatex.inline_mathjax_format
   - pymdownx.magiclink:
       repo_url_shortener: true
       repo_url_shorthand: true
       social_url_shorthand: true
       user: facelessuser
       repo: Rummage
   - pymdownx.tilde:
@@ -82,10 +99,10 @@
   - pymdownx.details:
 
 extra:
   social:
     - type: github
       link: https://github.com/facelessuser
 extra_css:
-  - extra-30d8e6755c.css
+  - extra-174a536342.css
 extra_javascript:
-  - extra-0b9b22dd13.js
+  - extra-0d9305e748.js
```

#### html2text {}

```diff
@@ -1,29 +1,37 @@
 site_name: Rummage Documentation site_url: https://facelessuser.github.io/
 Rummage repo_url: https://github.com/facelessuser/Rummage edit_uri: tree/
 master/docs/src/markdown site_description: A search and replace tool written in
-Python. copyright: | Copyright © 2013 - 2019 Isaac_Muse
-emoji provided free by Twemoji docs_dir: docs/src/markdown theme: name:
+Python. copyright: | Copyright © 2013 - 2020 Isaac_Muse
+emoji provided free by  Twemoji docs_dir: docs/src/markdown theme: name:
 material custom_dir: docs/theme palette: primary: blue accent: blue logo:
 images/rummage.png font: text: Roboto code: Roboto Mono nav: - Rummage:
 index.md - Installation: installation.md - Basic Usage: usage.md - Search
 Features: search.md - Settings: preferences.md - Extras: extras.md -
 Contributing & Support: contributing.md - Changelog: changelog.md - License:
 license.md markdown_extensions: - markdown.extensions.toc: slugify: !!python/
 name:pymdownx.slugs.uslugify permalink: "\ue157" -
 markdown.extensions.admonition: - markdown.extensions.smarty: smart_quotes:
 false - pymdownx.betterem: - markdown.extensions.attr_list: -
 markdown.extensions.def_list: - markdown.extensions.tables: -
 markdown.extensions.abbr: - markdown.extensions.footnotes: -
-pymdownx.extrarawhtml: - pymdownx.superfences: - pymdownx.highlight: css_class:
+pymdownx.extrarawhtml: - pymdownx.superfences: preserve_tabs: true
+custom_fences: - name: flow class: uml-flowchart format: !!python/name:
+pymdownx.superfences.fence_code_format - name: sequence class: uml-sequence-
+diagram format: !!python/name:pymdownx.superfences.fence_code_format - name:
+math class: arithmatex format: !!python/name:
+pymdownx.arithmatex.fence_mathjax_format - pymdownx.highlight: css_class:
 codehilite extend_pygments_lang: - name: php-inline lang: php options:
-startinline: true - name: pycon3 lang: pycon options: python3: true -
-pymdownx.inlinehilite: - pymdownx.magiclink: repo_url_shortener: true
-repo_url_shorthand: true social_url_shorthand: true user: facelessuser repo:
-Rummage - pymdownx.tilde: - pymdownx.caret: - pymdownx.smartsymbols: -
-pymdownx.emoji: emoji_index: !!python/name:pymdownx.emoji.twemoji
-emoji_generator: !!python/name:pymdownx.emoji.to_svg - pymdownx.escapeall:
-hardbreak: True nbsp: True - pymdownx.tasklist: custom_checkbox: true -
-pymdownx.striphtml: - pymdownx.snippets: base_path: docs/src/markdown/_snippets
-- pymdownx.keys: separator: "\uff0b" - pymdownx.details: extra: social: - type:
-github link: https://github.com/facelessuser extra_css: - extra-30d8e6755c.css
-extra_javascript: - extra-0b9b22dd13.js
+startinline: true - name: pycon3 lang: pycon options: python3: true
+linenums_style: pymdownx-inline - pymdownx.inlinehilite: custom_inline: - name:
+math class: arithmatex format: !!python/name:
+pymdownx.arithmatex.inline_mathjax_format - pymdownx.magiclink:
+repo_url_shortener: true repo_url_shorthand: true social_url_shorthand: true
+user: facelessuser repo: Rummage - pymdownx.tilde: - pymdownx.caret: -
+pymdownx.smartsymbols: - pymdownx.emoji: emoji_index: !!python/name:
+pymdownx.emoji.twemoji emoji_generator: !!python/name:pymdownx.emoji.to_svg -
+pymdownx.escapeall: hardbreak: True nbsp: True - pymdownx.tasklist:
+custom_checkbox: true - pymdownx.striphtml: - pymdownx.snippets: base_path:
+docs/src/markdown/_snippets - pymdownx.keys: separator: "\uff0b" -
+pymdownx.details: extra: social: - type: github link: https://github.com/
+facelessuser extra_css: - extra-174a536342.css extra_javascript: - extra-
+0d9305e748.js
```

### Comparing `rummage-4.8/rummage/__main__.py` & `rummage-4.9/rummage/__main__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/__meta__.py` & `rummage-4.9/rummage/lib/__meta__.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     # Handle post
     post = int(m.group('post')) if m.group('post') else 0
 
     return Version(major, minor, micro, release, pre, post, dev)
 
 
 #   (major, minor, micro, release type, pre-release build, post-release build, development-release)
-__version_info__ = Version(4, 8, 0, 'final')
+__version_info__ = Version(4, 9, 0, 'final')
 __version__ = __version_info__._get_canonical()
 __app__ = "Rummage"
 __status__ = __version_info__[3]
 __maintainers__ = [("Isaac Muse", "IsaacMuse@gmail.com")]
 __help__ = "https://github.com/facelessuser/Rummage/issues"
 __manual__ = "http://facelessuser.github.io/Rummage/"
 __changelog__ = "https://facelessuser.github.io/Rummage/changelog/"
```

### Comparing `rummage-4.8/rummage/lib/gui/actions/checksum/__init__.py` & `rummage-4.9/rummage/lib/gui/actions/checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/checksum/sum_hashes.py` & `rummage-4.9/rummage/lib/gui/actions/checksum/sum_hashes.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/checksum/tiger.py` & `rummage-4.9/rummage/lib/gui/actions/checksum/tiger.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/checksum/whirlpool.py` & `rummage-4.9/rummage/lib/gui/actions/checksum/whirlpool.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/export_csv.py` & `rummage-4.9/rummage/lib/gui/actions/export_csv.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/export_html.py` & `rummage-4.9/rummage/lib/gui/actions/export_html.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/fileops.py` & `rummage-4.9/rummage/lib/gui/actions/fileops.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/sanitize_json.py` & `rummage-4.9/rummage/lib/gui/actions/sanitize_json.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/actions/updates.py` & `rummage-4.9/rummage/lib/gui/actions/updates.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/app/custom_app.py` & `rummage-4.9/rummage/lib/gui/app/custom_app.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/app/platform_window_focus.py` & `rummage-4.9/rummage/lib/gui/app/platform_window_focus.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/app/rummage_app.py` & `rummage-4.9/rummage/lib/gui/app/rummage_app.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/autocomplete_combo.py` & `rummage-4.9/rummage/lib/gui/controls/autocomplete_combo.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/collapsible_pane.py` & `rummage-4.9/rummage/lib/gui/controls/collapsible_pane.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/custom_statusbar.py` & `rummage-4.9/rummage/lib/gui/controls/custom_statusbar.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/date_picker.py` & `rummage-4.9/rummage/lib/gui/controls/date_picker.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/dynamic_lists.py` & `rummage-4.9/rummage/lib/gui/controls/dynamic_lists.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/encoding_list.py` & `rummage-4.9/rummage/lib/gui/controls/encoding_list.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/file_picker.py` & `rummage-4.9/rummage/lib/gui/controls/file_picker.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/load_search_list.py` & `rummage-4.9/rummage/lib/gui/controls/load_search_list.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/pick_button.py` & `rummage-4.9/rummage/lib/gui/controls/pick_button.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/result_lists.py` & `rummage-4.9/rummage/lib/gui/controls/result_lists.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/search_chain_list.py` & `rummage-4.9/rummage/lib/gui/controls/search_chain_list.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/search_error_list.py` & `rummage-4.9/rummage/lib/gui/controls/search_error_list.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/time_picker.py` & `rummage-4.9/rummage/lib/gui/controls/time_picker.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/controls/webview.py` & `rummage-4.9/rummage/lib/gui/controls/webview.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/__init__.py` & `rummage-4.9/rummage/lib/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/binary.png` & `rummage-4.9/rummage/lib/gui/data/binary.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/doc.png` & `rummage-4.9/rummage/lib/gui/data/doc.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/404.html` & `rummage-4.9/rummage/lib/gui/data/docs/404.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/changelog.html` & `rummage-4.9/rummage/lib/gui/data/docs/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 <body>
 
   <!-- Content -->
   <div class="markdown">
 
   <!-- Table of Content (Don't show for static sites) -->
     <h1 id="changelog">Changelog</h1>
+<h2 id="490">4.9.0</h2>
+<ul>
+<li><strong>NEW</strong>: Require <code>wcmatch</code> 5.1.0+, <code>bracex</code> 1.4.0, and <code>backrefs</code> <code>1.3.0</code> to include latest bug fixes.</li>
+</ul>
 <h2 id="480">4.8.0</h2>
 <ul>
 <li><strong>NEW</strong>: Supports installing extras via <code>pip install rummage[extras]</code>.</li>
 <li><strong>FIX</strong>: Fix for notification sound display in settings dialog.</li>
 <li><strong>FIX</strong>: Fix notification sound not playing on Linux when configured.</li>
 </ul>
 <h2 id="471">4.7.1</h2>
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
 
 
 
 
 
 
 ****** Changelog ******
+***** 4.9.0 *****
+    * NEW: Require wcmatch 5.1.0+, bracex 1.4.0, and backrefs 1.3.0 to include
+      latest bug fixes.
 ***** 4.8.0 *****
     * NEW: Supports installing extras via pip install rummage[extras].
     * FIX: Fix for notification sound display in settings dialog.
     * FIX: Fix notification sound not playing on Linux when configured.
 ***** 4.7.1 *****
     * FIX: Require wcmatch 5.0 and make adjustments to support it.
 ***** 4.7.0 *****
```

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/contributing.html` & `rummage-4.9/rummage/lib/gui/data/docs/contributing.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/css/theme.css` & `rummage-4.9/rummage/lib/gui/data/docs/css/theme.css`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/extras.html` & `rummage-4.9/rummage/lib/gui/data/docs/extras.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/chain_button.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/chain_button.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/chain_mode.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/chain_mode.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/chains.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/chains.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/content_tab.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/content_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/file_pattern.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/file_pattern.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/files_tab.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/files_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/html_export.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/html_export.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/limit_search_panel.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/limit_search_panel.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/load_search.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/load_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/plugin_input.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/plugin_input.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/plugin_toggle.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/plugin_toggle.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/regex_buttons.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/regex_buttons.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/regex_tester.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/regex_tester.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/rummage.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/rummage.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/save_search.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/save_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/search_replace_inputs.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/search_replace_inputs.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/search_replace_panel.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/search_replace_panel.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/search_tab.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/search_tab.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_backup.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_backup.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_editor.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_editor.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_encoding.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_encoding.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_export.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_export.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_general.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_general.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_history.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_history.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_import.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_import.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_notify.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_notify.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/settings_search.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/settings_search.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/thunar-basic.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/thunar-basic.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/thunar-conditions.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/thunar-conditions.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/images/thunar-custom.png` & `rummage-4.9/rummage/lib/gui/data/docs/images/thunar-custom.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/index.html` & `rummage-4.9/rummage/lib/gui/data/docs/index.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/installation.html` & `rummage-4.9/rummage/lib/gui/data/docs/installation.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/license.html` & `rummage-4.9/rummage/lib/gui/data/docs/license.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
   <!-- Content -->
   <div class="markdown">
 
   <!-- Table of Content (Don't show for static sites) -->
     <h1 id="license">License</h1>
 <p>MIT license.</p>
-<p>Copyright &copy; 2013 - 2019 Isaac Muse <a href="&#109;&#97;&#105;&#108;&#116;&#111;&#58;&#105;&#115;&#97;&#97;&#99;&#109;&#117;&#115;&#101;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">&#105;&#115;&#97;&#97;&#99;&#109;&#117;&#115;&#101;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;</a></p>
+<p>Copyright &copy; 2013 - 2020 Isaac Muse <a href="&#109;&#97;&#105;&#108;&#116;&#111;&#58;&#105;&#115;&#97;&#97;&#99;&#109;&#117;&#115;&#101;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;">&#105;&#115;&#97;&#97;&#99;&#109;&#117;&#115;&#101;&#64;&#103;&#109;&#97;&#105;&#108;&#46;&#99;&#111;&#109;</a></p>
 <p>Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:</p>
 <p>The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.</p>
 <p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.</p>
 <hr />
 <p>Internal documentation includes use of <a href="https://fontawesome.com/v4.7.0/">Font Awesome 4.7 by Dave Gandy</a>. Only a subset of the icons are actually distributed with Rummage. The subset of icons was generated by <a href="http://fontello.com/">Fontello</a>.</p>
 <p>The Font Awesome font is licensed under the <a href="http://scripts.sil.org/OFL">SIL OFL 1.1</a></p>
   </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 ****** License ******
 MIT license.
-Copyright © 2013 - 2019 Isaac Muse isaacmuse@gmail.com
+Copyright © 2013 - 2020 Isaac Muse isaacmuse@gmail.com
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/preferences.html` & `rummage-4.9/rummage/lib/gui/data/docs/preferences.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/search.html` & `rummage-4.9/rummage/lib/gui/data/docs/search.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/sitemap.html` & `rummage-4.9/rummage/lib/gui/data/docs/sitemap.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/docs/usage.html` & `rummage-4.9/rummage/lib/gui/data/docs/usage.html`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/error.png` & `rummage-4.9/rummage/lib/gui/data/error.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/glass.png` & `rummage-4.9/rummage/lib/gui/data/glass.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/results.css` & `rummage-4.9/rummage/lib/gui/data/results.css`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage.icns` & `rummage-4.9/rummage/lib/gui/data/rummage.icns`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage.ico` & `rummage-4.9/rummage/lib/gui/data/rummage.ico`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage.png` & `rummage-4.9/rummage/lib/gui/data/rummage.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage_dialog.png` & `rummage-4.9/rummage/lib/gui/data/rummage_dialog.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage_hires.png` & `rummage-4.9/rummage/lib/gui/data/rummage_hires.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage_large.png` & `rummage-4.9/rummage/lib/gui/data/rummage_large.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage_medium.png` & `rummage-4.9/rummage/lib/gui/data/rummage_medium.png`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/rummage_tray.ico` & `rummage-4.9/rummage/lib/gui/data/rummage_tray.ico`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/data/sorttable.js` & `rummage-4.9/rummage/lib/gui/data/sorttable.js`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/checksum_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/checksum_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/column_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/column_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/delete_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/delete_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/edit_search_chain_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/edit_search_chain_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/error_text_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/error_text_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/export_settings_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/export_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/file_ext_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/file_ext_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/generic_dialogs.py` & `rummage-4.9/rummage/lib/gui/dialogs/generic_dialogs.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/html_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/html_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/import_settings_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/import_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/load_search_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/load_search_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/msg_dialogs.py` & `rummage-4.9/rummage/lib/gui/dialogs/msg_dialogs.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/overwrite_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/overwrite_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/regex_test_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/regex_test_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/rummage_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/rummage_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/save_search_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/save_search_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/search_chain_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/search_chain_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/search_error_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/search_error_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/settings_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/dialogs/support_info_dialog.py` & `rummage-4.9/rummage/lib/gui/dialogs/support_info_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             "rummage": format_version(__meta__, "__version__"),
             "status": __meta__.__status__,
             "py_type": platform.python_implementation()
         }
 
         try:
             import backrefs
-            info["backrefs"] = format_version(backrefs, 'version')
+            info["backrefs"] = format_version(backrefs, '__version__')
         except Exception:
             info["backrefs"] = 'Version could not be acquired!'
 
         try:
             import bracex
             info["bracex"] = format_version(bracex, '__version__')
         except Exception:
```

### Comparing `rummage-4.8/rummage/lib/gui/gui.py` & `rummage-4.9/rummage/lib/gui/gui.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/localization/__init__.py` & `rummage-4.9/rummage/lib/gui/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/rummage.po` & `rummage-4.9/rummage/lib/gui/localization/locale/en_US/LC_MESSAGES/rummage.po`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/rummage.po` & `rummage-4.9/rummage/lib/gui/localization/locale/ru_RU/LC_MESSAGES/rummage.po`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/__init__.py` & `rummage-4.9/rummage/lib/gui/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/notify_growl.py` & `rummage-4.9/rummage/lib/gui/notify/notify_growl.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/notify_linux.py` & `rummage-4.9/rummage/lib/gui/notify/notify_linux.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/notify_osx.py` & `rummage-4.9/rummage/lib/gui/notify/notify_osx.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/notify_windows.py` & `rummage-4.9/rummage/lib/gui/notify/notify_windows.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/notify/util.py` & `rummage-4.9/rummage/lib/gui/notify/util.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/settings/__init__.py` & `rummage-4.9/rummage/lib/gui/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/util/__init__.py` & `rummage-4.9/rummage/lib/gui/util/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/util/images.py` & `rummage-4.9/rummage/lib/gui/util/images.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/util/png.py` & `rummage-4.9/rummage/lib/gui/util/png.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/gui/util/rgba.py` & `rummage-4.9/rummage/lib/gui/util/rgba.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/rumcore/__init__.py` & `rummage-4.9/rummage/lib/rumcore/__init__.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/rumcore/text_decode.py` & `rummage-4.9/rummage/lib/rumcore/text_decode.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage/lib/rumcore/util.py` & `rummage-4.9/rummage/lib/rumcore/util.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/rummage.egg-info/PKG-INFO` & `rummage-4.9/rummage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: rummage
-Version: 4.8
+Version: 4.9
 Summary: A GUI search and replace app.
 Home-page: https://github.com/facelessuser/Rummage
 Author: Isaac Muse
 Author-email: Isaac.Muse@gmail.com
 License: MIT License
-Description: [![Build][github-ci-image]][github-ci-link]
+Description: [![Gitter][gitter-image]][gitter-link]
+        [![Build][github-ci-image]][github-ci-link]
         [![Unix Build Status][travis-image]][travis-link]
         [![Windows Build Status][appveyor-image]][appveyor-link]
         [![Coverage][codecov-image]][codecov-link]
-        [![Requirements Status][requires-image]][requires-link]
         [![PyPI Version][pypi-image]][pypi-link]
+        [![PyPI - Python Version][python-image]][pypi-link]
         ![License][license-image-mit]
         
         Rummage
         =======
         
         Rummage is a cross platform search and replace tool. Rummage crawls directories and searches for specified patterns (either regular expression or literal) and can optionally replace those targets with desired text.
         
@@ -27,42 +28,43 @@
         
         ![Rummage Files](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/files_tab.png)
         
         ![Rummage Content](https://github.com/facelessuser/Rummage/raw/master/docs/src/markdown/images/content_tab.png)
         
         # Documentation
         
-        http://facelessuser.github.io/Rummage/
+        https://facelessuser.github.io/Rummage/
         
         License
         =======
         
         Rummage is released under the MIT license.
         
-        Copyright (c) 2013 - 2019 Isaac Muse <isaacmuse@gmail.com>
+        Copyright (c) 2013 - 2020 Isaac Muse <isaacmuse@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         [github-ci-image]: https://github.com/facelessuser/Rummage/workflows/build/badge.svg
         [github-ci-link]: https://github.com/facelessuser/Rummage/actions?workflow=build
-        [travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=Unix%20Build
+        [travis-image]: https://img.shields.io/travis/facelessuser/Rummage/master.svg?label=travis&logo=travis%20ci&logoColor=cccccc
         [travis-link]: https://travis-ci.org/facelessuser/Rummage
-        [appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=Windows%20Build
+        [appveyor-image]: https://img.shields.io/appveyor/ci/facelessuser/Rummage/master.svg?label=appveyor&logo=appveyor&logoColor=cccccc
         [appveyor-link]: https://ci.appveyor.com/project/facelessuser/Rummage
         [license-image]: https://img.shields.io/badge/license-MIT-blue.svg
-        [codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg
+        [codecov-image]: https://img.shields.io/codecov/c/github/facelessuser/Rummage/master.svg?logo=codecov&logoColor=cccccc
         [codecov-link]: http://codecov.io/github/facelessuser/Rummage?branch=master
-        [requires-image]: https://img.shields.io/requires/github/facelessuser/Rummage/master.svg
-        [requires-link]: https://requires.io/github/facelessuser/Rummage/requirements/?branch=master
-        [pypi-image]: https://img.shields.io/pypi/v/Rummage.svg
+        [gitter-image]: https://img.shields.io/gitter/room/facelessuser/Rummage.svg?logo=gitter&color=fuchsia&logoColor=cccccc
+        [gitter-link]: https://gitter.im/facelessuser/Rummage
+        [pypi-image]: https://img.shields.io/pypi/v/Rummage.svg?logo=pypi&logoColor=cccccc
         [pypi-link]: https://pypi.python.org/pypi/Rummage
+        [python-image]: https://img.shields.io/pypi/pyversions/Rummage?logo=python&logoColor=cccccc
         [license-image-mit]: https://img.shields.io/badge/license-MIT-blue.svg
         
 Keywords: grep search find replace gui
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rummage-4.8/rummage.egg-info/SOURCES.txt` & `rummage-4.9/rummage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rummage-4.8/setup.cfg` & `rummage-4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `rummage-4.8/setup.py` & `rummage-4.9/setup.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tests/test_rumcore.py` & `rummage-4.9/tests/test_rumcore.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tests/test_text_decode.py` & `rummage-4.9/tests/test_text_decode.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tests/test_versions.py` & `rummage-4.9/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tests/util.py` & `rummage-4.9/tests/util.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tools/gen_docs.py` & `rummage-4.9/tools/gen_docs.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tools/gui_patch.py` & `rummage-4.9/tools/gui_patch.py`

 * *Files identical despite different names*

### Comparing `rummage-4.8/tox.ini` & `rummage-4.9/tox.ini`

 * *Files identical despite different names*

