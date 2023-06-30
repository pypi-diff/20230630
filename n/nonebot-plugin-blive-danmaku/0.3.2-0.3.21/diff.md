# Comparing `tmp/nonebot_plugin_blive_danmaku-0.3.2.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.3.21.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.3.2.tar` & `nonebot_plugin_blive_danmaku-0.3.21.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.2/LICENSE
--rw-r--r--   0        0        0      938 2023-06-12 10:18:14.127750 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/__init__.py
--rw-r--r--   0        0        0       91 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
--rw-r--r--   0        0        0   533008 2023-06-26 02:58:12.791659 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
--rw-r--r--   0        0        0   285956 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
--rw-r--r--   0        0        0   324265 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
--rw-r--r--   0        0        0     9045 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
--rw-r--r--   0        0        0     8799 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
--rw-r--r--   0        0        0     7006 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
--rw-r--r--   0        0        0      902 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
--rw-r--r--   0        0        0     6723 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js
--rw-r--r--   0        0        0     2787 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js
--rw-r--r--   0        0        0    20588 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js
--rw-r--r--   0        0        0     9107 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
--rw-r--r--   0        0        0      703 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
--rw-r--r--   0        0        0     3061 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
--rw-r--r--   0        0        0      815 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
--rw-r--r--   0        0        0     5128 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js
--rw-r--r--   0        0        0      167 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
--rw-r--r--   0        0        0      699 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
--rw-r--r--   0        0        0     3593 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js
--rw-r--r--   0        0        0     1239 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js
--rw-r--r--   0        0        0       51 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-fe1a4f18.css
--rw-r--r--   0        0        0    20126 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
--rw-r--r--   0        0        0     6259 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
--rw-r--r--   0        0        0     5886 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
--rw-r--r--   0        0        0    20334 2023-06-26 02:58:12.784659 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
--rw-r--r--   0        0        0      330 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
--rw-r--r--   0        0        0    18870 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js
--rw-r--r--   0        0        0     1757 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
--rw-r--r--   0        0        0   447924 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
--rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
--rw-r--r--   0        0        0      908 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/index.html
--rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/models.py
--rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/router.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     7552 2023-06-22 11:19:57.567827 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/listener/__init__.py
--rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/listener/kick.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     7816 2023-06-30 02:55:31.194002 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     9884 2023-06-30 02:57:46.146679 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     2750 2023-06-24 02:54:45.822615 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      999 2023-06-30 03:11:23.844505 nonebot_plugin_blive_danmaku-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5599 2023-06-24 09:07:18.310064 nonebot_plugin_blive_danmaku-0.3.2/README.md
--rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.3.21/LICENSE
+-rw-r--r--   0        0        0     1362 2023-06-30 05:23:36.765411 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-28 07:50:38.274424 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/_plugin-vue_export-helper-1b428a4d.js
+-rw-r--r--   0        0        0   533008 2023-06-26 02:58:12.791659 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js
+-rw-r--r--   0        0        0   285956 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js
+-rw-r--r--   0        0        0   324265 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css
+-rw-r--r--   0        0        0     9045 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png
+-rw-r--r--   0        0        0     8799 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png
+-rw-r--r--   0        0        0     7006 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png
+-rw-r--r--   0        0        0      902 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js
+-rw-r--r--   0        0        0     6723 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js
+-rw-r--r--   0        0        0     2787 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js
+-rw-r--r--   0        0        0    20588 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js
+-rw-r--r--   0        0        0     9107 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css
+-rw-r--r--   0        0        0      703 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css
+-rw-r--r--   0        0        0     3061 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js
+-rw-r--r--   0        0        0      815 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css
+-rw-r--r--   0        0        0     5128 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js
+-rw-r--r--   0        0        0      167 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-cd2e8127.css
+-rw-r--r--   0        0        0      699 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css
+-rw-r--r--   0        0        0     3593 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js
+-rw-r--r--   0        0        0     1239 2023-06-26 02:58:12.787659 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js
+-rw-r--r--   0        0        0       51 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-fe1a4f18.css
+-rw-r--r--   0        0        0    20126 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js
+-rw-r--r--   0        0        0     6259 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png
+-rw-r--r--   0        0        0     5886 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png
+-rw-r--r--   0        0        0    20334 2023-06-26 02:58:12.784659 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png
+-rw-r--r--   0        0        0      330 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-8f8a299b.css
+-rw-r--r--   0        0        0    18870 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js
+-rw-r--r--   0        0        0     1757 2023-06-26 02:58:12.786658 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css
+-rw-r--r--   0        0        0   447924 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js
+-rw-r--r--   0        0        0    12014 2023-04-15 02:38:23.791948 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico
+-rw-r--r--   0        0        0      908 2023-06-26 02:58:12.790656 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/index.html
+-rw-r--r--   0        0        0      200 2023-06-04 10:26:16.056985 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/models.py
+-rw-r--r--   0        0        0     4864 2023-06-24 03:21:58.563784 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/router.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     7552 2023-06-22 11:19:57.567827 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    13206 2023-06-22 11:29:10.027052 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-24 05:16:11.948995 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0      136 2023-06-07 09:20:41.977052 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        4 2023-06-07 09:03:03.288555 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/listener/__init__.py
+-rw-r--r--   0        0        0      991 2023-06-07 16:56:34.852077 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/listener/kick.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1654 2023-06-24 08:58:25.069731 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0     1198 2023-06-24 09:05:18.581398 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0     1719 2023-06-24 05:42:04.607908 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0     1704 2023-06-24 05:39:55.256327 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0      728 2023-06-04 03:13:56.120283 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_open.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     7816 2023-06-30 02:55:31.194002 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2057 2023-04-24 02:36:16.771789 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      450 2023-06-22 16:58:52.849473 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       20 2023-05-26 14:35:08.837033 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     9884 2023-06-30 02:57:46.146679 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     2750 2023-06-24 02:54:45.822615 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     4011 2023-06-22 17:11:16.482488 nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0     1000 2023-06-30 05:32:01.718055 nonebot_plugin_blive_danmaku-0.3.21/pyproject.toml
+-rw-r--r--   0        0        0     5599 2023-06-24 09:07:18.310064 nonebot_plugin_blive_danmaku-0.3.21/README.md
+-rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.3.21/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.21/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/echarts-400b5edd.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-2bbb65c2.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/elementPlus-5cfbb218.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-1-k-823c4f26.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-2-k-a0b7be7c.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/guard-3-k-3c7bacae.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/helpDialog-a1deb50e.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-10fe5420.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-1f52d48f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-3b039937.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-4d7b4401.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-54bfb553.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-6803b0c6.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-7bb2b86c.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-c1b5ef2f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-e7323967.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f24fc95e.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/index-f9e2a7e5.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/lodash-520df23f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-1-f98dcdbf.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/sc-badge-2-abaf3760.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/SC-bg-img-0e2aa755.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/SuperChat-fcb4d4cd.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-b57f6aba.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/assets/vendor-fa374c7f.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/icon/favicon.ico`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/frontend/index.html` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/frontend/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/app/router.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/app/router.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/listener/kick.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/listener/kick.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_off.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_on.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/sub/sub_open.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/sub/sub_open.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.3.21/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.3.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.3.2"
+version = "0.3.21"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/README.md` & `nonebot_plugin_blive_danmaku-0.3.21/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.3.2/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.3.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.3.2
+Version: 0.3.21
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.2
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.3.21
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

