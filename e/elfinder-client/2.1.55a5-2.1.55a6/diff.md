# Comparing `tmp/elfinder-client-2.1.55a5.tar.gz` & `tmp/elfinder-client-2.1.55a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elfinder-client-2.1.55a5.tar", last modified: Sun Apr 19 14:22:00 2020, max compression
+gzip compressed data, was "dist/elfinder-client-2.1.55a6.tar", last modified: Sun Apr 19 14:40:30 2020, max compression
```

## Comparing `elfinder-client-2.1.55a5.tar` & `elfinder-client-2.1.55a6.tar`

### file list

```diff
@@ -1,188 +1,189 @@
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1525 2020-04-18 23:04:15.000000 elfinder-client-2.1.55a5/LICENSE.md
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      109 2020-04-19 11:47:46.000000 elfinder-client-2.1.55a5/MANIFEST.in
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      273 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/PKG-INFO
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    10174 2020-04-18 23:06:42.000000 elfinder-client-2.1.55a5/README.md
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    63979 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/Changelog
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1525 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/LICENSE.md
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    10174 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/README.md
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      344 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/__init__.py
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1328 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/composer.json
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/css/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)   124509 2020-04-19 14:21:49.000000 elfinder-client-2.1.55a5/elfinder_client/css/elfinder.full.css
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    96055 2020-04-19 14:21:49.000000 elfinder-client-2.1.55a5/elfinder_client/css/elfinder.min.css
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    12073 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/css/theme.css
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3574 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/elfinder.html
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3138 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/elfinder.legacy.html
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/files/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        2 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/files/.gitignore
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/files/.trash/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        2 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/files/.trash/.gitignore
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/img/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      152 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/arrows-active.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      169 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/arrows-normal.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      323 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/crop.gif
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     5818 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/dialogs.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2719 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/editor-icons.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6880 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/icons-big.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    26458 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/icons-big.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3674 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/icons-small.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4893 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/logo.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      667 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/progress.gif
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       71 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/quicklook-bg.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1604 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/quicklook-icons.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       83 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/resize.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1434 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/spinner-mini.gif
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     7506 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/toolbar.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      164 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/trashmesh.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    20133 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-a.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-b.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-c.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-d.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3759 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/ui-icons_ffffff_256x240.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      621 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_box.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      686 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_box.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      413 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_dropbox.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      312 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_dropbox.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      371 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_ftp.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    11329 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_ftp.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      663 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_googledrive.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      223 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_googledrive.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      357 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_local.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    16208 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_local.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      872 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_network.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    13092 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_network.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      204 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_onedrive.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      505 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_onedrive.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      572 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_sql.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     9275 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_sql.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      706 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_trash.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     7318 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_trash.svg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      475 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_zip.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     8954 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_zip.svg
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)  1053430 2020-04-19 14:21:49.000000 elfinder-client-2.1.55a5/elfinder_client/js/elfinder.full.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)   544163 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/elfinder.min.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/extras/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    83441 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/extras/editors.default.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    46010 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/extras/editors.default.min.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2305 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/extras/quicklook.googledocs.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1575 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/extras/quicklook.googledocs.min.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    32640 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.LANG.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    30529 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ar.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    40582 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.bg.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    16767 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ca.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    34214 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.cs.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    16034 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.da.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    34492 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.de.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    21599 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.el.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    31884 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.es.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    33786 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fa.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      235 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fallback.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    19695 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fo.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    35217 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fr.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    35373 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fr_CA.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    18944 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.he.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    20678 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.hr.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    22321 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.hu.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    26603 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.id.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    31973 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.it.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    38989 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ja.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    35771 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ko.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    35813 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.nl.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    15982 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.no.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    34436 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.pl.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    34548 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.pt_BR.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    20243 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ro.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    42490 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ru.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    44135 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.si.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    34915 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sk.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    16167 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sl.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    16075 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sr.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    15753 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sv.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    33498 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.tr.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    20592 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ug_CN.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    42329 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.uk.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    35222 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.vi.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    32332 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.zh_CN.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    27201 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.zh_TW.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      978 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/cs.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2296 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/de.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      800 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/en.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1058 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/es.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1282 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ja.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1052 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ko.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1031 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/pl.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1605 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ru.html.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      997 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/sk.html.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/proxy/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    10092 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/proxy/elFinderSupportVer1.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/js/worker/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      532 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/worker/calcfilehash.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      330 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/worker/quicklook.tiff.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1844 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/js/worker/quicklook.unzip.js
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6495 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/main.default.js
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/.tmp/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       31 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/.tmp/.htaccess
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2316 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/MySQLStorage.sql
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2598 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/autoload.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    17685 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/connector.maximal.php-dist
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     9201 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/connector.minimal.php-dist
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/OnlineConvert/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     4304 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/OnlineConvert/editor.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/ZipArchive/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      401 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/ZipArchive/editor.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/ZohoOffice/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     8607 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/ZohoOffice/editor.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1418 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/editors/editor.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)   181575 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinder.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    12549 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderConnector.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    15177 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderFlysystemGoogleDriveNetmount.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3331 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderPlugin.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     8789 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderSession.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1094 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderSessionInterface.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    61762 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeBox.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)   260129 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeDriver.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    47420 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeDropbox2.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    58448 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeFTP.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    71249 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeGoogleDrive.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     5371 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeGroup.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    46722 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeLocalFileSystem.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    30056 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeMySQL.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    67804 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeOneDrive.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1583 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeTrash.class.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     1576 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeTrashMySQL.class.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/libs/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    20186 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/libs/GdBmp.php
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    24832 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/mime.types
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoResize/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6964 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoResize/plugin.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoRotate/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     5610 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoRotate/plugin.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Normalizer/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     8027 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Normalizer/plugin.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Sanitizer/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     5901 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Sanitizer/plugin.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Watermark/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     8931 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Watermark/logo.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    18240 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/plugins/Watermark/plugin.php
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/php/resources/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     3626 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/resources/image.png
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     2289 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/php/resources/video.png
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client/sounds/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)    92204 2020-04-19 14:21:52.000000 elfinder-client-2.1.55a5/elfinder_client/sounds/rm.wav
-drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      273 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/PKG-INFO
--rw-r--r--   0 wei.ouyang   (501) staff       (20)     6276 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/SOURCES.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/dependency_links.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2020-04-19 00:23:24.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/not-zip-safe
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       16 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/elfinder_client.egg-info/top_level.txt
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      722 2020-04-19 14:21:32.000000 elfinder-client-2.1.55a5/package.json
--rw-r--r--   0 wei.ouyang   (501) staff       (20)       38 2020-04-19 14:22:00.000000 elfinder-client-2.1.55a5/setup.cfg
--rw-r--r--   0 wei.ouyang   (501) staff       (20)      642 2020-04-19 00:22:21.000000 elfinder-client-2.1.55a5/setup.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1525 2020-04-18 23:04:15.000000 elfinder-client-2.1.55a6/LICENSE.md
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      109 2020-04-19 11:47:46.000000 elfinder-client-2.1.55a6/MANIFEST.in
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      273 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    10174 2020-04-18 23:06:42.000000 elfinder-client-2.1.55a6/README.md
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    63979 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/Changelog
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1525 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/LICENSE.md
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    10174 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/README.md
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      541 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1328 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/composer.json
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/css/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)   124509 2020-04-19 14:40:20.000000 elfinder-client-2.1.55a6/elfinder_client/css/elfinder.full.css
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    96055 2020-04-19 14:40:21.000000 elfinder-client-2.1.55a6/elfinder_client/css/elfinder.min.css
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    12073 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/css/theme.css
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3574 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/elfinder.html
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3138 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/elfinder.legacy.html
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/files/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        2 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/files/.gitignore
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/files/.trash/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        2 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/files/.trash/.gitignore
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/img/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      152 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/arrows-active.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      169 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/arrows-normal.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      323 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/crop.gif
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     5818 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/dialogs.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2719 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/editor-icons.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6880 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/icons-big.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    26458 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/icons-big.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3674 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/icons-small.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4893 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/logo.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      667 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/progress.gif
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       71 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/quicklook-bg.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1604 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/quicklook-icons.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       83 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/resize.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1434 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/spinner-mini.gif
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     7506 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/toolbar.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      164 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/trashmesh.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    20133 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-a.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-b.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-c.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    19744 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-d.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3759 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      621 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_box.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      686 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_box.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      413 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_dropbox.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      312 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_dropbox.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      371 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_ftp.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    11329 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_ftp.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      663 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_googledrive.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      223 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_googledrive.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      357 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_local.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    16208 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_local.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      872 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_network.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    13092 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_network.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      204 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_onedrive.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      505 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_onedrive.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      572 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_sql.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     9275 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_sql.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      706 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_trash.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     7318 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_trash.svg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      475 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_zip.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8954 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_zip.svg
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)  1053430 2020-04-19 14:40:21.000000 elfinder-client-2.1.55a6/elfinder_client/js/elfinder.full.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)   544163 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/elfinder.min.js
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/extras/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    83441 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/extras/editors.default.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    46010 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/extras/editors.default.min.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2305 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/extras/quicklook.googledocs.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1575 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/extras/quicklook.googledocs.min.js
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    32640 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.LANG.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    30529 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ar.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    40582 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.bg.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    16767 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ca.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    34214 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.cs.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    16034 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.da.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    34492 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.de.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    21599 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.el.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    31884 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.es.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    33786 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fa.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      235 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fallback.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    19695 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fo.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    35217 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fr.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    35373 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fr_CA.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    18944 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.he.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    20678 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.hr.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    22321 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.hu.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    26603 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.id.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    31973 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.it.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    38989 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ja.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    35771 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ko.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    35813 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.nl.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    15982 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.no.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    34436 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.pl.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    34548 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.pt_BR.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    20243 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ro.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    42490 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ru.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    44135 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.si.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    34915 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sk.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    16167 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sl.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    16075 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sr.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    15753 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sv.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    33498 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.tr.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    20592 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ug_CN.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    42329 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.uk.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    35222 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.vi.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    32332 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.zh_CN.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    27201 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.zh_TW.js
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      978 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/cs.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2296 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/de.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      800 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/en.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1058 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/es.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1282 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ja.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1052 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ko.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1031 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/pl.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1605 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ru.html.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      997 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/sk.html.js
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/proxy/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    10092 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/proxy/elFinderSupportVer1.js
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/js/worker/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      532 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/worker/calcfilehash.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      330 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/worker/quicklook.tiff.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1844 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/js/worker/quicklook.unzip.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6495 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/main.default.js
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      722 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/package.json
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/.tmp/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       31 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/.tmp/.htaccess
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2316 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/MySQLStorage.sql
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2598 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/autoload.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    17685 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/connector.maximal.php-dist
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     9201 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/connector.minimal.php-dist
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/OnlineConvert/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     4304 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/OnlineConvert/editor.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/ZipArchive/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      401 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/ZipArchive/editor.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/ZohoOffice/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8607 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/ZohoOffice/editor.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1418 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/editors/editor.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)   181575 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinder.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    12549 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderConnector.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    15177 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderFlysystemGoogleDriveNetmount.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3331 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderPlugin.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8789 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderSession.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1094 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderSessionInterface.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    61762 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeBox.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)   260129 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeDriver.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    47420 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeDropbox2.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    58448 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeFTP.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    71249 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeGoogleDrive.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     5371 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeGroup.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    46722 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeLocalFileSystem.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    30056 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeMySQL.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    67804 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeOneDrive.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1583 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeTrash.class.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1576 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeTrashMySQL.class.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/libs/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    20186 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/libs/GdBmp.php
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    24832 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/mime.types
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoResize/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6964 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoResize/plugin.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoRotate/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     5610 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoRotate/plugin.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Normalizer/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8027 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Normalizer/plugin.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Sanitizer/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     5901 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Sanitizer/plugin.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Watermark/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8931 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Watermark/logo.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    18240 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/plugins/Watermark/plugin.php
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/php/resources/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     3626 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/resources/image.png
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2289 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/php/resources/video.png
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client/sounds/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    92204 2020-04-19 14:40:23.000000 elfinder-client-2.1.55a6/elfinder_client/sounds/rm.wav
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      273 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     6305 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/SOURCES.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/dependency_links.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2020-04-19 00:23:24.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/not-zip-safe
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       16 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/elfinder_client.egg-info/top_level.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      722 2020-04-19 14:40:15.000000 elfinder-client-2.1.55a6/package.json
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       38 2020-04-19 14:40:30.000000 elfinder-client-2.1.55a6/setup.cfg
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      642 2020-04-19 00:22:21.000000 elfinder-client-2.1.55a6/setup.py
```

### Comparing `elfinder-client-2.1.55a5/LICENSE.md` & `elfinder-client-2.1.55a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/README.md` & `elfinder-client-2.1.55a6/README.md`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/Changelog` & `elfinder-client-2.1.55a6/elfinder_client/Changelog`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/LICENSE.md` & `elfinder-client-2.1.55a6/elfinder_client/LICENSE.md`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/README.md` & `elfinder-client-2.1.55a6/elfinder_client/README.md`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/composer.json` & `elfinder-client-2.1.55a6/elfinder_client/composer.json`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/css/elfinder.full.css` & `elfinder-client-2.1.55a6/elfinder_client/css/elfinder.full.css`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/css/elfinder.min.css` & `elfinder-client-2.1.55a6/elfinder_client/css/elfinder.min.css`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/css/theme.css` & `elfinder-client-2.1.55a6/elfinder_client/css/theme.css`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/elfinder.html` & `elfinder-client-2.1.55a6/elfinder_client/elfinder.html`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/elfinder.legacy.html` & `elfinder-client-2.1.55a6/elfinder_client/elfinder.legacy.html`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/dialogs.png` & `elfinder-client-2.1.55a6/elfinder_client/img/dialogs.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/editor-icons.png` & `elfinder-client-2.1.55a6/elfinder_client/img/editor-icons.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/icons-big.png` & `elfinder-client-2.1.55a6/elfinder_client/img/icons-big.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/icons-big.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/icons-big.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/icons-small.png` & `elfinder-client-2.1.55a6/elfinder_client/img/icons-small.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/logo.png` & `elfinder-client-2.1.55a6/elfinder_client/img/logo.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/progress.gif` & `elfinder-client-2.1.55a6/elfinder_client/img/progress.gif`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/quicklook-icons.png` & `elfinder-client-2.1.55a6/elfinder_client/img/quicklook-icons.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/spinner-mini.gif` & `elfinder-client-2.1.55a6/elfinder_client/img/spinner-mini.gif`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/toolbar.png` & `elfinder-client-2.1.55a6/elfinder_client/img/toolbar.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-a.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-a.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-b.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-b.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-c.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-c.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/tui-icon-d.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/tui-icon-d.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/ui-icons_ffffff_256x240.png` & `elfinder-client-2.1.55a6/elfinder_client/img/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_box.png` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_box.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_box.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_box.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_ftp.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_ftp.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_googledrive.png` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_googledrive.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_local.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_local.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_network.png` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_network.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_network.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_network.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_sql.png` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_sql.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_sql.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_sql.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_trash.png` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_trash.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_trash.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_trash.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/img/volume_icon_zip.svg` & `elfinder-client-2.1.55a6/elfinder_client/img/volume_icon_zip.svg`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/elfinder.full.js` & `elfinder-client-2.1.55a6/elfinder_client/js/elfinder.full.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/elfinder.min.js` & `elfinder-client-2.1.55a6/elfinder_client/js/elfinder.min.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/extras/editors.default.js` & `elfinder-client-2.1.55a6/elfinder_client/js/extras/editors.default.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/extras/editors.default.min.js` & `elfinder-client-2.1.55a6/elfinder_client/js/extras/editors.default.min.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/extras/quicklook.googledocs.js` & `elfinder-client-2.1.55a6/elfinder_client/js/extras/quicklook.googledocs.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/extras/quicklook.googledocs.min.js` & `elfinder-client-2.1.55a6/elfinder_client/js/extras/quicklook.googledocs.min.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.LANG.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.LANG.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ar.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ar.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.bg.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.bg.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ca.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ca.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.cs.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.cs.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.da.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.da.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.de.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.de.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.el.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.el.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.es.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.es.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fa.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fa.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fo.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fo.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fr.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fr.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.fr_CA.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.fr_CA.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.he.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.he.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.hr.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.hr.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.hu.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.hu.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.id.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.id.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.it.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.it.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ja.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ja.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ko.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ko.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.nl.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.nl.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.no.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.no.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.pl.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.pl.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.pt_BR.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.pt_BR.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ro.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ro.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ru.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ru.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.si.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.si.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sk.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sk.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sl.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sl.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sr.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sr.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.sv.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.sv.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.tr.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.tr.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.ug_CN.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.ug_CN.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.uk.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.uk.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.vi.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.vi.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.zh_CN.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.zh_CN.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/elfinder.zh_TW.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/elfinder.zh_TW.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/cs.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/cs.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/de.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/de.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/en.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/en.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/es.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/es.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ja.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ja.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ko.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ko.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/pl.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/pl.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/ru.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/ru.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/i18n/help/sk.html.js` & `elfinder-client-2.1.55a6/elfinder_client/js/i18n/help/sk.html.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/proxy/elFinderSupportVer1.js` & `elfinder-client-2.1.55a6/elfinder_client/js/proxy/elFinderSupportVer1.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/worker/calcfilehash.js` & `elfinder-client-2.1.55a6/elfinder_client/js/worker/calcfilehash.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/js/worker/quicklook.unzip.js` & `elfinder-client-2.1.55a6/elfinder_client/js/worker/quicklook.unzip.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/main.default.js` & `elfinder-client-2.1.55a6/elfinder_client/main.default.js`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/MySQLStorage.sql` & `elfinder-client-2.1.55a6/elfinder_client/php/MySQLStorage.sql`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/autoload.php` & `elfinder-client-2.1.55a6/elfinder_client/php/autoload.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/connector.maximal.php-dist` & `elfinder-client-2.1.55a6/elfinder_client/php/connector.maximal.php-dist`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/connector.minimal.php-dist` & `elfinder-client-2.1.55a6/elfinder_client/php/connector.minimal.php-dist`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/editors/OnlineConvert/editor.php` & `elfinder-client-2.1.55a6/elfinder_client/php/editors/OnlineConvert/editor.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/editors/ZohoOffice/editor.php` & `elfinder-client-2.1.55a6/elfinder_client/php/editors/ZohoOffice/editor.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/editors/editor.php` & `elfinder-client-2.1.55a6/elfinder_client/php/editors/editor.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinder.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinder.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderConnector.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderConnector.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderFlysystemGoogleDriveNetmount.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderFlysystemGoogleDriveNetmount.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderPlugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderPlugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderSession.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderSession.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderSessionInterface.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderSessionInterface.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeBox.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeBox.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeDriver.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeDriver.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeDropbox2.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeDropbox2.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeFTP.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeFTP.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeGoogleDrive.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeGoogleDrive.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeGroup.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeGroup.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeLocalFileSystem.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeLocalFileSystem.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeMySQL.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeMySQL.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeOneDrive.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeOneDrive.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeTrash.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeTrash.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/elFinderVolumeTrashMySQL.class.php` & `elfinder-client-2.1.55a6/elfinder_client/php/elFinderVolumeTrashMySQL.class.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/libs/GdBmp.php` & `elfinder-client-2.1.55a6/elfinder_client/php/libs/GdBmp.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/mime.types` & `elfinder-client-2.1.55a6/elfinder_client/php/mime.types`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoResize/plugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoResize/plugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/AutoRotate/plugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/AutoRotate/plugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/Normalizer/plugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/Normalizer/plugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/Sanitizer/plugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/Sanitizer/plugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/Watermark/logo.png` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/Watermark/logo.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/plugins/Watermark/plugin.php` & `elfinder-client-2.1.55a6/elfinder_client/php/plugins/Watermark/plugin.php`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/resources/image.png` & `elfinder-client-2.1.55a6/elfinder_client/php/resources/image.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/php/resources/video.png` & `elfinder-client-2.1.55a6/elfinder_client/php/resources/video.png`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client/sounds/rm.wav` & `elfinder-client-2.1.55a6/elfinder_client/sounds/rm.wav`

 * *Files identical despite different names*

### Comparing `elfinder-client-2.1.55a5/elfinder_client.egg-info/SOURCES.txt` & `elfinder-client-2.1.55a6/elfinder_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 elfinder_client/LICENSE.md
 elfinder_client/README.md
 elfinder_client/__init__.py
 elfinder_client/composer.json
 elfinder_client/elfinder.html
 elfinder_client/elfinder.legacy.html
 elfinder_client/main.default.js
+elfinder_client/package.json
 elfinder_client.egg-info/PKG-INFO
 elfinder_client.egg-info/SOURCES.txt
 elfinder_client.egg-info/dependency_links.txt
 elfinder_client.egg-info/not-zip-safe
 elfinder_client.egg-info/top_level.txt
 elfinder_client/css/elfinder.full.css
 elfinder_client/css/elfinder.min.css
```

### Comparing `elfinder-client-2.1.55a5/package.json` & `elfinder-client-2.1.55a6/elfinder_client/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'2.1.55a6'"}*

```diff
@@ -25,9 +25,9 @@
     "repository": {
         "type": "git",
         "url": "https://github.com/Studio-42/elFinder.git"
     },
     "scripts": {
         "build": "mkdir -p ./elfinder_client && jake -C ./elfinder_client elfinder"
     },
-    "version": "2.1.55a5"
+    "version": "2.1.55a6"
 }
```

### Comparing `elfinder-client-2.1.55a5/setup.py` & `elfinder-client-2.1.55a6/setup.py`

 * *Files identical despite different names*

