# Comparing `tmp/stig-0.8.3a0.tar.gz` & `tmp/stig-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stig-0.8.3a0.tar", last modified: Sun Feb 25 15:24:35 2018, max compression
+gzip compressed data, was "dist/stig-0.9.0a0.tar", last modified: Mon May  7 12:26:52 2018, max compression
```

## Comparing `stig-0.8.3a0.tar` & `stig-0.9.0a0.tar`

### file list

```diff
@@ -1,130 +1,135 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/
--rw-------   0 ich       (1000) ich       (1000)       38 2018-02-25 15:24:35.000000 stig-0.8.3a0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     7635 2018-02-25 15:24:35.000000 stig-0.8.3a0/PKG-INFO
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/
--rw-------   0 ich       (1000) ich       (1000)       73 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        5 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       35 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)     7635 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     2903 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)     1532 2018-02-25 14:48:13.000000 stig-0.8.3a0/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/utils/
--rw-------   0 ich       (1000) ich       (1000)     3924 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9048 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/utils/_number.py
--rw-------   0 ich       (1000) ich       (1000)     3055 2016-11-27 14:02:38.000000 stig-0.8.3a0/stig/utils/expandtabs.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/settings/
--rw-------   0 ich       (1000) ich       (1000)    31719 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/settings/types.py
--rw-------   0 ich       (1000) ich       (1000)     6316 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/settings/types_srv.py
--rw-------   0 ich       (1000) ich       (1000)      659 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/settings/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    31599 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/settings/default.theme
--rw-------   0 ich       (1000) ich       (1000)     1998 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/settings/rcfile.py
--rw-------   0 ich       (1000) ich       (1000)    20071 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/settings/defaults.py
--rw-------   0 ich       (1000) ich       (1000)       23 2018-02-25 15:15:46.000000 stig-0.8.3a0/stig/version.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/client/
--rw-------   0 ich       (1000) ich       (1000)      818 2017-12-02 12:47:35.000000 stig-0.8.3a0/stig/client/geoip.py
--rw-------   0 ich       (1000) ich       (1000)     8020 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/api.py
--rw-------   0 ich       (1000) ich       (1000)     1318 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1214 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/errors.py
--rw-------   0 ich       (1000) ich       (1000)    24780 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/ttypes.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/client/aiotransmission/
--rw-------   0 ich       (1000) ich       (1000)    15335 2018-02-25 15:15:46.000000 stig-0.8.3a0/stig/client/aiotransmission/rpc.py
--rw-------   0 ich       (1000) ich       (1000)     5846 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/aiotransmission/api_status.py
--rw-------   0 ich       (1000) ich       (1000)      532 2016-11-27 14:02:38.000000 stig-0.8.3a0/stig/client/aiotransmission/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    45066 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/aiotransmission/api_torrent.py
--rw-------   0 ich       (1000) ich       (1000)    15836 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/aiotransmission/api_settings.py
--rw-------   0 ich       (1000) ich       (1000)    24051 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/aiotransmission/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     4745 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/convert.py
--rw-------   0 ich       (1000) ich       (1000)     2915 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/base.py
--rw-------   0 ich       (1000) ich       (1000)     6996 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/utils.py
--rw-------   0 ich       (1000) ich       (1000)     1985 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/constants.py
--rw-------   0 ich       (1000) ich       (1000)     9271 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/poll.py
--rw-------   0 ich       (1000) ich       (1000)     5800 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/trequestpool.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/client/sorters/
--rw-------   0 ich       (1000) ich       (1000)     4471 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/sorters/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     7759 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/client/sorters/tsorter.py
--rw-------   0 ich       (1000) ich       (1000)     2917 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/sorters/trksorter.py
--rw-------   0 ich       (1000) ich       (1000)     2641 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/sorters/psorter.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/client/filters/
--rw-------   0 ich       (1000) ich       (1000)     4055 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/filters/trkfilter.py
--rw-------   0 ich       (1000) ich       (1000)    15371 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/filters/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2916 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/filters/pfilter.py
--rw-------   0 ich       (1000) ich       (1000)     2457 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/filters/ffilter.py
--rw-------   0 ich       (1000) ich       (1000)     8968 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/client/filters/tfilter.py
--rw-------   0 ich       (1000) ich       (1000)      875 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3643 2017-11-20 13:43:52.000000 stig-0.8.3a0/stig/cliopts.py
--rw-------   0 ich       (1000) ich       (1000)      660 2017-11-20 14:03:23.000000 stig-0.8.3a0/stig/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     5879 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/main.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/tui/
--rw-------   0 ich       (1000) ich       (1000)    14431 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/scroll.py
--rw-------   0 ich       (1000) ich       (1000)     6946 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/urwidpatches.py
--rw-------   0 ich       (1000) ich       (1000)     8377 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/cli.py
--rw-------   0 ich       (1000) ich       (1000)    21058 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/keymap.py
--rw-------   0 ich       (1000) ich       (1000)      532 2017-10-12 13:24:18.000000 stig-0.8.3a0/stig/tui/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    10871 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/infobar.py
--rw-------   0 ich       (1000) ich       (1000)    12477 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/tabs.py
--rw-------   0 ich       (1000) ich       (1000)     6646 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/main.py
--rw-------   0 ich       (1000) ich       (1000)    12720 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/group.py
--rw-------   0 ich       (1000) ich       (1000)     3394 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/hooks.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/tui/views/
--rw-------   0 ich       (1000) ich       (1000)     2950 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/trackerlist.py
--rw-------   0 ich       (1000) ich       (1000)     4149 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/views/summary.py
--rw-------   0 ich       (1000) ich       (1000)     4845 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/plist_columns.py
--rw-------   0 ich       (1000) ich       (1000)    14427 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    12898 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/filelist.py
--rw-------   0 ich       (1000) ich       (1000)     3401 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/flist_columns.py
--rw-------   0 ich       (1000) ich       (1000)    15457 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/tlist_columns.py
--rw-------   0 ich       (1000) ich       (1000)     3312 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/views/torrentlist.py
--rw-------   0 ich       (1000) ich       (1000)     6189 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/views/trklist_columns.py
--rw-------   0 ich       (1000) ich       (1000)     1448 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/hooks.py
--rw-------   0 ich       (1000) ich       (1000)     2701 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/views/peerlist.py
--rw-------   0 ich       (1000) ich       (1000)     1723 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/views/common_columns.py
--rw-------   0 ich       (1000) ich       (1000)     8533 2017-10-12 13:24:18.000000 stig-0.8.3a0/stig/tui/theme.py
--rw-------   0 ich       (1000) ich       (1000)     8008 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/tui/logger.py
--rw-------   0 ich       (1000) ich       (1000)     4209 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/tui/table.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/commands/
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/commands/base/
--rw-------   0 ich       (1000) ich       (1000)     6889 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     3781 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/peer.py
--rw-------   0 ich       (1000) ich       (1000)     5724 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/_mixin.py
--rw-------   0 ich       (1000) ich       (1000)      532 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     4154 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/misc.py
--rw-------   0 ich       (1000) ich       (1000)     2915 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/_common.py
--rw-------   0 ich       (1000) ich       (1000)     6293 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/file.py
--rw-------   0 ich       (1000) ich       (1000)     8945 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/config.py
--rw-------   0 ich       (1000) ich       (1000)    12842 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/base/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    27556 2018-01-19 20:54:59.000000 stig-0.8.3a0/stig/commands/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/commands/cli/
--rw-------   0 ich       (1000) ich       (1000)     2507 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/cli/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     9247 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/cli/_table.py
--rw-------   0 ich       (1000) ich       (1000)     2185 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/cli/peer.py
--rw-------   0 ich       (1000) ich       (1000)     4823 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/cli/_mixin.py
--rw-------   0 ich       (1000) ich       (1000)      661 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/cli/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1779 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/cli/misc.py
--rw-------   0 ich       (1000) ich       (1000)     3802 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/cli/file.py
--rw-------   0 ich       (1000) ich       (1000)     1199 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/cli/config.py
--rw-------   0 ich       (1000) ich       (1000)     4701 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/cli/torrent.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/commands/tui/
--rw-------   0 ich       (1000) ich       (1000)     1541 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/tracker.py
--rw-------   0 ich       (1000) ich       (1000)    20465 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/tui.py
--rw-------   0 ich       (1000) ich       (1000)     1224 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/peer.py
--rw-------   0 ich       (1000) ich       (1000)    10127 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/tui/_mixin.py
--rw-------   0 ich       (1000) ich       (1000)      681 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2954 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/misc.py
--rw-------   0 ich       (1000) ich       (1000)      979 2017-12-06 14:39:06.000000 stig-0.8.3a0/stig/commands/tui/_common.py
--rw-------   0 ich       (1000) ich       (1000)     1395 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/tui/file.py
--rw-------   0 ich       (1000) ich       (1000)     1194 2018-02-08 15:43:08.000000 stig-0.8.3a0/stig/commands/tui/config.py
--rw-------   0 ich       (1000) ich       (1000)     4654 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/tui/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     2779 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/commands/utils.py
--rw-------   0 ich       (1000) ich       (1000)     3174 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/commands/guess_ui.py
--rw-------   0 ich       (1000) ich       (1000)     2467 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/hooks.py
-drwx------   0 ich       (1000) ich       (1000)        0 2018-02-25 15:24:35.000000 stig-0.8.3a0/stig/views/
--rw-------   0 ich       (1000) ich       (1000)     4818 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/views/trackerlist.py
--rw-------   0 ich       (1000) ich       (1000)     7360 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/views/summary.py
--rw-------   0 ich       (1000) ich       (1000)     3839 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/views/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     4414 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/views/filelist.py
--rw-------   0 ich       (1000) ich       (1000)    11993 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/views/torrentlist.py
--rw-------   0 ich       (1000) ich       (1000)     3595 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/views/peerlist.py
--rw-------   0 ich       (1000) ich       (1000)    17834 2018-02-25 14:48:13.000000 stig-0.8.3a0/stig/helpmgr.py
--rw-------   0 ich       (1000) ich       (1000)     3880 2017-11-25 16:29:19.000000 stig-0.8.3a0/stig/logging.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/
+-rw-------   0 ich       (1000) ich       (1000)       38 2018-05-07 12:26:52.000000 stig-0.9.0a0/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     9469 2018-05-07 12:26:52.000000 stig-0.9.0a0/PKG-INFO
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)      130 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)        5 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       35 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)     9469 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     2984 2018-05-07 12:26:51.000000 stig-0.9.0a0/stig.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)     1716 2018-04-27 14:41:53.000000 stig-0.9.0a0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/utils/
+-rw-------   0 ich       (1000) ich       (1000)     2508 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/utils/_converter.py
+-rw-------   0 ich       (1000) ich       (1000)     4207 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/utils/string.py
+-rw-------   0 ich       (1000) ich       (1000)      721 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3055 2016-11-27 14:02:38.000000 stig-0.9.0a0/stig/utils/expandtabs.py
+-rw-------   0 ich       (1000) ich       (1000)    20326 2018-05-04 13:12:59.000000 stig-0.9.0a0/stig/utils/usertypes.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/settings/
+-rw-------   0 ich       (1000) ich       (1000)     3473 2018-04-29 12:24:30.000000 stig-0.9.0a0/stig/settings/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    33664 2018-05-01 12:31:44.000000 stig-0.9.0a0/stig/settings/default.theme
+-rw-------   0 ich       (1000) ich       (1000)     1998 2017-11-25 16:29:19.000000 stig-0.9.0a0/stig/settings/rcfile.py
+-rw-------   0 ich       (1000) ich       (1000)    20807 2018-05-04 15:12:31.000000 stig-0.9.0a0/stig/settings/defaults.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/client/
+-rw-------   0 ich       (1000) ich       (1000)     1218 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/rdns.py
+-rw-------   0 ich       (1000) ich       (1000)     5259 2018-04-30 12:53:35.000000 stig-0.9.0a0/stig/client/geoip.py
+-rw-------   0 ich       (1000) ich       (1000)     7798 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/api.py
+-rw-------   0 ich       (1000) ich       (1000)     1326 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1546 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/errors.py
+-rw-------   0 ich       (1000) ich       (1000)    24724 2018-04-30 12:16:21.000000 stig-0.9.0a0/stig/client/ttypes.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/client/aiotransmission/
+-rw-------   0 ich       (1000) ich       (1000)    15116 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/aiotransmission/rpc.py
+-rw-------   0 ich       (1000) ich       (1000)     5703 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/aiotransmission/api_status.py
+-rw-------   0 ich       (1000) ich       (1000)      532 2016-11-27 14:02:38.000000 stig-0.9.0a0/stig/client/aiotransmission/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    41328 2018-05-01 14:53:44.000000 stig-0.9.0a0/stig/client/aiotransmission/api_torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    21079 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/aiotransmission/api_settings.py
+-rw-------   0 ich       (1000) ich       (1000)    24477 2018-05-03 13:01:26.000000 stig-0.9.0a0/stig/client/aiotransmission/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     3054 2018-05-03 12:34:45.000000 stig-0.9.0a0/stig/client/base.py
+-rw-------   0 ich       (1000) ich       (1000)     9447 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/utils.py
+-rw-------   0 ich       (1000) ich       (1000)     1812 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     9405 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/poll.py
+-rw-------   0 ich       (1000) ich       (1000)     5504 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/trequestpool.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/client/sorters/
+-rw-------   0 ich       (1000) ich       (1000)     3188 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/sorters/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     1402 2018-05-03 13:29:51.000000 stig-0.9.0a0/stig/client/sorters/setting.py
+-rw-------   0 ich       (1000) ich       (1000)     2833 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/sorters/peer.py
+-rw-------   0 ich       (1000) ich       (1000)     4520 2018-05-03 13:17:00.000000 stig-0.9.0a0/stig/client/sorters/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     8253 2018-05-03 13:17:51.000000 stig-0.9.0a0/stig/client/sorters/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/client/filters/
+-rw-------   0 ich       (1000) ich       (1000)     4383 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/filters/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     2986 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/filters/peer.py
+-rw-------   0 ich       (1000) ich       (1000)    15601 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/filters/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2454 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/filters/file.py
+-rw-------   0 ich       (1000) ich       (1000)     9472 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/client/filters/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     1022 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3643 2018-05-07 11:39:18.000000 stig-0.9.0a0/stig/cliopts.py
+-rw-------   0 ich       (1000) ich       (1000)       23 2018-05-04 15:12:31.000000 stig-0.9.0a0/stig/__version__.py
+-rw-------   0 ich       (1000) ich       (1000)      660 2017-11-20 14:03:23.000000 stig-0.9.0a0/stig/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     7171 2018-05-07 11:44:51.000000 stig-0.9.0a0/stig/main.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/tui/
+-rw-------   0 ich       (1000) ich       (1000)    14445 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/scroll.py
+-rw-------   0 ich       (1000) ich       (1000)     7998 2018-05-07 12:26:10.000000 stig-0.9.0a0/stig/tui/urwidpatches.py
+-rw-------   0 ich       (1000) ich       (1000)     6294 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/cli.py
+-rw-------   0 ich       (1000) ich       (1000)    21204 2018-05-04 14:06:49.000000 stig-0.9.0a0/stig/tui/keymap.py
+-rw-------   0 ich       (1000) ich       (1000)      532 2018-05-04 14:51:23.000000 stig-0.9.0a0/stig/tui/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    11729 2018-04-30 15:58:54.000000 stig-0.9.0a0/stig/tui/infobar.py
+-rw-------   0 ich       (1000) ich       (1000)    12541 2018-05-07 12:08:45.000000 stig-0.9.0a0/stig/tui/tabs.py
+-rw-------   0 ich       (1000) ich       (1000)     6934 2018-05-04 13:59:44.000000 stig-0.9.0a0/stig/tui/main.py
+-rw-------   0 ich       (1000) ich       (1000)    13057 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/group.py
+-rw-------   0 ich       (1000) ich       (1000)     4057 2018-05-01 12:42:46.000000 stig-0.9.0a0/stig/tui/hooks.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/tui/views/
+-rw-------   0 ich       (1000) ich       (1000)     6183 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     4552 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/summary.py
+-rw-------   0 ich       (1000) ich       (1000)     2206 2018-05-01 12:33:09.000000 stig-0.9.0a0/stig/tui/views/setting.py
+-rw-------   0 ich       (1000) ich       (1000)     2872 2018-04-30 12:15:32.000000 stig-0.9.0a0/stig/tui/views/peer_list.py
+-rw-------   0 ich       (1000) ich       (1000)     4919 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/peer.py
+-rw-------   0 ich       (1000) ich       (1000)    13991 2018-05-04 13:45:50.000000 stig-0.9.0a0/stig/tui/views/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3255 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/tracker_list.py
+-rw-------   0 ich       (1000) ich       (1000)    13096 2018-04-27 14:50:31.000000 stig-0.9.0a0/stig/tui/views/file_list.py
+-rw-------   0 ich       (1000) ich       (1000)     1615 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/hooks.py
+-rw-------   0 ich       (1000) ich       (1000)     1657 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/common_columns.py
+-rw-------   0 ich       (1000) ich       (1000)     3639 2018-05-04 13:41:30.000000 stig-0.9.0a0/stig/tui/views/torrent_list.py
+-rw-------   0 ich       (1000) ich       (1000)     3308 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/views/file.py
+-rw-------   0 ich       (1000) ich       (1000)    14309 2018-04-30 16:12:30.000000 stig-0.9.0a0/stig/tui/views/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     6537 2018-05-04 13:42:58.000000 stig-0.9.0a0/stig/tui/views/setting_list.py
+-rw-------   0 ich       (1000) ich       (1000)     8533 2017-10-12 13:24:18.000000 stig-0.9.0a0/stig/tui/theme.py
+-rw-------   0 ich       (1000) ich       (1000)     8013 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/tui/logger.py
+-rw-------   0 ich       (1000) ich       (1000)     4209 2017-11-25 16:29:19.000000 stig-0.9.0a0/stig/tui/table.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/commands/
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/commands/base/
+-rw-------   0 ich       (1000) ich       (1000)     6965 2018-04-30 13:02:13.000000 stig-0.9.0a0/stig/commands/base/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     3772 2018-04-30 17:03:37.000000 stig-0.9.0a0/stig/commands/base/peer.py
+-rw-------   0 ich       (1000) ich       (1000)     5699 2018-05-04 13:43:08.000000 stig-0.9.0a0/stig/commands/base/_mixin.py
+-rw-------   0 ich       (1000) ich       (1000)      532 2017-11-25 16:29:19.000000 stig-0.9.0a0/stig/commands/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     4165 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/base/misc.py
+-rw-------   0 ich       (1000) ich       (1000)     2905 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/base/_common.py
+-rw-------   0 ich       (1000) ich       (1000)     5762 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/base/file.py
+-rw-------   0 ich       (1000) ich       (1000)    14453 2018-05-07 11:58:03.000000 stig-0.9.0a0/stig/commands/base/config.py
+-rw-------   0 ich       (1000) ich       (1000)    13232 2018-05-04 13:36:52.000000 stig-0.9.0a0/stig/commands/base/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    27496 2018-05-04 15:10:12.000000 stig-0.9.0a0/stig/commands/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/commands/cli/
+-rw-------   0 ich       (1000) ich       (1000)     2496 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)    10217 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/_table.py
+-rw-------   0 ich       (1000) ich       (1000)     2403 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/peer.py
+-rw-------   0 ich       (1000) ich       (1000)     4982 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/_mixin.py
+-rw-------   0 ich       (1000) ich       (1000)      661 2018-03-05 18:39:04.000000 stig-0.9.0a0/stig/commands/cli/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1725 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/misc.py
+-rw-------   0 ich       (1000) ich       (1000)      599 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/_common.py
+-rw-------   0 ich       (1000) ich       (1000)     3998 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/file.py
+-rw-------   0 ich       (1000) ich       (1000)     2360 2018-05-01 12:23:47.000000 stig-0.9.0a0/stig/commands/cli/config.py
+-rw-------   0 ich       (1000) ich       (1000)     4561 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/cli/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/commands/tui/
+-rw-------   0 ich       (1000) ich       (1000)     1500 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)    20630 2018-05-04 14:05:37.000000 stig-0.9.0a0/stig/commands/tui/tui.py
+-rw-------   0 ich       (1000) ich       (1000)     1182 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/peer.py
+-rw-------   0 ich       (1000) ich       (1000)    11348 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/_mixin.py
+-rw-------   0 ich       (1000) ich       (1000)      680 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2954 2017-11-25 16:29:19.000000 stig-0.9.0a0/stig/commands/tui/misc.py
+-rw-------   0 ich       (1000) ich       (1000)      986 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/_common.py
+-rw-------   0 ich       (1000) ich       (1000)     1353 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/file.py
+-rw-------   0 ich       (1000) ich       (1000)     2116 2018-05-04 15:12:24.000000 stig-0.9.0a0/stig/commands/tui/config.py
+-rw-------   0 ich       (1000) ich       (1000)     3922 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/tui/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     2778 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/utils.py
+-rw-------   0 ich       (1000) ich       (1000)     3538 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/commands/guess_ui.py
+-rw-------   0 ich       (1000) ich       (1000)     4025 2018-04-30 12:37:49.000000 stig-0.9.0a0/stig/hooks.py
+drwx------   0 ich       (1000) ich       (1000)        0 2018-05-07 12:26:52.000000 stig-0.9.0a0/stig/views/
+-rw-------   0 ich       (1000) ich       (1000)     4715 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/views/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     9004 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/views/summary.py
+-rw-------   0 ich       (1000) ich       (1000)     1867 2018-05-04 13:21:54.000000 stig-0.9.0a0/stig/views/setting.py
+-rw-------   0 ich       (1000) ich       (1000)     3544 2018-04-29 11:50:13.000000 stig-0.9.0a0/stig/views/peer.py
+-rw-------   0 ich       (1000) ich       (1000)     3962 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/views/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     4267 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/views/file.py
+-rw-------   0 ich       (1000) ich       (1000)    11104 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/views/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    18025 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/helpmgr.py
+-rw-------   0 ich       (1000) ich       (1000)     3872 2018-04-27 14:41:53.000000 stig-0.9.0a0/stig/logging.py
```

### Comparing `stig-0.8.3a0/stig.egg-info/SOURCES.txt` & `stig-0.9.0a0/stig.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 setup.py
 stig/__init__.py
 stig/__main__.py
+stig/__version__.py
 stig/cliopts.py
 stig/helpmgr.py
 stig/hooks.py
 stig/logging.py
 stig/main.py
-stig/version.py
 stig.egg-info/PKG-INFO
 stig.egg-info/SOURCES.txt
 stig.egg-info/dependency_links.txt
 stig.egg-info/entry_points.txt
 stig.egg-info/requires.txt
 stig.egg-info/top_level.txt
 stig/client/__init__.py
 stig/client/api.py
 stig/client/base.py
 stig/client/constants.py
-stig/client/convert.py
 stig/client/errors.py
 stig/client/geoip.py
 stig/client/poll.py
+stig/client/rdns.py
 stig/client/trequestpool.py
 stig/client/ttypes.py
 stig/client/utils.py
 stig/client/aiotransmission/__init__.py
 stig/client/aiotransmission/api_settings.py
 stig/client/aiotransmission/api_status.py
 stig/client/aiotransmission/api_torrent.py
 stig/client/aiotransmission/rpc.py
 stig/client/aiotransmission/torrent.py
 stig/client/filters/__init__.py
-stig/client/filters/ffilter.py
-stig/client/filters/pfilter.py
-stig/client/filters/tfilter.py
-stig/client/filters/trkfilter.py
+stig/client/filters/file.py
+stig/client/filters/peer.py
+stig/client/filters/torrent.py
+stig/client/filters/tracker.py
 stig/client/sorters/__init__.py
-stig/client/sorters/psorter.py
-stig/client/sorters/trksorter.py
-stig/client/sorters/tsorter.py
+stig/client/sorters/peer.py
+stig/client/sorters/setting.py
+stig/client/sorters/torrent.py
+stig/client/sorters/tracker.py
 stig/commands/__init__.py
 stig/commands/guess_ui.py
 stig/commands/utils.py
 stig/commands/base/__init__.py
 stig/commands/base/_common.py
 stig/commands/base/_mixin.py
 stig/commands/base/config.py
 stig/commands/base/file.py
 stig/commands/base/misc.py
 stig/commands/base/peer.py
 stig/commands/base/torrent.py
 stig/commands/base/tracker.py
 stig/commands/cli/__init__.py
+stig/commands/cli/_common.py
 stig/commands/cli/_mixin.py
 stig/commands/cli/_table.py
 stig/commands/cli/config.py
 stig/commands/cli/file.py
 stig/commands/cli/misc.py
 stig/commands/cli/peer.py
 stig/commands/cli/torrent.py
@@ -70,16 +72,14 @@
 stig/commands/tui/torrent.py
 stig/commands/tui/tracker.py
 stig/commands/tui/tui.py
 stig/settings/__init__.py
 stig/settings/default.theme
 stig/settings/defaults.py
 stig/settings/rcfile.py
-stig/settings/types.py
-stig/settings/types_srv.py
 stig/tui/__init__.py
 stig/tui/cli.py
 stig/tui/group.py
 stig/tui/hooks.py
 stig/tui/infobar.py
 stig/tui/keymap.py
 stig/tui/logger.py
@@ -87,26 +87,31 @@
 stig/tui/scroll.py
 stig/tui/table.py
 stig/tui/tabs.py
 stig/tui/theme.py
 stig/tui/urwidpatches.py
 stig/tui/views/__init__.py
 stig/tui/views/common_columns.py
-stig/tui/views/filelist.py
-stig/tui/views/flist_columns.py
+stig/tui/views/file.py
+stig/tui/views/file_list.py
 stig/tui/views/hooks.py
-stig/tui/views/peerlist.py
-stig/tui/views/plist_columns.py
+stig/tui/views/peer.py
+stig/tui/views/peer_list.py
+stig/tui/views/setting.py
+stig/tui/views/setting_list.py
 stig/tui/views/summary.py
-stig/tui/views/tlist_columns.py
-stig/tui/views/torrentlist.py
-stig/tui/views/trackerlist.py
-stig/tui/views/trklist_columns.py
+stig/tui/views/torrent.py
+stig/tui/views/torrent_list.py
+stig/tui/views/tracker.py
+stig/tui/views/tracker_list.py
 stig/utils/__init__.py
-stig/utils/_number.py
+stig/utils/_converter.py
 stig/utils/expandtabs.py
+stig/utils/string.py
+stig/utils/usertypes.py
 stig/views/__init__.py
-stig/views/filelist.py
-stig/views/peerlist.py
+stig/views/file.py
+stig/views/peer.py
+stig/views/setting.py
 stig/views/summary.py
-stig/views/torrentlist.py
-stig/views/trackerlist.py
+stig/views/torrent.py
+stig/views/tracker.py
```

### Comparing `stig-0.8.3a0/setup.py` & `stig-0.9.0a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import os
     if os.path.exists('README.org'):
         long_description = pypandoc.convert('README.org', 'rst')
 except ImportError:
     pass
 
 # Load __version__ variable without importing the whole stig module
-with open('stig/version.py') as f:
+with open('stig/__version__.py') as f:
     exec(f.read())
 
 from setuptools import setup, find_packages
 setup(
     name             = 'stig',
     version          = __version__,
     license          = 'GPLv3+',
@@ -29,19 +29,27 @@
     packages         = find_packages(),
     package_data     = {'stig': ['settings/default.theme']},
 
     python_requires  = '>=3.5',
     install_requires = [
         'urwid>=1.3.0',
         'urwidtrees>=1.0.3dev0',
-        'aiohttp>=0.22.5',
+        'aiohttp>=3',
+        'async_timeout',
         'pyxdg',
         'blinker',
         'natsort',
     ],
+    extras_require = {
+        'geoip': ['maxminddb'],
+        'setproctitle': ['setproctitle'],
+    },
+    tests_require = [
+        'asynctest>=0.11',
+    ],
 
     entry_points = { 'console_scripts': [ 'stig = stig:run' ] },
 
     classifiers = [
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
```

### Comparing `stig-0.8.3a0/stig/utils/__init__.py` & `stig-0.9.0a0/stig/utils/string.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,44 +5,51 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-from ._number import (NumberFloat, NumberInt, pretty_float)
 
-import unicodedata
+from unicodedata import normalize as _normalize_unicode
+def normalize_unicode(string):
+    """
+    Convert combining character sequences into graphemes (e.g. "a˚" -> "å") so
+    that len() reports the correct length.
+    http://www.unicode.org/faq/char_combmark.html
+    """
+    return _normalize_unicode('NFC', string)
 
 
 def striplines(lines):
     """Remove empty strings from start and end of `lines` using `pop`"""
     lines = list(lines)
     while lines and lines[0] == '':
         lines.pop(0)
     while lines and lines[-1] == '':
         lines.pop(-1)
     yield from lines
 
 
+from unicodedata import east_asian_width as _east_asian_width
 def strwidth(string):
     """Return displayed width of `string`, considering wide characters"""
     return len(string) + sum(1 for char in string
-                             if unicodedata.east_asian_width(char) in 'FW')
+                             if _east_asian_width(char) in 'FW')
 
 
 def strcrop(string, width, tail=None):
     """Return `string` cropped to `width`, considering wide characters
 
     If `tail` is not None, it must be a string that is appended to the cropped
     string.
     """
     def widechar_indexes(s):
         for i,c in enumerate(s):
-            if unicodedata.east_asian_width(c) in 'FW':
+            if _east_asian_width(c) in 'FW':
                 yield i
 
     if strwidth(string) <= width:
         return string  # string is already short enough
 
     if tail is not None:
         width -= strwidth(tail)  # Account for tail in final width
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stig-0.8.3a0/stig/utils/_number.py` & `stig-0.9.0a0/stig/client/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,214 +5,285 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-
-from itertools import chain
-from types import MethodType
-import re
+from ..utils.usertypes import (Bool, Int, Float, Option, Path, multitype)
+from ..utils import convert
+from . import constants as const
 
 
-def pretty_float(n):
-    """Format float with a reasonable amount of decimal places"""
-    if n >= float('inf'):
-        return '∞'
-    n_abs = abs(n)
-    n_abs_r2 = round(n_abs, 2)
-    if n_abs == 0:
-        return '0'
-    elif n_abs_r2 == int(n_abs):
-        return '%.0f' % n
-    elif n_abs_r2 < 10:
-        return '%.2f' % n
-    elif round(n_abs, 1) < 100:
-        return '%.1f' % n
-    else:
-        return '%.0f' % n
-
-
-class _NumberBase():
-    _PREFIXES_BINARY = (('Ti', 1024**4), ('Gi', 1024**3), ('Mi', 1024**2), ('Ki', 1024))
-    _PREFIXES_METRIC = (('T', 1000**4), ('G', 1000**3), ('M', 1000**2), ('k', 1000))
-    _PREFIXES = tuple((prefix.lower(), size)
-                      for prefix,size in chain.from_iterable(zip(_PREFIXES_BINARY,
-                                                                 _PREFIXES_METRIC)))
-    _PREFIXES_DCT = dict(_PREFIXES)
-
-    _REGEX = re.compile('^([-+]?(?:\d+\.\d+|\d+|\.\d+)) ?(' +\
-                        '|'.join(p[0] for p in _PREFIXES) + \
-                        '|)(\S*?)$',
-                        flags=re.IGNORECASE)
-
-    # Public tuple of all supported unit prefixes
-    UNIT_PREFIXES = tuple(prefix for prefix,size in chain.from_iterable(zip(_PREFIXES_BINARY,
-                                                                            _PREFIXES_METRIC)))
+class Bandwidth(Int):
+    typename = 'bandwidth'
+
+    def __new__(cls, value, **kwargs):
+        value = convert.bandwidth(value)
+        kwargs.update(unit=convert.bandwidth.unit,
+                      prefix=convert.bandwidth.prefix)
+        return super().__new__(cls, value, **kwargs)
 
     @classmethod
-    def from_string(cls, string, *, prefix=None, unit=None, str_includes_unit=None):
-        match = cls._REGEX.match(str(string))
-        if match is None:
-            raise ValueError('Not a number: %r' % string)
-        else:
-            # Convert to float first, because a) int('1.2') is not allowed and
-            # b) so '1.2k' (which is a integer) is not parsed to 1000
-            num = float(match.group(1))
-            unit = match.group(3) or unit
-            prfx = match.group(2)
-            if prfx:
-                all_prfxs = cls._PREFIXES_DCT
-                prfx_lower = prfx.lower()
-                # _REGEX matches, so we can be sure that prfx_lower is in all_prfxs
-                num *= all_prfxs[prfx_lower]
-            num = cls._numtype(num)
-
-            prfx_len = len(prfx)
-            if prfx_len == 2:
-                prefix = 'binary'
-            elif prfx_len == 1:
-                prefix = 'metric'
-
-            return cls(num, prefix=prefix, unit=unit, str_includes_unit=str_includes_unit)
-
-    def __new__(cls, num, *, prefix=None, unit=None, str_includes_unit=None):
-        if isinstance(num, _NumberBase):
-            # Copy properties from existing Number instance unless they are
-            # overridden by arguments.
-            prefix = num.prefix if prefix is None else prefix
-            unit = num.unit if unit is None else unit
-            str_includes_unit = num.str_includes_unit if str_includes_unit is None else str_includes_unit
-            # return cls(float(num), prefix=prefix, unit=unit, str_includes_unit=str_includes_unit)
-            return cls(cls._numtype(num), prefix=prefix, unit=unit, str_includes_unit=str_includes_unit)
-
-        # We can't specify defaults in the arguments because then we don't know
-        # which arguments are passed and which are default.
-        prefix = 'metric' if prefix is None else prefix
-        str_includes_unit = True if str_includes_unit is None else str_includes_unit
-
-        if isinstance(num, str):
-            return cls.from_string(num, prefix=prefix, unit=unit, str_includes_unit=str_includes_unit)
-        elif isinstance(num, (int, float)):
-            obj = super().__new__(cls, num)
-            obj.unit = unit
-            obj.prefix = prefix
-            obj.str_includes_unit = str_includes_unit
-            return obj
-        else:
-            raise ValueError('Not a number: %r' % num)
+    def _get_syntax(cls, **kwargs):
+        return '%s[b|B]' % super()._get_syntax(**kwargs)
 
-    def __str__(self):
-        return self.__str()
 
-    @property
-    def str_includes_unit(self):
-        return self._str_includes_unit
-    @str_includes_unit.setter
-    def str_includes_unit(self, str_includes_unit):
-        if str_includes_unit:
-            self.__str = MethodType(lambda self: self.with_unit, self)
+class BoolOrBandwidth(multitype(Bool.partial(true=('limited', 'enabled', 'yes', 'on', 'true'),
+                                             false=('unlimited', 'disabled', 'no', 'off', 'false')),
+                                Bandwidth)):
+    @staticmethod
+    def adjust(current, adjustment):
+        """Adjust `current` by `adjustment`"""
+        if isinstance(current, Bool) or current >= float('inf'):
+            # If current number is infinity, adjust from 0
+            current = 0
+        new = current + adjustment
+        if new < 0:
+            # Drop to 0 if current is greater than zero.
+            # If current already is zero, drop to infinity.
+            if current > 0:
+                new = 0
+            else:
+                new = const.UNLIMITED
+        return new
+
+    def __new__(cls, value, **kwargs):
+        if isinstance(value, (float, int)) and value >= float('inf'):
+            return super().__new__(cls, 'unlimited')
         else:
-            self.__str = MethodType(lambda self: self.without_unit, self)
-        self._str_includes_unit = bool(str_includes_unit)
+            return super().__new__(cls, value, **kwargs)
 
-    def __repr__(self):
-        return '<{} {}, prefix={!r}, unit={!r}>'.format(type(self).__name__, self._numtype(self),
-                                                        self._prefix, self._unit)
 
-    @property
-    def with_unit(self):
-        s = self.without_unit
-        if self.unit is not None:
-            s += self.unit
-        return s
+BoolOrPath = multitype(Bool, Path)
 
-    @property
-    def without_unit(self):
-        absolute = abs(self)
-        if self == 0:
-            # This should increase efficiency since 0 is a common value
-            return '0'
-        elif absolute >= float('inf'):
-            return pretty_float(self)
+
+class PerfectInterval():
+    """Remove processing time from intervals"""
+
+    def __init__(self, loop):
+        self._loop = loop
+        self._last_timestamp = 0
+
+    def __call__(self, seconds):
+        now = self._loop.time()
+        if self._last_timestamp <= 0:
+            self._last_timestamp = int(now)
+            return seconds
         else:
-            for prefix,size in self._prefixes:
-                if absolute >= size:
-                    return pretty_float(self/size) + prefix
-            return pretty_float(self)
+            expected = self._last_timestamp + seconds
+            diff = now - expected
+            interval = max(seconds - diff, 0)
+            self._last_timestamp = expected
+            return interval
+
+
+import asyncio
+from async_timeout import timeout as async_timeout
+class SleepUneasy():
+    """Asynchronous sleep() that can be aborted"""
+
+    def __init__(self, loop):
+        self.loop = loop
+        self._interrupt = asyncio.Event(loop=self.loop)
+        self._perfint = PerfectInterval(self.loop)
+
+    async def sleep(self, seconds):
+        """Sleep for `seconds` or until `interrupt` is called"""
+        self._interrupt.clear()
+        # Remove processing time from seconds
+        seconds = self._perfint(seconds)
+        try:
+            async with async_timeout(seconds, loop=self.loop):
+                await self._interrupt.wait()
+        except asyncio.TimeoutError:
+            pass  # Interval passed without interrupt
+        finally:
+            self._interrupt.clear()
+
+    def interrupt(self):
+        """Stop sleeping"""
+        self._interrupt.set()
+
+
+from types import SimpleNamespace
+class Response(SimpleNamespace):
+    """Response to an API call
+
+    All API implementations should use this class to provide return values to
+    API calls.
+
+    success: Whether the call was a success
+    msgs: Sequence of messages; either strings or ClientError exceptions
+
+    Any other keyword arguments are made available as attributes.
+    """
+    def __init__(self, success=False, msgs=(), **kwargs):
+        super().__init__(success=bool(success), msgs=tuple(msgs), **kwargs)
+
+
+def lazy_property(after_creation=None):
+    """Property that replaces itself with the requested object when accessed
+
+    `after_creation` is called with the instance of the property.
+    """
+    # https://stackoverflow.com/a/6849299
+    class _lazy_property():
+        def __init__(self, fget):
+            self.fget = fget
+            self.func_name = fget.__name__
+            self.after_creation = after_creation
+
+        def __get__(self, obj, cls):
+            if obj is None:
+                return None
+            value = self.fget(obj)
+            setattr(obj, self.func_name, value)
+            if self.after_creation is not None:
+                self.after_creation(obj)
+            return value
+
+    return _lazy_property
+
+
+class LazyDict(dict):
+    """Dictionary with callables as values that return the actual value on demand"""
+    def __getitem__(self, key):
+        value = dict.__getitem__(self, key)
+        if callable(value):
+            value = value()
+            dict.__setitem__(self, key, value)
+        return value
 
-    @property
-    def unit(self):
-        return self._unit
-    @unit.setter
-    def unit(self, unit):
-        self._unit = str(unit) if unit is not None else None
+
+import re
+class URL():
+    """Parse URL as lenient as possible (no validation)"""
+
+    ### Pilfered from yurl: https://github.com/homm/yurl
+    # This is not validating regexp.
+    # It splits url to unambiguous parts according RFC.
+    _split_re = re.compile(r'''
+        (?:([^:/?#]+):)?            # scheme
+        (?://                       # authority
+            (?:([^/?\#@]*)@)?       # userinfo
+            ([^/?\#]*)              # host:port
+        )?
+        ([^?\#]*)                   # path
+        \??([^\#]*)                 # query
+        \#?(.*)                     # fragment
+        ''', re.VERBOSE | re.DOTALL).match
+
+    @classmethod
+    def _parse_url(cls, url):
+        # Default to http scheme so 'host:123' is not interpreted as 'host://123/'
+        if len(url) > 0 and '://' not in str(url):
+            url = 'http://' + str(url)
+
+        groups = cls._split_re(url).groups('')
+        # Order: scheme, user+password, host+port, path, query, fragment
+        dct = {}
+        dct['scheme']   = groups[0] or None
+        dct['path']     = groups[3] or None
+        dct['query']    = groups[4] or None
+        dct['fragment'] = groups[5] or None
+
+        auth = groups[1]
+        user, pw = None, None
+        if auth:
+            # Password in authentication is optional
+            if ':' in auth:
+                user, pw = auth.split(':')
+            else:
+                user, pw = auth, None
+        dct['user'] = user or None
+        dct['password'] = pw or None
+
+        # Split port from host only if it consists of digits.
+        host = groups[2]
+        port = None
+        port_idx = host.rfind(':')
+        if port_idx >= 0:
+            port_str = host[port_idx+1:]
+            if port_str.isdigit():
+                host = host[:port_idx]
+                port = int(port_str)
+        dct['host'] = host or None
+        dct['port'] = port or None
+
+        return dct
+
+    _obj_cache = {}
+    def __new__(cls, url):
+        if isinstance(url, cls):
+            return url
+
+        cache_id = url
+        cache = cls._obj_cache
+        url_dict = cache.get(cache_id)
+        if url_dict is None:
+            url_dict = cache[cache_id] = cls._parse_url(url)
+
+        obj = super().__new__(cls)
+        for attr in ('scheme', 'host', 'port', 'path', 'user', 'password'):
+            setattr(obj, attr, url_dict[attr])
+        return obj
 
     @property
-    def prefix(self):
-        return self._prefix
-    @prefix.setter
-    def prefix(self, prefix):
-        if prefix == 'binary':
-            self._prefixes = self._PREFIXES_BINARY
-        elif prefix == 'metric':
-            self._prefixes = self._PREFIXES_METRIC
-        else:
-            raise ValueError("prefix must be 'binary' or 'metric', not {!r}".format(prefix))
-        self._prefix = prefix
+    def has_auth(self):
+        """Whether user and password properties are set"""
+        return self.user is not None and self.password is not None
 
-    def _do_math(self, method, *args, **kwargs):
-        # Get the new value as int or float
-        if self == float('inf'):
-            # No need to do any calculations with infinity, especially because
-            # of round() throwing an OverflowError because `int` has no infinity
-            # value implemented.
-            new_value = float('inf')
-        else:
-            new_value = getattr(self._numtype, method)(self, *args, **kwargs)
+    @property
+    def domain(self):
+        """TLD Domain"""
+        if not hasattr(self, '_domain_cached'):
+            host = self.host
+            if not host:
+                self._domain_cached = None
+            else:
+                if host.count('.') <= 1:
+                    self._domain_cached = host
+                else:
+                    parts = host.rsplit('.', maxsplit=2)
+                    self._domain_cached = '.'.join(parts[-2:])
+        return self._domain_cached
 
-        if new_value is NotImplemented:
-            # This may have happened because `self._numtype` is `int` and it got
-            # a `float` to handle.  To make this work, we must flip `self` and
-            # `other`, getting the method from `other` and passing it `self`:
-            #
-            #     int.__add__(<int>, <float>)  ->  float.__add__(<float>, <int>)
-            #
-            # If we get the parent method from the instance instead of its type,
-            # we don't have to pass two values and it's a little bit faster.
-            parent_method = getattr(args[0], method)
-            new_value = parent_method(self, **kwargs)
-            if new_value is NotImplemented:
-                return NotImplemented
-
-        # Determine the appropriate class (1.0 should return a NumberInt)
-        if isinstance(new_value, int) or (new_value < float('inf') and
-                                          isinstance(new_value, float) and
-                                          int(new_value) == new_value):
-            new_cls = NumberInt
-        else:
-            new_cls = NumberFloat
+    def __str__(self):
+        if not hasattr(self, '_cached_string'):
+            parts = []
+            if self.scheme:
+                parts.append('%s://' % self.scheme)
+            if self.user:
+                parts.append('%s' % self.user)
+                if self.password:
+                    parts.append(':%s' % self.password)
+                parts.append('@')
+            if self.host:
+                parts.append(self.host)
+            if self.port:
+                parts.append(':%s' % self.port)
+            if self.path:
+                parts.append('%s' % self.path)
+            self._cached_string = ''.join(parts)
+        return self._cached_string
+
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        if name[0] != '_':
+            # Clear caches
+            if hasattr(self, '_cached_string'):
+                del self._cached_string
+            if name == 'host' and hasattr(self, '_domain_cached'):
+                del self._domain_cached
 
-        # Copy all properties to new instance
-        return new_cls(new_value, unit=self.unit, prefix=self.prefix,
-                       str_includes_unit=self._str_includes_unit)
-
-    def __add__(self, other):             return self._do_math('__add__', other)
-    def __sub__(self, other):             return self._do_math('__sub__', other)
-    def __mul__(self, other):             return self._do_math('__mul__', other)
-    def __div__(self, other):             return self._do_math('__div__', other)
-    def __truediv__(self, other):         return self._do_math('__truediv__', other)
-    def __floordiv__(self, other):        return self._do_math('__floordiv__', other)
-    def __mod__(self, other):             return self._do_math('__mod__', other)
-    def __divmod__(self, other):          return self._do_math('__divmod__', other)
-    def __pow__(self, other):             return self._do_math('__pow__', other)
-    def __floor__(self):                  return self._do_math('__floor__')
-    def __ceil__(self):                   return self._do_math('__ceil__')
-    def __round__(self, *args, **kwargs): return self._do_math('__round__', *args, **kwargs)
+    def __repr__(self):
+        return '<%s %s>' % (type(self).__name__, str(self))
 
+    def __hash__(self):
+        return hash(str(self))
 
-class NumberFloat(_NumberBase, float):
-    _numtype = float
+    def __eq__(self, other):
+        return str(self) == str(other)
 
-class NumberInt(_NumberBase, int):
-    _numtype = int
+    def __ne__(self, other):
+        return str(self) != str(other)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stig-0.8.3a0/stig/utils/expandtabs.py` & `stig-0.9.0a0/stig/utils/expandtabs.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/settings/__init__.py` & `stig-0.9.0a0/stig/commands/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,10 +5,13 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-from .types import Settings
-from .types_srv import is_srv_setting
-from .defaults import (init_defaults, init_server_defaults)
+from .config import *
+from .misc import *
+from .torrent import *
+from .file import *
+from .peer import *
+from .tracker import *
```

### Comparing `stig-0.8.3a0/stig/settings/default.theme` & `stig-0.9.0a0/stig/settings/default.theme`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,33 @@
 tabs.torrentsummary.focused   black         on light blue
 tabs.filelist.unfocused       light magenta on dark gray
 tabs.filelist.focused         black         on dark magenta
 tabs.peerlist.unfocused       light green   on dark gray
 tabs.peerlist.focused         black         on dark green
 tabs.trackerlist.unfocused    white         on dark gray
 tabs.trackerlist.focused      black         on light gray
-tabs.help.unfocused           yellow        on dark gray
-tabs.help.focused             black         on yellow
+tabs.settinglist.unfocused    yellow        on dark blue
+tabs.settinglist.focused      dark blue     on yellow
+tabs.help.unfocused           light green   on dark blue
+tabs.help.focused             dark blue     on light green
 
 $topbar_bg = dark blue
 topbar                    light gray    on $topbar_bg
 topbar.host.connected     light green   on $topbar_bg
 topbar.host.connecting    black         on light magenta
 topbar.host.disconnected  black         on light red
 topbar.help.key           light cyan    on $topbar_bg
 topbar.help.equals        light cyan    on $topbar_bg
 topbar.help.label         light cyan    on $topbar_bg
 topbar.help.space         light cyan    on $topbar_bg
 
 $bottombar_bg = dark gray
 bottombar                             light gray     on $bottombar_bg
 bottombar.important                   light red,bold on $bottombar_bg
+bottombar.marked                      yellow,bold    on $bottombar_bg
 bottombar.bandwidth.up                dark green     on $bottombar_bg
 bottombar.bandwidth.up.highlighted    light green    on $bottombar_bg
 bottombar.bandwidth.down              dark cyan      on $bottombar_bg
 bottombar.bandwidth.down.highlighted  light cyan     on $bottombar_bg
 
 $log_bg = dark gray
 log                        light gray     on $log_bg
@@ -94,14 +97,19 @@
 
 $tlist_bg.uf = black
 $tlist_bg.f  = dark gray
 torrentlist                                        default              on $tlist_bg.uf
 torrentlist.focused                                default              on $tlist_bg.f
 torrentlist.header                                 light gray,underline on $tlist_bg.uf
 
+$id_fg = white
+torrentlist.id.header                              $id_fg,underline on $tlist_bg.uf
+torrentlist.id.unfocused                           $id_fg           on $tlist_bg.uf
+torrentlist.id.focused                             $id_fg           on $tlist_bg.f
+
 $downloaded_fg = dark cyan
 $downloaded_hl = light cyan
 torrentlist.downloaded.header                      $downloaded_fg,underline on $tlist_bg.uf
 torrentlist.downloaded.unfocused                   $downloaded_fg           on $tlist_bg.uf
 torrentlist.downloaded.focused                     $downloaded_fg           on $tlist_bg.f
 torrentlist.downloaded.highlighted.unfocused       $downloaded_hl           on $tlist_bg.uf
 torrentlist.downloaded.highlighted.focused         $downloaded_hl           on $tlist_bg.f
@@ -128,37 +136,37 @@
 torrentlist.marked.focused                         $marked_fg           on $tlist_bg.f
 
 $path_fg = light gray
 torrentlist.path.header                            $path_fg,underline on $tlist_bg.uf
 torrentlist.path.unfocused                         $path_fg           on $tlist_bg.uf
 torrentlist.path.focused                           $path_fg           on $tlist_bg.f
 
-$connections_fg = light gray
-$connections_hl = white
-torrentlist.connections.header                     $connections_fg,underline on $tlist_bg.uf
-torrentlist.connections.unfocused                  $connections_fg           on $tlist_bg.uf
-torrentlist.connections.focused                    $connections_fg           on $tlist_bg.f
-torrentlist.connections.highlighted.unfocused      $connections_hl           on $tlist_bg.uf
-torrentlist.connections.highlighted.focused        $connections_hl           on $tlist_bg.f
+$peers_fg = light gray
+$peers_hl = white
+torrentlist.peers.header                           $peers_fg,underline on $tlist_bg.uf
+torrentlist.peers.unfocused                        $peers_fg           on $tlist_bg.uf
+torrentlist.peers.focused                          $peers_fg           on $tlist_bg.f
+torrentlist.peers.highlighted.unfocused            $peers_hl           on $tlist_bg.uf
+torrentlist.peers.highlighted.focused              $peers_hl           on $tlist_bg.f
 
 $seeds_fg = light gray
 $seeds_hl = white
 torrentlist.seeds.header                           $seeds_fg,underline on $tlist_bg.uf
 torrentlist.seeds.unfocused                        $seeds_fg           on $tlist_bg.uf
 torrentlist.seeds.focused                          $seeds_fg           on $tlist_bg.f
 torrentlist.seeds.highlighted.unfocused            $seeds_hl           on $tlist_bg.uf
 torrentlist.seeds.highlighted.focused              $seeds_hl           on $tlist_bg.f
 
-$progress_fg = dark blue
-$progress_hl = light blue
-torrentlist.progress.header                        $progress_fg,underline on $tlist_bg.uf
-torrentlist.progress.unfocused                     $progress_fg           on $tlist_bg.uf
-torrentlist.progress.focused                       $progress_fg           on $tlist_bg.f
-torrentlist.progress.highlighted.unfocused         $progress_hl           on $tlist_bg.uf
-torrentlist.progress.highlighted.focused           $progress_hl           on $tlist_bg.f
+$%downloaded_fg = dark blue
+$%downloaded_hl = light blue
+torrentlist.%downloaded.header                     $%downloaded_fg,underline on $tlist_bg.uf
+torrentlist.%downloaded.unfocused                  $%downloaded_fg           on $tlist_bg.uf
+torrentlist.%downloaded.focused                    $%downloaded_fg           on $tlist_bg.f
+torrentlist.%downloaded.highlighted.unfocused      $%downloaded_hl           on $tlist_bg.uf
+torrentlist.%downloaded.highlighted.focused        $%downloaded_hl           on $tlist_bg.f
 
 $%available_fg = dark blue
 $%available_hl = light blue
 torrentlist.%available.header                      $%available_fg,underline on $tlist_bg.uf
 torrentlist.%available.unfocused                   $%available_fg           on $tlist_bg.uf
 torrentlist.%available.focused                     $%available_fg           on $tlist_bg.f
 torrentlist.%available.highlighted.unfocused       $%available_hl           on $tlist_bg.uf
@@ -176,29 +184,29 @@
 $rate-up_hl = light green
 torrentlist.rate-up.header                         $rate-up_fg,underline on $tlist_bg.uf
 torrentlist.rate-up.unfocused                      $rate-up_fg           on $tlist_bg.uf
 torrentlist.rate-up.focused                        $rate-up_fg           on $tlist_bg.f
 torrentlist.rate-up.highlighted.unfocused          $rate-up_hl           on $tlist_bg.uf
 torrentlist.rate-up.highlighted.focused            $rate-up_hl           on $tlist_bg.f
 
-$rate-limit-down_fg = dark cyan
-$rate-limit-down_hl = light cyan
-torrentlist.rate-limit-down.header                 $rate-limit-down_fg,underline on $tlist_bg.uf
-torrentlist.rate-limit-down.unfocused              $rate-limit-down_fg           on $tlist_bg.uf
-torrentlist.rate-limit-down.focused                $rate-limit-down_fg           on $tlist_bg.f
-torrentlist.rate-limit-down.highlighted.unfocused  $rate-limit-down_hl           on $tlist_bg.uf
-torrentlist.rate-limit-down.highlighted.focused    $rate-limit-down_hl           on $tlist_bg.f
-
-$rate-limit-up_fg = dark green
-$rate-limit-up_hl = light green
-torrentlist.rate-limit-up.header                   $rate-limit-up_fg,underline on $tlist_bg.uf
-torrentlist.rate-limit-up.unfocused                $rate-limit-up_fg           on $tlist_bg.uf
-torrentlist.rate-limit-up.focused                  $rate-limit-up_fg           on $tlist_bg.f
-torrentlist.rate-limit-up.highlighted.unfocused    $rate-limit-up_hl           on $tlist_bg.uf
-torrentlist.rate-limit-up.highlighted.focused      $rate-limit-up_hl           on $tlist_bg.f
+$limit-rate-down_fg = dark cyan
+$limit-rate-down_hl = light cyan
+torrentlist.limit-rate-down.header                 $limit-rate-down_fg,underline on $tlist_bg.uf
+torrentlist.limit-rate-down.unfocused              $limit-rate-down_fg           on $tlist_bg.uf
+torrentlist.limit-rate-down.focused                $limit-rate-down_fg           on $tlist_bg.f
+torrentlist.limit-rate-down.highlighted.unfocused  $limit-rate-down_hl           on $tlist_bg.uf
+torrentlist.limit-rate-down.highlighted.focused    $limit-rate-down_hl           on $tlist_bg.f
+
+$limit-rate-up_fg = dark green
+$limit-rate-up_hl = light green
+torrentlist.limit-rate-up.header                   $limit-rate-up_fg,underline on $tlist_bg.uf
+torrentlist.limit-rate-up.unfocused                $limit-rate-up_fg           on $tlist_bg.uf
+torrentlist.limit-rate-up.focused                  $limit-rate-up_fg           on $tlist_bg.f
+torrentlist.limit-rate-up.highlighted.unfocused    $limit-rate-up_hl           on $tlist_bg.uf
+torrentlist.limit-rate-up.highlighted.focused      $limit-rate-up_hl           on $tlist_bg.f
 
 $ratio_fg = dark blue
 $ratio_hl = light blue
 torrentlist.ratio.header                           $ratio_fg,underline on $tlist_bg.uf
 torrentlist.ratio.unfocused                        $ratio_fg           on $tlist_bg.uf
 torrentlist.ratio.focused                          $ratio_fg           on $tlist_bg.f
 torrentlist.ratio.highlighted.unfocused            $ratio_hl           on $tlist_bg.uf
@@ -370,15 +378,16 @@
 torrentlist.name.discovering.progress1.focused     $name.discovering_fg,underline on $tlist_bg.f
 torrentlist.name.discovering.progress2.unfocused   $name.discovering_fg           on $tlist_bg.uf
 torrentlist.name.discovering.progress2.focused     $name.discovering_fg           on $tlist_bg.f
 torrentlist.name.discovering.complete.unfocused    $name.discovering_fg           on $tlist_bg.uf
 torrentlist.name.discovering.complete.focused      $name.discovering_fg           on $tlist_bg.f
 
 
-torrentsummary light gray on black
+torrentsummary       light gray on black
+torrentsummary.error light red  on black
 
 
 $flist_bg.uf = black
 $flist_bg.f  = dark gray
 filelist                                   default              on $flist_bg.uf
 filelist.focused                           default              on $flist_bg.f
 filelist.header                            light gray,underline on $flist_bg.uf
@@ -405,21 +414,21 @@
 $downloaded_hl = light cyan
 filelist.downloaded.header                 $downloaded_fg,underline on $flist_bg.uf
 filelist.downloaded.unfocused              $downloaded_fg           on $flist_bg.uf
 filelist.downloaded.focused                $downloaded_fg           on $flist_bg.f
 filelist.downloaded.highlighted.unfocused  $downloaded_hl           on $flist_bg.uf
 filelist.downloaded.highlighted.focused    $downloaded_hl           on $flist_bg.f
 
-$progress_fg = dark blue
-$progress_hl = light blue
-filelist.progress.header                   $progress_fg,underline on $flist_bg.uf
-filelist.progress.unfocused                $progress_fg           on $flist_bg.uf
-filelist.progress.focused                  $progress_fg           on $flist_bg.f
-filelist.progress.highlighted.unfocused    $progress_hl           on $flist_bg.uf
-filelist.progress.highlighted.focused      $progress_hl           on $flist_bg.f
+$%downloaded_fg = dark blue
+$%downloaded_hl = light blue
+filelist.%downloaded.header                $%downloaded_fg,underline on $flist_bg.uf
+filelist.%downloaded.unfocused             $%downloaded_fg           on $flist_bg.uf
+filelist.%downloaded.focused               $%downloaded_fg           on $flist_bg.f
+filelist.%downloaded.highlighted.unfocused $%downloaded_hl           on $flist_bg.uf
+filelist.%downloaded.highlighted.focused   $%downloaded_hl           on $flist_bg.f
 
 $priority_fg = brown
 $priority_hl = yellow
 filelist.priority.header                   $priority_fg,underline on $flist_bg.uf
 filelist.priority.unfocused                $priority_fg           on $flist_bg.uf
 filelist.priority.focused                  $priority_fg           on $flist_bg.f
 filelist.priority.low.unfocused            $priority_fg           on $flist_bg.uf
@@ -447,19 +456,19 @@
 peerlist.port.header                       $port_fg,underline on $plist_bg
 peerlist.port.unfocused                    $port_fg           on $plist_bg
 
 $client_fg = dark magenta
 peerlist.client.header                     $client_fg,underline on $plist_bg
 peerlist.client.unfocused                  $client_fg           on $plist_bg
 
-$progress_fg = dark blue
-$progress_hl = light blue
-peerlist.progress.header                   $progress_fg,underline on $plist_bg
-peerlist.progress.unfocused                $progress_fg           on $plist_bg
-peerlist.progress.highlighted.unfocused    $progress_hl           on $plist_bg
+$%downloaded_fg = dark blue
+$%downloaded_hl = light blue
+peerlist.%downloaded.header                $%downloaded_fg,underline on $plist_bg
+peerlist.%downloaded.unfocused             $%downloaded_fg           on $plist_bg
+peerlist.%downloaded.highlighted.unfocused $%downloaded_hl           on $plist_bg
 
 $rate-down_fg = dark cyan
 $rate-down_hl = light cyan
 peerlist.rate-down.header                  $rate-down_fg,underline on $plist_bg
 peerlist.rate-down.unfocused               $rate-down_fg           on $plist_bg
 peerlist.rate-down.highlighted.unfocused   $rate-down_hl           on $plist_bg
 
@@ -513,18 +522,18 @@
 trackerlist.url-announce.focused           $url-announce_fg           on $trklist_bg.f
 
 $url-scrape_fg = light blue
 trackerlist.url-scrape.header              $url-scrape_fg,underline on $trklist_bg.uf
 trackerlist.url-scrape.unfocused           $url-scrape_fg           on $trklist_bg.uf
 trackerlist.url-scrape.focused             $url-scrape_fg           on $trklist_bg.f
 
-$state_fg = dark cyan
-trackerlist.state.header                   $state_fg,underline on $trklist_bg.uf
-trackerlist.state.unfocused                $state_fg           on $trklist_bg.uf
-trackerlist.state.focused                  $state_fg           on $trklist_bg.f
+$status_fg = dark cyan
+trackerlist.status.header                  $status_fg,underline on $trklist_bg.uf
+trackerlist.status.unfocused               $status_fg           on $trklist_bg.uf
+trackerlist.status.focused                 $status_fg           on $trklist_bg.f
 
 $error_fg = dark red
 trackerlist.error.header                   $error_fg,underline on $trklist_bg.uf
 trackerlist.error.unfocused                $error_fg           on $trklist_bg.uf
 trackerlist.error.focused                  $error_fg           on $trklist_bg.f
 
 $error-announce_fg = dark red
@@ -559,16 +568,45 @@
 
 $next-announce_fg = white
 trackerlist.next-announce.header           $next-announce_fg,underline on $trklist_bg.uf
 trackerlist.next-announce.unfocused        $next-announce_fg           on $trklist_bg.uf
 trackerlist.next-announce.focused          $next-announce_fg           on $trklist_bg.f
 
 $last-scrape_fg = white
-trackerlist.last-scrape.header           $last-scrape_fg,underline on $trklist_bg.uf
-trackerlist.last-scrape.unfocused        $last-scrape_fg           on $trklist_bg.uf
-trackerlist.last-scrape.focused          $last-scrape_fg           on $trklist_bg.f
+trackerlist.last-scrape.header             $last-scrape_fg,underline on $trklist_bg.uf
+trackerlist.last-scrape.unfocused          $last-scrape_fg           on $trklist_bg.uf
+trackerlist.last-scrape.focused            $last-scrape_fg           on $trklist_bg.f
 
 $next-scrape_fg = white
-trackerlist.next-scrape.header           $next-scrape_fg,underline on $trklist_bg.uf
-trackerlist.next-scrape.unfocused        $next-scrape_fg           on $trklist_bg.uf
-trackerlist.next-scrape.focused          $next-scrape_fg           on $trklist_bg.f
-
+trackerlist.next-scrape.header             $next-scrape_fg,underline on $trklist_bg.uf
+trackerlist.next-scrape.unfocused          $next-scrape_fg           on $trklist_bg.uf
+trackerlist.next-scrape.focused            $next-scrape_fg           on $trklist_bg.f
+
+
+$slist_bg.uf = black
+$slist_bg.f  = dark gray
+settinglist                                default              on $slist_bg.uf
+settinglist.focused                        default              on $slist_bg.f
+settinglist.header                         light gray,underline on $slist_bg.uf
+
+$name_fg = light blue
+settinglist.name.header                    $name_fg,underline on $slist_bg.uf
+settinglist.name.unfocused                 $name_fg           on $slist_bg.uf
+settinglist.name.focused                   $name_fg           on $slist_bg.f
+
+$value_fg = light gray
+$value_hl = white,bold
+settinglist.value.header                   $value_fg,underline on $slist_bg.uf
+settinglist.value.unfocused                $value_fg           on $slist_bg.uf
+settinglist.value.focused                  $value_fg           on $slist_bg.f
+settinglist.value.highlighted.unfocused    $value_hl           on $slist_bg.uf
+settinglist.value.highlighted.focused      $value_hl           on $slist_bg.f
+
+$default_fg = light gray
+settinglist.default.header                 $default_fg,underline on $slist_bg.uf
+settinglist.default.unfocused              $default_fg           on $slist_bg.uf
+settinglist.default.focused                $default_fg           on $slist_bg.f
+
+$description_fg = light gray
+settinglist.description.header             $description_fg,underline on $slist_bg.uf
+settinglist.description.unfocused          $description_fg           on $slist_bg.uf
+settinglist.description.focused            $description_fg           on $slist_bg.f
```

### Comparing `stig-0.8.3a0/stig/settings/rcfile.py` & `stig-0.9.0a0/stig/settings/rcfile.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/settings/defaults.py` & `stig-0.9.0a0/stig/settings/defaults.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,177 +11,193 @@
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 import os
 from xdg.BaseDirectory import xdg_config_home as XDG_CONFIG_HOME
 from xdg.BaseDirectory import xdg_cache_home  as XDG_CACHE_HOME
+from xdg.BaseDirectory import xdg_data_home  as XDG_DATA_HOME
+
+from .. import __appname__
+from ..views import (torrent, file, peer, tracker, setting)
+from ..client.sorters.torrent import TorrentSorter
+from ..client.sorters.peer import TorrentPeerSorter
+from ..client.sorters.tracker import TorrentTrackerSorter
+from ..client.sorters.setting import SettingSorter
+
+DEFAULT_RCFILE       = os.path.join(XDG_CONFIG_HOME, __appname__, 'rc')
+DEFAULT_HISTORY_FILE = os.path.join(XDG_DATA_HOME, __appname__, 'history')
+DEFAULT_GEOIP_DIR    = os.path.join(XDG_CACHE_HOME, __appname__)
+DEFAULT_THEME_FILE   = os.path.join(os.path.dirname(__file__), 'default.theme')
+
+
+def init_defaults(localcfg):
+    from ..utils.usertypes import (String, Int, Float, Bool, Path, Tuple, Option)
+
+    class SortOrder(str):
+        """String that is equal to the same string with '!' or '.' prepended"""
+        _invert_chars = ''.join(TorrentSorter.INVERT_CHARS)
+        def __eq__(self, other):
+            return self.lstrip(self._invert_chars) == other.lstrip(self._invert_chars)
+
+        # An overloaded __eq__() obligates an overloaded __hash__(), or
+        # instances won't be hashable.
+        def __hash__(self):
+            return super().__hash__()
+
+
+    def partial_sort_order(sortercls):
+        options = tuple(SortOrder(opt) for opt in sortercls.SORTSPECS)
+        return Tuple.partial(options=options, dedup=True)
+
+    localcfg.add('connect.host',
+                 constructor=String.partial(),
+                 default='localhost',
+                 description='Hostname or IP of Transmission RPC interface')
+    localcfg.add('connect.port',
+                 Int.partial(min=1, max=65535, prefix='none'),
+                 default=9091,
+                 description='Port of Transmission RPC interface')
+    localcfg.add('connect.path',
+                 String.partial(),
+                 default='/transmission/rpc',
+                 description='Path of Transmission RPC interface')
+    localcfg.add('connect.user',
+                 String.partial(),
+                 default='',
+                 description='Username to use for authentication with Transmission RPC interface')
+    localcfg.add('connect.password',
+                 String.partial(),
+                 default='',
+                 description='Password to use for authentication with Transmission RPC interface')
+    localcfg.add('connect.timeout',
+                 Float.partial(min=0),
+                 default=10,
+                 description='Number of seconds before connecting to Transmission RPC interface fails')
+    localcfg.add('connect.tls',
+                 Bool.partial(),
+                 default='off',
+                 description='Whether to connect via HTTPS to the Transmission RPC interface')
+
+    localcfg.add('columns.torrents',
+                 Tuple.partial(options=torrent.COLUMNS, aliases=torrent.ALIASES),
+                 default=('marked', 'size', 'downloaded', 'uploaded', 'ratio',
+                          'seeds', 'peers', 'status', 'eta', '%downloaded',
+                          'rate-down', 'rate-up', 'name'),
+                 description='Default columns in torrent lists')
+    localcfg.add('columns.peers',
+                 Tuple.partial(options=peer.COLUMNS, aliases=peer.ALIASES),
+                 default=('ip', 'client', 'country', '%downloaded', 'rate-down',
+                          'rate-up', 'rate-est', 'eta'),
+                 description='Default columns in peer lists')
+    localcfg.add('columns.files',
+                 Tuple.partial(options=file.COLUMNS, aliases=file.ALIASES),
+                 default=('marked', 'priority', '%downloaded', 'downloaded', 'size', 'name'),
+                 description='Default columns in file lists')
+    localcfg.add('columns.trackers',
+                 Tuple.partial(options=tracker.COLUMNS, aliases=tracker.ALIASES),
+                 default=('tier', 'domain', 'error', 'last-announce', 'next-announce',
+                          'leeches', 'seeds', 'downloads'),
+                 description='Default columns in tracker lists')
+    localcfg.add('columns.settings',
+                 Tuple.partial(options=setting.COLUMNS, aliases=setting.ALIASES),
+                 default=('name', 'value', 'default', 'description'),
+                 description='Default columns in setting lists')
+
+    localcfg.add('geoip',
+                 Bool.partial(),
+                 default=True,
+                 description='Whether to lookup peers\' country codes')
+    localcfg.add('geoip.dir',
+                 Path.partial(),
+                 default=DEFAULT_GEOIP_DIR,
+                 description='Where to cache the downloaded geolocation database')
+
+    localcfg.add('remove.max-hits',
+                 Int.partial(min=0),
+                 default=10,
+                 description=('Maximum number of torrents to remove without extra confirmation'))
+
+    localcfg.add('reverse-dns',
+                 Bool.partial(),
+                 default=True,
+                 description=('Whether to lookup peers\' host names'))
+
+    localcfg.add('sort.torrents',
+                 partial_sort_order(TorrentSorter),
+                 default=TorrentSorter.DEFAULT_SORT,
+                 description='List of sort orders in torrent lists')
+    localcfg.add('sort.peers',
+                 partial_sort_order(TorrentPeerSorter),
+                 default=TorrentPeerSorter.DEFAULT_SORT,
+                 description='List of sort orders in peer lists')
+    localcfg.add('sort.trackers',
+                 partial_sort_order(TorrentTrackerSorter),
+                 default=TorrentTrackerSorter.DEFAULT_SORT,
+                 description='List of sort orders in tracker lists')
+    localcfg.add('sort.settings',
+                 partial_sort_order(SettingSorter),
+                 default=SettingSorter.DEFAULT_SORT,
+                 description='List of sort orders in setting lists')
+
+    localcfg.add('tui.theme',
+                 Path.partial(),
+                 default=DEFAULT_THEME_FILE,
+                 description='Path to theme file'),
+    localcfg.add('tui.log.height',
+                 Int.partial(min=1),
+                 default=10,
+                 description='Maximum height of the log section')
+    localcfg.add('tui.log.autohide',
+                 Float.partial(min=0),
+                 default=10,
+                 description=('If the log is hidden, show it for this many seconds '
+                              'for new log entries before hiding it again'))
+    localcfg.add('tui.cli.history-file',
+                 Path.partial(),
+                 default=DEFAULT_HISTORY_FILE,
+                 description='Path to TUI command line history file')
+    localcfg.add('tui.cli.history-size',
+                 Int.partial(min=0),
+                 default=10000,
+                 description='Maximum number of lines in history file')
+    localcfg.add('tui.poll',
+                 Float.partial(min=0.1),
+                 default=5,
+                 description='Interval in seconds between TUI updates')
+
+    localcfg.add('unit.bandwidth',
+                 Option.partial(options=('bit', 'byte')),
+                 default='byte',
+                 description="Unit for bandwidth rates ('bit' or 'byte')")
+    localcfg.add('unitprefix.bandwidth',
+                 Option.partial(options=('metric', 'binary')),
+                 default='metric',
+                 description=("Unit prefix for bandwidth rates ('metric' or 'binary')"))
+
+    localcfg.add('unit.size',
+                 Option.partial(options=('bit', 'byte')),
+                 default='byte',
+                 description="Unit for file sizes ('bit' or 'byte')")
+    localcfg.add('unitprefix.size',
+                 Option.partial(options=('metric', 'binary')),
+                 default='binary',
+                 description=("Unit prefix for file sizes ('metric' or 'binary')"))
+
+    localcfg.add('tui.marked.on',
+                 String.partial(minlen=1, maxlen=1),
+                 default='●',
+                 description=("Character displayed in 'marked' column for marked "
+                              "list items (see 'mark' command)"))
+    localcfg.add('tui.marked.off',
+                 String.partial(minlen=1, maxlen=1),
+                 default=' ',
+                 description=("Character displayed in 'marked' column for unmarked "
+                              "list items (see 'mark' command)"))
 
-from .. import APPNAME
-from ..views import (torrentlist, filelist, peerlist, trackerlist)
-from ..client.sorters.tsorter import TorrentSorter
-from ..client.sorters.psorter import TorrentPeerSorter
-from ..client.sorters.trksorter import TorrentTrackerSorter
-
-DEFAULT_RCFILE        = os.path.join(XDG_CONFIG_HOME, APPNAME, 'rc')
-DEFAULT_HISTORY_FILE  = os.path.join(XDG_CACHE_HOME, APPNAME, 'history')
-DEFAULT_THEME_FILE    = os.path.join(os.path.dirname(__file__), 'default.theme')
-
-DEFAULT_TORRENT_SORT = ('name',)
-DEFAULT_PEER_SORT    = ('torrent',)
-DEFAULT_TRACKER_SORT = ('domain',)
-
-DEFAULT_TORRENT_COLUMNS = ('marked', 'size', 'downloaded', 'uploaded', 'ratio',
-                           'seeds', 'connections', 'status', 'eta', 'progress',
-                           'rate-down', 'rate-up', 'name')
-DEFAULT_FILE_COLUMNS    = ('marked', 'priority', 'progress', 'downloaded', 'size', 'name')
-DEFAULT_TRACKER_COLUMNS = ('tier', 'domain', 'state', 'error',
-                           'leeches', 'seeds', 'downloads',
-                           'last-announce', 'next-announce')
-
-from ..client.geoip import GEOIP_AVAILABLE
-if GEOIP_AVAILABLE:
-    DEFAULT_PEER_COLUMNS = ('client', 'country', 'ip', 'progress', 'rate-down',
-                            'rate-up', 'rate-est', 'eta')
-else:
-    DEFAULT_PEER_COLUMNS = ('client', 'ip', 'progress', 'rate-down', 'rate-up',
-                            'rate-est', 'eta', )
-
-
-def init_defaults(cfg):
-    from .types import (StringValue, IntegerValue, NumberValue, BooleanValue,
-                        PathValue, ListValue, SetValue, OptionValue)
-
-    class SortOrderValue(SetValue):
-        """SetValue that correctly validates inverted sort orders (e.g. '!name')"""
-        def __init__(self, sortercls, *args, **kwargs):
-            super().__init__(*args, options=tuple(sortercls.SORTSPECS), **kwargs)
-
-        def validate(self, names):
-            super().validate(name.strip('!.') for name in names)
-
-    cfg.load(
-        StringValue('srv.url', default='localhost:9091',
-                    description='URL of the Transmission RPC interface ([USER:PASSWORD@]HOST[:PORT])'),
-        NumberValue('srv.timeout', default=10, min=0,
-                    description=('Number of seconds before connecting '
-                                 'to Transmission daemon fails')),
-
-        SetValue('columns.torrents', default=DEFAULT_TORRENT_COLUMNS,
-                 options=torrentlist.COLUMNS,
-                 aliases=torrentlist.ALIASES,
-                 description='List of columns in new torrent lists'),
-        SetValue('columns.peers', default=DEFAULT_PEER_COLUMNS,
-                 options=peerlist.COLUMNS,
-                 aliases=peerlist.ALIASES,
-                 description='List of columns in new peer lists'),
-        SetValue('columns.files', default=DEFAULT_FILE_COLUMNS,
-                 options=filelist.COLUMNS,
-                 aliases=filelist.ALIASES,
-                 description='List of columns in new torrent file lists'),
-        SetValue('columns.trackers', default=DEFAULT_TRACKER_COLUMNS,
-                 options=trackerlist.COLUMNS,
-                 aliases=trackerlist.ALIASES,
-                 description='List of columns in new tracker lists'),
-
-        SortOrderValue(TorrentSorter, 'sort.torrents', default=DEFAULT_TORRENT_SORT,
-                       description='List of torrent list sort orders'),
-        SortOrderValue(TorrentPeerSorter, 'sort.peers', default=DEFAULT_PEER_SORT,
-                       description='List of peer list sort orders'),
-        SortOrderValue(TorrentTrackerSorter, 'sort.trackers', default=DEFAULT_TRACKER_SORT,
-                       description='List of tracker list sort orders'),
-
-        PathValue('tui.theme', default=DEFAULT_THEME_FILE,
-                  description='Path to theme file'),
-        IntegerValue('tui.log.height', default=10, min=1,
-                     description='Maximum height of the log section'),
-        NumberValue('tui.log.autohide', default=10, min=0,
-                    description=('If the log is hidden, show it for this many seconds '
-                                 'for new log entries before hiding it again')),
-        PathValue('tui.cli.history-file', default=DEFAULT_HISTORY_FILE,
-                  description='Path to TUI command line history file'),
-        PathValue('tui.cli.history-size', default=10000,
-                  description='Maximum number of lines in history file'),
-        NumberValue('tui.poll', default=5, min=0.1,
-                    description='Interval in seconds between TUI updates'),
-
-        OptionValue('unit.bandwidth', default='byte', options=('bit', 'byte'),
-                    description="Unit for bandwidth rates ('bit' or 'byte')"),
-        OptionValue('unitprefix.bandwidth', default='metric', options=('metric', 'binary'),
-                    description=("Unit prefix for bandwidth rates ('metric' or 'binary')")),
-
-        OptionValue('unit.size', default='byte', options=('bit', 'byte'),
-                    description="Unit for sizes ('bit' or 'byte')"),
-        OptionValue('unitprefix.size', default='binary', options=('metric', 'binary'),
-                    description=("Unit prefix for sizes ('metric' or 'binary')")),
-
-        StringValue('tui.marked.on', default='✔', minlen=1, maxlen=1,
-                    description=('Character displayed in "marked" column for marked '
-                                 'list items (see "mark" command)')),
-        StringValue('tui.marked.off', default=' ', minlen=1, maxlen=1,
-                    description=('Character displayed in "marked" column for unmarked '
-                                 'list items (see "mark" command)')),
-
-        IntegerValue('remove.max-hits', default=10, min=0,
-                     description=('Maximum number of torrents to remove without '
-                                  'getting extra user confirmation')),
-    )
-
-
-
-def init_server_defaults(cfg, settingsapi):
-    from .types_srv import (BooleanSrvValue, IntegerSrvValue, OptionSrvValue,
-                            PathSrvValue, PathIncompleteSrvValue,
-                            RateLimitSrvValue, PortSrvValue)
-
-    def mk(cls, name, setting, description, **kwargs):
-        getter = lambda: settingsapi[setting]
-        setter = getattr(settingsapi, 'set_'+setting)
-        return cls(name, getter=getter, setter=setter, description=description, **kwargs)
-
-    cfg.load(
-        mk(BooleanSrvValue, 'srv.utp', 'utp',
-           'Whether to use Micro Transport Protocol to mitigate latency issues'),
-        mk(BooleanSrvValue, 'srv.dht', 'dht',
-           'Whether to use Distributed Hash Tables to discover peers for public torrents'),
-        mk(BooleanSrvValue, 'srv.lpd', 'lpd',
-           'Whether to use Local Peer Discovery to discover peers for public torrents'),
-        mk(BooleanSrvValue, 'srv.pex', 'pex',
-           'Whether to use Peer Exchange to discover peers for public torrents'),
-
-        mk(PortSrvValue, 'srv.port', 'port',
-           'Port used to communicate with peers or "random" to use a random port',
-           min=1, max=65535),
-        mk(BooleanSrvValue, 'srv.port-forwarding', 'port_forwarding',
-           'Whether to instruct your router to forward the peer port via UPnP or NAT-PMP'),
-
-        mk(OptionSrvValue, 'srv.encryption', 'encryption',
-           'Protocol encryption policy; "required", "preferred" or "tolerated"',
-           options=('required', 'preferred', 'tolerated')),
-
-        mk(IntegerSrvValue, 'srv.limit.peers.global', 'peer_limit_global',
-           'Maximum number of connections for all torrents combined'),
-        mk(IntegerSrvValue, 'srv.limit.peers.torrent', 'peer_limit_torrent',
-           'Maximum number of connections for a single torrent'),
-
-        mk(RateLimitSrvValue, 'srv.limit.rate.up', 'rate_limit_up',
-           'Combined upload rate limit'),
-        mk(RateLimitSrvValue, 'srv.limit.rate.down', 'rate_limit_down',
-           'Combined download rate limit'),
-
-        mk(BooleanSrvValue, 'srv.part-files', 'part_files',
-           'Whether to append ".part" to incomplete file names'),
-        mk(PathSrvValue, 'srv.path.complete', 'path_complete',
-           'Where to put torrent files'),
-        mk(PathIncompleteSrvValue, 'srv.path.incomplete', 'path_incomplete',
-           'Where to put incomplete torrent files'),
-
-        mk(BooleanSrvValue, 'srv.autostart-torrents', 'autostart_torrents',
-           'Automatically start torrents when they are added'),
-    )
 
 
 DEFAULT_KEYMAP = (
     # Use some vi and emacs keybindings
     {'key': 'h',      'action': '<left>'},
     {'key': 'j',      'action': '<down>'},
     {'key': 'k',      'action': '<up>'},
@@ -190,59 +206,60 @@
     {'key': 'G',      'action': '<end>'},
     {'key': 'ctrl-n', 'action': '<down>'},
     {'key': 'ctrl-p', 'action': '<up>'},
     {'key': 'ctrl-f', 'action': '<right>'},
     {'key': 'ctrl-b', 'action': '<left>'},
 
     # Global TUI keys
-    {'context': 'main', 'key': 'q', 'action': 'quit'},
-    {'context': 'main', 'key': ':', 'action': 'tui show cli'},
+    {'context': 'main', 'key': 'q',     'action': 'quit'},
+    {'context': 'main', 'key': ':',     'action': 'tui show cli'},
+    {'context': 'main', 'key': 'alt-s', 'action': 'tab set'},
 
     # Help
     {'context': 'main', 'key': 'F1+c', 'action': 'tab help commands'},
     {'context': 'main', 'key': 'F1+s', 'action': 'tab help settings'},
     {'context': 'main', 'key': 'F1+k', 'action': 'tab help keymap'},
     {'context': 'main', 'key': 'F1+f', 'action': 'tab help filtering'},
     {'context': 'main', 'key': 'F1+r', 'action': 'tab help rcfile'},
     {'context': 'main', 'key': '?',    'action': '<F1>'},
 
     # Hide/Show TUI elements
-    {'context': 'main', 'key': 'meta-L', 'action': 'tui toggle log'},
-    {'context': 'main', 'key': 'meta-M', 'action': 'tui toggle main'},
-    {'context': 'main', 'key': 'meta-T', 'action': 'tui toggle topbar'},
-    {'context': 'main', 'key': 'meta-B', 'action': 'tui toggle bottombar'},
+    {'context': 'main', 'key': 'alt-L', 'action': 'tui toggle log'},
+    {'context': 'main', 'key': 'alt-M', 'action': 'tui toggle main'},
+    {'context': 'main', 'key': 'alt-T', 'action': 'tui toggle topbar'},
+    {'context': 'main', 'key': 'alt-B', 'action': 'tui toggle bottombar'},
 
     # Log messages
     {'context': 'main', 'key': 'ctrl-l',   'action': 'tui toggle log'},
     {'context': 'main', 'key': 'alt-l',    'action': 'log clear'},
     {'context': 'main', 'key': 'alt-pgup', 'action': 'log scroll page up'},
     {'context': 'main', 'key': 'alt-pgdn', 'action': 'log scroll page down'},
     {'context': 'main', 'key': 'alt-home', 'action': 'log scroll top'},
     {'context': 'main', 'key': 'alt-end',  'action': 'log scroll bottom'},
 
-    # Bandwidth limits
-    {'context': 'main', 'key': 'shift-up',    'action': 'set srv.limit.rate.down +=100kB'},
-    {'context': 'main', 'key': 'shift-down',  'action': 'set srv.limit.rate.down -=100kB'},
-    {'context': 'main', 'key': 'shift-right', 'action': 'set srv.limit.rate.up +=100kB'},
-    {'context': 'main', 'key': 'shift-left',  'action': 'set srv.limit.rate.up -=100kB'},
+    # Global bandwidth limits
+    {'context': 'main', 'key': 'shift-up',    'action': 'rate --quiet dn -- +=100kB global'},
+    {'context': 'main', 'key': 'shift-down',  'action': 'rate --quiet dn -- -=100kB global'},
+    {'context': 'main', 'key': 'shift-right', 'action': 'rate --quiet up -- +=100kB global'},
+    {'context': 'main', 'key': 'shift-left',  'action': 'rate --quiet up -- -=100kB global'},
 
     # Tab management
-    {'context': 'tabs', 'key': 'n',      'action': 'tab'},
-    {'context': 'tabs', 'key': 'd',      'action': 'tab --close'},
-    {'context': 'tabs', 'key': 'D',      'action': 'tab --close --focus left'},
-    {'context': 'tabs', 'key': 'meta-1', 'action': 'tab --focus 1'},
-    {'context': 'tabs', 'key': 'meta-2', 'action': 'tab --focus 2'},
-    {'context': 'tabs', 'key': 'meta-3', 'action': 'tab --focus 3'},
-    {'context': 'tabs', 'key': 'meta-4', 'action': 'tab --focus 4'},
-    {'context': 'tabs', 'key': 'meta-5', 'action': 'tab --focus 5'},
-    {'context': 'tabs', 'key': 'meta-6', 'action': 'tab --focus 6'},
-    {'context': 'tabs', 'key': 'meta-7', 'action': 'tab --focus 7'},
-    {'context': 'tabs', 'key': 'meta-8', 'action': 'tab --focus 8'},
-    {'context': 'tabs', 'key': 'meta-9', 'action': 'tab --focus 9'},
-    {'context': 'tabs', 'key': 'meta-0', 'action': 'tab --focus 10'},
+    {'context': 'tabs', 'key': 'n',     'action': 'tab'},
+    {'context': 'tabs', 'key': 'd',     'action': 'tab --close'},
+    {'context': 'tabs', 'key': 'D',     'action': 'tab --close --focus left'},
+    {'context': 'tabs', 'key': 'alt-1', 'action': 'tab --focus 1'},
+    {'context': 'tabs', 'key': 'alt-2', 'action': 'tab --focus 2'},
+    {'context': 'tabs', 'key': 'alt-3', 'action': 'tab --focus 3'},
+    {'context': 'tabs', 'key': 'alt-4', 'action': 'tab --focus 4'},
+    {'context': 'tabs', 'key': 'alt-5', 'action': 'tab --focus 5'},
+    {'context': 'tabs', 'key': 'alt-6', 'action': 'tab --focus 6'},
+    {'context': 'tabs', 'key': 'alt-7', 'action': 'tab --focus 7'},
+    {'context': 'tabs', 'key': 'alt-8', 'action': 'tab --focus 8'},
+    {'context': 'tabs', 'key': 'alt-9', 'action': 'tab --focus 9'},
+    {'context': 'tabs', 'key': 'alt-0', 'action': 'tab --focus 10'},
 
     # List torrents with different filters
     {'context': 'tabs', 'key': 'f a', 'action': 'tab ls active'},
     {'context': 'tabs', 'key': 'f A', 'action': 'tab ls !active'},
     {'context': 'tabs', 'key': 'f i', 'action': 'tab ls isolated --columns name,tracker,error'},
     {'context': 'tabs', 'key': 'f p', 'action': 'tab ls paused'},
     {'context': 'tabs', 'key': 'f P', 'action': 'tab ls !paused'},
@@ -259,16 +276,16 @@
     {'context': 'torrentlist', 'key': 's D',       'action': 'sort --add !dir'},
     {'context': 'torrentlist', 'key': 's e',       'action': 'sort --add eta'},
     {'context': 'torrentlist', 'key': 's E',       'action': 'sort --add !eta'},
     {'context': 'torrentlist', 'key': 's n',       'action': 'sort --add name'},
     {'context': 'torrentlist', 'key': 's N',       'action': 'sort --add !name'},
     {'context': 'torrentlist', 'key': 's o',       'action': 'sort --add ratio'},
     {'context': 'torrentlist', 'key': 's O',       'action': 'sort --add !ratio'},
-    {'context': 'torrentlist', 'key': 's p',       'action': 'sort --add progress'},
-    {'context': 'torrentlist', 'key': 's P',       'action': 'sort --add !progress'},
+    {'context': 'torrentlist', 'key': 's p',       'action': 'sort --add %downloaded'},
+    {'context': 'torrentlist', 'key': 's P',       'action': 'sort --add !%downloaded'},
     {'context': 'torrentlist', 'key': 's r',       'action': 'sort --add rate'},
     {'context': 'torrentlist', 'key': 's R',       'action': 'sort --add !rate'},
     {'context': 'torrentlist', 'key': 's s',       'action': 'sort --add seeds'},
     {'context': 'torrentlist', 'key': 's S',       'action': 'sort --add !seeds'},
     {'context': 'torrentlist', 'key': 's t',       'action': 'sort --add tracker'},
     {'context': 'torrentlist', 'key': 's T',       'action': 'sort --add !tracker'},
     {'context': 'torrentlist', 'key': 's z',       'action': 'sort --add size'},
@@ -293,20 +310,18 @@
     # Peer list actions
     {'context': 'peerlist', 'key': 's c',       'action': 'sort --add country'},
     {'context': 'peerlist', 'key': 's C',       'action': 'sort --add !country'},
     {'context': 'peerlist', 'key': 's d',       'action': 'sort --add rate-down'},
     {'context': 'peerlist', 'key': 's D',       'action': 'sort --add !rate-down'},
     {'context': 'peerlist', 'key': 's e',       'action': 'sort --add eta'},
     {'context': 'peerlist', 'key': 's E',       'action': 'sort --add !eta'},
-    {'context': 'peerlist', 'key': 's i',       'action': 'sort --add ip'},
-    {'context': 'peerlist', 'key': 's I',       'action': 'sort --add !ip'},
     {'context': 'peerlist', 'key': 's l',       'action': 'sort --add client'},
     {'context': 'peerlist', 'key': 's L',       'action': 'sort --add !client'},
-    {'context': 'peerlist', 'key': 's p',       'action': 'sort --add progress'},
-    {'context': 'peerlist', 'key': 's P',       'action': 'sort --add !progress'},
+    {'context': 'peerlist', 'key': 's p',       'action': 'sort --add %downloaded'},
+    {'context': 'peerlist', 'key': 's P',       'action': 'sort --add !%downloaded'},
     {'context': 'peerlist', 'key': 's u',       'action': 'sort --add rate-up'},
     {'context': 'peerlist', 'key': 's U',       'action': 'sort --add !rate-up'},
     {'context': 'peerlist', 'key': 's s',       'action': 'sort --add rate-est'},
     {'context': 'peerlist', 'key': 's S',       'action': 'sort --add !rate-est'},
     {'context': 'peerlist', 'key': 's r',       'action': 'sort --add rate'},
     {'context': 'peerlist', 'key': 's R',       'action': 'sort --add !rate'},
     {'context': 'peerlist', 'key': 's t',       'action': 'sort --add torrent'},
@@ -339,17 +354,32 @@
     {'context': 'trackerlist', 'key': 's c',     'action': 'sort --add leeches'},
     {'context': 'trackerlist', 'key': 's C',     'action': 'sort --add !leeches'},
     {'context': 'trackerlist', 'key': 's s',     'action': 'sort --add seeds'},
     {'context': 'trackerlist', 'key': 's S',     'action': 'sort --add !seeds'},
 
     {'context': 'trackerlist', 'key': 's e',     'action': 'sort --add error'},
     {'context': 'trackerlist', 'key': 's E',     'action': 'sort --add !error'},
-    {'context': 'trackerlist', 'key': 's t',     'action': 'sort --add state'},
-    {'context': 'trackerlist', 'key': 's T',     'action': 'sort --add !state'},
+    {'context': 'trackerlist', 'key': 's t',     'action': 'sort --add status'},
+    {'context': 'trackerlist', 'key': 's T',     'action': 'sort --add !status'},
 
     {'context': 'trackerlist', 'key': 's ,',     'action': 'sort --reset'},
     {'context': 'trackerlist', 'key': 's .',     'action': 'sort --none'},
 
     # Tracker actions
     {'context': 'tracker', 'key': 'enter',       'action': 'tab summary'},
     {'context': 'tracker', 'key': 'alt-enter',   'action': 'tab filelist'},
+
+    # Setting list actions
+    {'context': 'settinglist', 'key': 's n', 'action': 'sort --add name'},
+    {'context': 'settinglist', 'key': 's N', 'action': 'sort --add !name'},
+    {'context': 'settinglist', 'key': 's v', 'action': 'sort --add value'},
+    {'context': 'settinglist', 'key': 's V', 'action': 'sort --add !value'},
+    {'context': 'settinglist', 'key': 's d', 'action': 'sort --add default'},
+    {'context': 'settinglist', 'key': 's D', 'action': 'sort --add !default'},
+    {'context': 'settinglist', 'key': 's c', 'action': 'sort --add description'},
+    {'context': 'settinglist', 'key': 's C', 'action': 'sort --add !description'},
+    {'context': 'settinglist', 'key': 's ,', 'action': 'sort --reset'},
+    {'context': 'settinglist', 'key': 's .', 'action': 'sort --none'},
+
+    # Setting actions
+    {'context': 'setting', 'key': 'ctrl-r', 'action': 'reset'},
 )
```

### Comparing `stig-0.8.3a0/stig/client/geoip.py` & `stig-0.9.0a0/stig/commands/cli/_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,9 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-try:
-    import GeoIP
-
-except ImportError:
-    GEOIP_AVAILABLE = False
-    def country_code(addr):
-        return '?'
-
-else:
-    GEOIP_AVAILABLE = True
-    _geoip = GeoIP.new(GeoIP.GEOIP_MEMORY_CACHE)
-    def country_code(addr):
-        return _geoip.country_code_by_addr(addr) or '?'
+def clear_line():
+    print('\x1b[2K\x1b[1`', end='', flush=True)
```

### Comparing `stig-0.8.3a0/stig/client/api.py` & `stig-0.9.0a0/stig/client/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,120 +8,107 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
-import weakref
+import asyncio
 
-from . import convert
 from .utils import SleepUneasy
 
 from .aiotransmission.rpc import TransmissionRPC
 from .aiotransmission.api_status import StatusAPI
 from .aiotransmission.api_settings import SettingsAPI
 from .aiotransmission.api_torrent import TorrentAPI
 
 from .poll import RequestPoller
 from .trequestpool import TorrentRequestPool
-from .errors import *
 from .utils import lazy_property
+from . import errors
 
 
-class API(convert.bandwidth_mixin, convert.size_mixin):
-    """Provide and manage *API classes as singletons
+class API():
+    """
+    Provide and manage *API classes as singletons
 
-    A convenience class that creates instances of TransmissionRPC, TorrentAPI,
-    StatusAPI, TorrentRequestPool and TorrentCounters in a lazy manner on
-    demand.
+    A convenience class that provides instances of TransmissionRPC, TorrentAPI,
+    StatusAPI, TorrentRequestPool and TorrentCounters and all ClientError
+    exceptions in one object. All instances except TransmissionRPC are created
+    lazily on demand.
     """
 
     # Make errors available without having to import them everywhere
-    ClientError     = ClientError
-    ConnectionError = ConnectionError
-    RPCError        = RPCError
-    AuthError       = AuthError
-    URLParserError  = URLParserError
-
-    def __init__(self, url, interval=1, loop=None):
-        if loop is None:
-            raise TypeError('Missing argument: loop')
-        self.loop = loop
-        self._url = url
-        self._interval = interval
+    ClientError     = errors.ClientError
+    ConnectionError = errors.ConnectionError
+    RPCError        = errors.RPCError
+    AuthError       = errors.AuthError
+
+    def __init__(self, host='localhost', port=9091, *, tls=False, user=None,
+                 password=None, path='/transmission/rpc', loop=None, interval=1):
+        self.loop = loop if loop is not None else asyncio.get_event_loop()
+        self._rpc = TransmissionRPC(host=host, port=port, tls=tls, user=user,
+                                    password=password, loop=self.loop, path=path)
         self._pollers = []
         self._manage_pollers_interval = SleepUneasy(loop=self.loop)
+        self.interval = interval
 
     @property
-    def url(self):
-        """URL to API interface"""
-        if self.created('rpc'):
-            return self.rpc.url
-        return self._url
-
-    @url.setter
-    def url(self, url):
-        self._url = url
-        if self.created('rpc'):
-            self.rpc.url = url
+    def rpc(self):
+        """TransmissionRPC singleton"""
+        return self._rpc
 
     @property
     def interval(self):
         """Delay between polls of all pollers"""
         return self._interval
 
     @interval.setter
     def interval(self, interval):
-        self._interval = interval
+        self._interval = float(interval)
         for poller in self._existing_pollers:
-            poller.interval = interval
+            poller.interval = self._interval
 
 
     def created(self, prop):
         """Whether property `prop` was created"""
         return hasattr(self, prop+'_created')
 
-    @lazy_property(after_creation=lambda self: setattr(self, 'rpc_created', True))
-    def rpc(self):
-        """TransmissionRPC singleton"""
-        log.debug('Creating RPC singleton')
-        return TransmissionRPC(self._url, loop=self.loop)
-
     @lazy_property(after_creation=lambda self: setattr(self, 'torrent_created', True))
     def torrent(self):
         """TorrentAPI singleton"""
         log.debug('Creating TorrentAPI singleton')
         return TorrentAPI(self.rpc)
 
     @lazy_property(after_creation=lambda self: setattr(self, 'status_created', True))
     def status(self):
         """StatusAPI singleton"""
         log.debug('Creating StatusAPI singleton')
-        return StatusAPI(self, interval=self._interval, autoconnect=True)
+        return StatusAPI(self, interval=self._interval)
 
     @lazy_property(after_creation=lambda self: setattr(self, 'settings_created', True))
     def settings(self):
         """SettingsAPI singleton"""
         log.debug('Creating SettingsAPI singleton')
-        return SettingsAPI(self, interval=self._interval, autoconnect=True)
+        return SettingsAPI(self, interval=self._interval)
 
     @lazy_property(after_creation=lambda self: setattr(self, 'treqpool_created', True))
     def treqpool(self):
         """TorrentRequestPool singleton"""
         log.debug('Creating TorrentRequestPool singleton')
-        return TorrentRequestPool(self, interval=self._interval, autoconnect=True)
+        return TorrentRequestPool(self, interval=self._interval)
 
 
     def create_poller(self, *args, interval=None, loop=None, **kwargs):
-        """Create, start and return custom RequestPoller instance
+        """
+        Create, start and return custom RequestPoller instance
 
         All arguments are used to create the poller, except for `interval` and
-        `loop`, which are ignored and replaced with this object's `interval`
-        and `loop` attributes so all pollers have the same interval.
+        `loop`, which are ignored and replaced with this object's `interval` and
+        `loop` attributes so all pollers have the same interval.
 
         The RequestPoller instance is treated like all other pollers, i.e. it
         is polled when `poll` is called, its interval is changed when
         `interval` is set, etc.
         """
         poller = RequestPoller(*args, interval=self.interval, loop=self.loop, **kwargs)
         self._pollers.append(poller)
@@ -190,15 +177,16 @@
         """Whether pollers are running or not"""
         pollers = tuple(self._existing_pollers)
         if not pollers:
             return False
         return pollers[0].running
 
     def poll(self):
-        """Poll all created and running pollers immediately
+        """
+        Poll all created and running pollers immediately
 
         This also resets the interval - the next polls are made `interval`
         seconds later.
         """
         for poller in self._existing_pollers:
             if poller.running:
                 poller.poll()
```

### Comparing `stig-0.8.3a0/stig/client/__init__.py` & `stig-0.9.0a0/stig/client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-# External dependencies
-from ..utils import (NumberFloat, NumberInt)
-
-
 from .errors import *
 from .constants import *
 
-from .utils import Response
+from .utils import (Response, URL)
+
+from .geoip import GeoIP
+geoip = GeoIP()
 
-from .sorters.tsorter import TorrentSorter
-from .sorters.psorter import TorrentPeerSorter
-from .sorters.trksorter import TorrentTrackerSorter
-
-from .filters.tfilter import TorrentFilter
-from .filters.ffilter import TorrentFileFilter
-from .filters.pfilter import TorrentPeerFilter
-from .filters.trkfilter import TorrentTrackerFilter
+from .sorters.torrent import TorrentSorter
+from .sorters.peer import TorrentPeerSorter
+from .sorters.tracker import TorrentTrackerSorter
+from .sorters.setting import SettingSorter
+
+from .filters.torrent import TorrentFilter
+from .filters.file import TorrentFileFilter
+from .filters.peer import TorrentPeerFilter
+from .filters.tracker import TorrentTrackerFilter
 
 from .poll import RequestPoller
 from .trequestpool import TorrentRequestPool
 
 from .aiotransmission.rpc import TransmissionRPC
 from .aiotransmission.api_status import StatusAPI
 from .aiotransmission.api_settings import SettingsAPI
```

### Comparing `stig-0.8.3a0/stig/client/ttypes.py` & `stig-0.9.0a0/stig/client/ttypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,68 +13,59 @@
 
 # The TYPES dictionary at the end of this file maps Torrent key names to
 # types.  Every Torrent key must have a type, even if it's just a no-op
 # (`lambda obj: obj`).
 #
 # A type is any callable that converts a single value to the appropriate object.
 #
-# Types are used to convert values from the server by instantiating them
-# normally (e.g. `NumberFloat(1234567)`) and from the user by using the class
-# method `from_string` (e.g. `NumberFloat.from_string('1.3GB')`). Not all types
-# must provide a `from_string` class method (e.g. 'files').
-
+# Types are used to convert values from the server (e.g. `Float(1234567)`) and
+# for some types from the user as strings (e.g. `Float('1.3GB')`).
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 from collections import abc
 import os
 import re
 import time
 
-from . import (NumberFloat, NumberInt)
-from . import constants as const
-from . import convert
-from . import utils
+from .utils import (URL, Float, Int, convert, const)
 
 
-def _rate_limit(limit):
+def _limit_rate(limit):
     return const.UNLIMITED if limit is None else convert.bandwidth(limit, unit='byte')
 
 
 def _calc_percent(a, b):
     try:
         return a / b * 100
     except ZeroDivisionError:
         return 0
 
 
-class Percent(NumberFloat):
-    def __new__(cls, *args, **kwargs):
-        kwargs['unit'] = '%'
-        return super().__new__(cls, *args, **kwargs)
+Percent = Float.partial(unit='%')
 
 
-class Ratio(NumberFloat):
+class Ratio(Float):
     """A Torrent's upload/download ratio as a float"""
     INFINITE = float('inf')
     NOT_APPLICABLE = -1
     def __str__(self):
         if self == self.INFINITE:
             return '∞'
         elif self == self.NOT_APPLICABLE:
             return ''
         else:
             return super().without_unit
 
 
-class Count(NumberInt):
+class Count(Int):
     UNKNOWN = -1
     def __str__(self):
-        return '?' if self < 0 else super().__str__()
+        return '?' if self == self.UNKNOWN else super().without_unit
 
 
 class Status(tuple):
     """A Torrent's status as string"""
 
     IDLE      = 'idle'
     DOWNLOAD  = 'downloading'
@@ -109,20 +100,14 @@
     """String with smart comparison capabilities
 
     Adds the <, >, <=, >= operators that compare length of strings and makes
     comparison case-insensitive if the other string consists solely of
     lower-case characters.
     """
 
-    def __new__(cls, string):
-        # Combine characters with diacritical marks ("a˚" -> "å") so len()
-        # reports the correct length.
-        # http://www.unicode.org/faq/char_combmark.html
-        return super().__new__(cls, unicodedata.normalize('NFC', string))
-
     def __cmp(self, op, other):
         if not isinstance(other, str):
             return NotImplemented
 
         # Do case-insensitive comparison?
         # Make copies to avoid infinite recursion.
         o = str(other)
@@ -219,17 +204,17 @@
             if abs_secs >= amount:
                 num = self/amount
 
                 # Small numbers get a sub-unit, for example '1d15h'
                 if 1 <= abs_secs/amount < 10 and i < len(SECONDS)-1:
                     subunit, subamount = SECONDS[i+1]
                     if num >= 0:
-                        subnum = abs( ((num%1) * amount) / subamount )
+                        subnum = abs(((num % 1) * amount) / subamount)
                     else:
-                        subnum = abs( ((num%-1) * amount) / subamount )
+                        subnum = abs(((num % -1) * amount) / subamount)
 
                     if subnum >= 1:
                         return '%d%s%d%s' % (int(num), unit, int(subnum), subunit)
 
                 return '%d%s' % (int(num), unit)
 
     @property
@@ -330,17 +315,17 @@
             return 'now'
         elif self == self.SOON:
             return 'soon'
         elif self == self.NEVER:
             return 'never'
 
         abs_delta = abs(self - time.time())
-        if abs_delta < 120:     # <= 2 minutes
+        if abs_delta < 120:      # <= 2 minutes
             frmt = '%H:%M:%S'
-        elif abs_delta < 86400: # <= 1 day
+        elif abs_delta < 86400:  # <= 1 day
             frmt = '%H:%M'
         else:
             frmt = '%Y-%m-%d'
         return time.strftime(frmt, time.localtime(self))
 
     @property
     def full(self):
@@ -405,65 +390,78 @@
     def __lt__(self, other): return int(self) < int(other)
     def __gt__(self, other): return int(self) > int(other)
     def __le__(self, other): return int(self) <= int(other)
     def __ge__(self, other): return int(self) >= int(other)
     def __int__(self): return self.STR2INT[self]
     def __repr__(self): return '<%s %r>' % (type(self).__name__, str(self))
 
+
 class TorrentFile(abc.Mapping):
     """Mapping that holds the values of a single file in a torrent"""
 
     # Distinguish subtrees from files without comparing classes everywhere
     nodetype = 'leaf'
 
     TYPES = {
-        'tid'             : int,
-        'id'              : int,
+        'id'              : lambda val: val,
+        'tid'             : lambda val: val,
         'name'            : SmartCmpStr,
         'path'            : Path,
+        'location'        : Path,
         'size-total'      : lambda size: convert.size(size, unit='byte'),
         'size-downloaded' : lambda size: convert.size(size, unit='byte'),
         'is-wanted'       : bool,
         'priority'        : TorrentFilePriority,
-        'progress'        : Percent,
+        '%downloaded'     : Percent,
     }
 
     _MODIFIERS = {
-        'tid'             : lambda raw: raw['tid'],
         'id'              : lambda raw: raw['id'],
+        'tid'             : lambda raw: raw['tid'],
         'name'            : lambda raw: raw['name'],
         'path'            : lambda raw: os.sep.join(raw['path']),
+        'location'        : lambda raw: raw['location'],
         'size-total'      : lambda raw: raw['size-total'],
         'size-downloaded' : lambda raw: raw['size-downloaded'],
         'is-wanted'       : lambda raw: raw['is-wanted'],
         'priority'        : lambda raw: 'off' if not raw['is-wanted'] else raw['priority'],
-        'progress'        : lambda raw: _calc_percent(raw['size-downloaded'], raw['size-total']),
+        '%downloaded'     : lambda raw: _calc_percent(raw['size-downloaded'], raw['size-total']),
     }
 
-    def __init__(self, tid, id, name, path, size_total, size_downloaded, is_wanted, priority):
-        self._raw = {'tid': tid, 'id': id, 'name': name, 'path': path,
+    def __init__(self, tid, id, name, path, location, size_total, size_downloaded, is_wanted, priority):
+        self._raw = {'tid': tid, 'id': id, 'name': name, 'path': path, 'location': location,
                      'is-wanted': is_wanted, 'priority': priority,
                      'size-total': size_total, 'size-downloaded': size_downloaded}
         self._cache = {}
 
     def __getitem__(self, key):
         if key not in self._cache:
             val = self._MODIFIERS[key](self._raw)
-            self._cache[key] = self.TYPES[key](val)
+            typ = self.TYPES.get(key)
+            if typ is not None:
+                self._cache[key] = typ(val)
+            else:
+                self._cache[key] = val
         return self._cache[key]
 
     def update(self, raw):
         self._raw.update(raw)
-        try:
-            for k in raw:
-                del self._cache[k]
-            if 'size-downloaded' in raw:
-                del self._cache['progress']
-        except KeyError:
-            pass
+        cache = self._cache
+        for key,new_value in raw.items():
+            cached_value = cache.get(key)
+            if cached_value is not None and cached_value != new_value:
+                del cache[key]
+
+        # %downloaded is never in raw because it is calculated from
+        # size-downloaded and size-total
+        if 'size-downloaded' in raw:
+            try:
+                del cache['%downloaded']
+            except KeyError:
+                pass
 
     def __repr__(self): return '<{} {!r}>'.format(type(self).__name__, self['name'])
     def __iter__(self): return iter(self.TYPES)
     def __len__(self): return len(self.TYPES)
 
 
 from . import base
@@ -524,81 +522,84 @@
                 eta = size_remaining / rate
 
     return rate, eta
 
 from . import geoip
 class TorrentPeer(abc.Mapping):
     TYPES = {
-        'id'        : lambda val: val,
-        'tid'       : lambda val: val,
-        'tname'     : SmartCmpStr,
-        'tsize'     : lambda size: convert.size(size, unit='byte'),
-        'ip'        : str,
-        'port'      : int,
-        'client'    : SmartCmpStr,
-        'country'   : SmartCmpStr,
-        'progress'  : Percent,
-        'rate-up'   : lambda rate: convert.bandwidth(rate, unit='byte'),
-        'rate-down' : lambda rate: convert.bandwidth(rate, unit='byte'),
-        'eta'       : Timedelta,
-        'rate-est'  : lambda rate: convert.bandwidth(rate, unit='byte'),
+        'id'          : lambda val: val,
+        'tid'         : lambda val: val,
+        'tname'       : SmartCmpStr,
+        'tsize'       : lambda size: convert.size(size, unit='byte'),
+        'ip'          : str,
+        'port'        : int,
+        'client'      : SmartCmpStr,
+        'country'     : SmartCmpStr,
+        '%downloaded' : Percent,
+        'rate-up'     : lambda rate: convert.bandwidth(rate, unit='byte'),
+        'rate-down'   : lambda rate: convert.bandwidth(rate, unit='byte'),
+        'eta'         : Timedelta,
+        'rate-est'    : lambda rate: convert.bandwidth(rate, unit='byte'),
     }
 
     _MODIFIERS = {
-        'id'      : lambda p: hash((p['tid'], p['ip'], p['port'])),
+        'id'      : lambda p: (p['tid'], p['ip'], p['port']),
         'country' : lambda p: geoip.country_code(p['ip']) or '?',
     }
 
-    def __init__(self, tid, tname, tsize, ip, port, client, progress, rate_up, rate_down):
+    def __init__(self, tid, tname, tsize, ip, port, client, pdownloaded, rate_up, rate_down):
         self._dct = {'tid': tid, 'tname': tname, 'tsize': tsize,
-                     'ip': ip, 'port': port, 'client': client, 'progress': progress,
+                     'ip': ip, 'port': port, 'client': client, '%downloaded': pdownloaded,
                      'rate-up': rate_up, 'rate-down': rate_down}
         self._cache = {}
 
     def __getitem__(self, key):
         if key not in self._cache:
             if key in ('eta', 'rate-est'):
-                rate, eta = _guess_peer_rate_and_eta(self['id'], self['progress'] / 100, self['tsize'])
+                rate, eta = _guess_peer_rate_and_eta(self['id'], self['%downloaded'] / 100, self['tsize'])
                 self._cache['rate-est'] = self.TYPES['rate-est'](rate)
                 self._cache['eta'] = self.TYPES['eta'](eta)
 
             else:
                 if key in self._MODIFIERS:
                     val = self._MODIFIERS[key](self._dct)
                 else:
                     val = self._dct[key]
                 self._cache[key] = self.TYPES[key](val)
         return self._cache[key]
 
+    def clearcache(self):
+        self._cache.clear()
+
     def __repr__(self): return '<{} #{}, {}>'.format(type(self).__name__, self['tid'], self['ip'])
     def __iter__(self): return iter(self.TYPES)
     def __len__(self): return len(self.TYPES)
 
 
 
 class TorrentTracker(abc.Mapping):
-    def _validate_tracker_state(string):
+    def _validate_tracker_status(string):
         if string not in ('stopped', 'idle', 'queued', 'announcing', 'scraping'):
-            raise TypeError('Invalid tracker state: %r' % string)
+            raise ValueError('Invalid tracker status: %r' % string)
         else:
             return SmartCmpStr(string)
 
     TYPES = {
+        'id'                 : lambda val: val,
         'tid'                : int,
         'tname'              : SmartCmpStr,
-        'id'                 : lambda val: val,
         'tier'               : int,
 
-        'url-announce'       : utils.URL,
-        'url-scrape'         : lambda url: utils.URL(url) if url else '',
+        'url-announce'       : URL,
+        'url-scrape'         : URL,
         'domain'             : SmartCmpStr,
 
-        'state-announce'     : _validate_tracker_state,
-        'state-scrape'       : _validate_tracker_state,
-        'state'              : _validate_tracker_state,
+        'status-announce'    : _validate_tracker_status,
+        'status-scrape'      : _validate_tracker_status,
+        'status'             : _validate_tracker_status,
 
         'error-announce'     : SmartCmpStr,
         'error-scrape'       : SmartCmpStr,
         'error'              : SmartCmpStr,
 
         'count-downloads'    : Count,
         'count-leeches'      : Count,
@@ -606,40 +607,38 @@
 
         'time-last-announce' : Timestamp,
         'time-next-announce' : Timestamp,
         'time-last-scrape'   : Timestamp,
         'time-next-scrape'   : Timestamp,
     }
 
-    _GENERATORS = {
+    _MODIFIERS = {
         'id'     : lambda self: hash((self['tid'], self['url-announce'])),
         'domain' : lambda self: self['url-announce'].domain,
-        'state'  : lambda self: (self['state-scrape'] if self['state-announce'] == 'idle'
-                                 else self['state-announce']),
+        'status' : lambda self: (self['status-scrape'] if self['status-announce'] == 'idle'
+                                 else self['status-announce']),
         'error'  : lambda self: ('Announce error: %s' % self['error-announce']
                                  if self['error-announce'] else
                                  'Scrape error: %s' % self['error-scrape']
                                  if self['error-scrape'] else '')
     }
 
     def __init__(self, trkdict):
         self._dct = trkdict
         self._cache = {}
 
     def __getitem__(self, key):
         cache = self._cache
         if key not in self._cache:
-            types = self.TYPES
-            generators = self._GENERATORS
-
-            if key in generators:
-                val = generators[key](self)
+            modifier = self._MODIFIERS.get(key)
+            if modifier is not None:
+                val = modifier(self)
             else:
                 val = self._dct[key]
-            cache[key] = types[key](val)
+            cache[key] = self.TYPES[key](val)
 
         return cache[key]
 
     def __repr__(self): return '<%s %s>' % (type(self).__name__, self['url-announce'])
     def __iter__(self): return iter(self.TYPES)
     def __len__(self): return len(self.TYPES)
 
@@ -652,25 +651,25 @@
     'ratio'                        : Ratio,
     'status'                       : Status,
     'path'                         : Path,
     'private'                      : bool,
     'comment'                      : SmartCmpStr,
     'creator'                      : SmartCmpStr,
     'magnetlink'                   : str,
-    'count-pieces'                 : NumberInt,
+    'count-pieces'                 : Int,
 
     '%downloaded'                  : Percent,
     '%uploaded'                    : Percent,
     '%metadata'                    : Percent,
     '%verified'                    : Percent,
     '%available'                   : Percent,
 
-    'peers-connected'              : NumberInt,
-    'peers-uploading'              : NumberInt,
-    'peers-downloading'            : NumberInt,
+    'peers-connected'              : Int,
+    'peers-uploading'              : Int,
+    'peers-downloading'            : Int,
     'peers-seeding'                : Count,
 
     'timespan-eta'                 : Timedelta,
     'timespan-seeding'             : Timedelta,
     'timespan-downloading'         : Timedelta,
     'time-created'                 : Timestamp,
     'time-added'                   : Timestamp,
@@ -678,16 +677,16 @@
     'time-activity'                : Timestamp,
     'time-completed'               : Timestamp,
     'time-manual-announce-allowed' : Timestamp,
 
     'rate-down'                    : lambda rate: convert.bandwidth(rate, unit='byte'),
     'rate-up'                      : lambda rate: convert.bandwidth(rate, unit='byte'),
 
-    'rate-limit-down'              : _rate_limit,
-    'rate-limit-up'                : _rate_limit,
+    'limit-rate-down'              : _limit_rate,
+    'limit-rate-up'                : _limit_rate,
 
     'size-final'                   : lambda size: convert.size(size, unit='byte'),
     'size-total'                   : lambda size: convert.size(size, unit='byte'),
     'size-downloaded'              : lambda size: convert.size(size, unit='byte'),
     'size-uploaded'                : lambda size: convert.size(size, unit='byte'),
     'size-available'               : lambda size: convert.size(size, unit='byte'),
     'size-left'                    : lambda size: convert.size(size, unit='byte'),
```

### Comparing `stig-0.8.3a0/stig/client/aiotransmission/rpc.py` & `stig-0.9.0a0/stig/client/aiotransmission/rpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,360 +11,416 @@
 
 """Low-level communication with the Transmission daemon"""
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
 import asyncio
-import aiohttp
 import json
 import textwrap
 from blinker import Signal
-from urllib.parse import urlsplit
-import re
 import warnings
 import async_timeout
 
-from ..errors import (URLParserError, ConnectionError, RPCError, AuthError, ClientError)
-from ..utils import URL
+from ..errors import (ConnectionError, TimeoutError, RPCError, AuthError, ClientError)
 
 
 AUTH_ERROR_CODE = 401
 CSRF_ERROR_CODE = 409
 CSRF_HEADER = 'X-Transmission-Session-Id'
 TIMEOUT = 10
 
 
-class TransmissionURL(URL):
-    DEFAULT = URL('http://localhost:9091/transmission/rpc')
-
-    def __new__(cls, url=str(DEFAULT)):
-        obj = super().__new__(cls, url)
-
-        # Fill in defaults
-        for attr in ('scheme', 'host', 'port', 'path'):
-            if getattr(obj, attr) is None:
-                setattr(obj, attr, getattr(cls.DEFAULT, attr))
-
-        return obj
-
-
 class TransmissionRPC():
-    """Low-level AsyncIO Transmission RPC communication
+    """
+    Low-level AsyncIO Transmission RPC communication
 
     This class handles connecting to a Transmission daemon via the RPC
     interface.  It does not implement the RPC protocol, only basic things like
-    authentication, sending requests and receiving responses.  High-level RPC
+    authentication, sending requests and receiving responses.  High-level RPCs
     are done in the *API classes.
     """
 
-    def __init__(self, url='localhost:9091', loop=None):
-        # Use double underscores because TransmissionAPI inherits from this
-        # class; this way, we don't have to worry about name collisions.
+    def __init__(self, host='localhost', port=9091, *, tls=False, user='',
+                 password='', path='/transmission/rpc', enabled=True, loop=None):
         self.loop = loop if loop is not None else asyncio.get_event_loop()
-        self.__url = TransmissionURL(url)
-        self.__headers = {'content-type': 'application/json'}
-        self.__session = None
-        self.__connect_exception = None
-        self.__connection_lock = asyncio.Lock(loop=loop)
-        self.__request_lock = asyncio.Lock(loop=loop)
-        self.__connection_tested = False
-        self.__timeout = TIMEOUT
-        self.__version = None
-        self.__rpcversion = None
-        self.__rpcversionmin = None
-        self.__on_connecting = Signal()
-        self.__on_connected = Signal()
-        self.__on_disconnected = Signal()
-        self.__on_error = Signal()
+        self._host = host
+        self._port = port
+        self._path = path
+        self._tls = tls
+        self._user = user
+        self._password = password
+        self._headers = {'content-type': 'application/json'}
+        self._session = None
+        self._enabled_event = asyncio.Event(loop=loop)
+        self.enabled = enabled
+        self._request_lock = asyncio.Lock(loop=loop)
+        self._connecting_lock = asyncio.Lock(loop=loop)
+        self._connection_tested = False
+        self._connection_exception = None
+        self._timeout = TIMEOUT
+        self._version = None
+        self._rpcversion = None
+        self._rpcversionmin = None
+        self._on_connecting = Signal()
+        self._on_connected = Signal()
+        self._on_disconnected = Signal()
+        self._on_error = Signal()
 
     def __del__(self, _warnings=warnings):
-        if self.__session is not None and not self.__session.closed:
+        if self._session is not None and not self._session.closed:
             _warnings.warn('disconnect() wasn\'t called', ResourceWarning)
-            asyncio.ensure_future(self.__session.close())
+            asyncio.ensure_future(self._session.close())
 
     def on(self, signal, callback, autoremove=True):
-        """Register `callback` for `signal`
+        """
+        Register `callback` for `signal`
 
         signal: 'connecting', 'connected', 'disconnected' or 'error'
-        callback: a callable that receives the RPC URL and, for 'error', the
-                  exception
+        callback: a callable that receives this instance as a positional
+                  argument and, in case of the 'error' signal, the exception as
+                  a keyword argument with the name 'error'
 
         Callbacks are automatically unsubscribed when they are
         garbage-collected.
         """
         try:
-            # Attributes with '__' become '_Classname__attribute'
-            sig = getattr(self, '_TransmissionRPC__on_' + signal)
+            sig = getattr(self, '_on_' + signal)
         except AttributeError:
             raise ValueError('Unknown signal: {!r}'.format(signal))
         else:
             if not isinstance(sig, Signal):
                 raise ValueError('Unknown signal: {!r}'.format(signal))
             else:
                 log.debug('Registering %r for %r event', callback, signal)
                 sig.connect(callback, weak=autoremove)
 
     @property
     def version(self):
         """Version of the Transmission daemon or None if not connected"""
-        return self.__version
+        return self._version
 
     @property
     def rpcversion(self):
         """RPC version of the Transmission daemon or None if not connected"""
-        return self.__rpcversion
+        return self._rpcversion
 
     @property
     def rpcversionmin(self):
         """Oldest RPC version supported by Transmission daemon or None if not connected"""
-        return self.__rpcversionmin
+        return self._rpcversionmin
 
     @property
-    def url(self):
-        """Transmission's RPC URL without the path"""
-        return self.__url
+    def host(self):
+        """
+        Hostname or IP of the Transmission RPC interface
+
+        Setting this property calls disconnect().
+        """
+        return self._host
+    @host.setter
+    def host(self, host):
+        self._host = str(host)
+        asyncio.ensure_future(self.disconnect('Changing host: %r' % self._host))
+
+    @property
+    def path(self):
+        """
+        Path of the Transmission RPC interface
+
+        Setting this property calls disconnect().
+        """
+        return self._path
+    @path.setter
+    def path(self, path):
+        if not path or path[0] != '/':
+            path = '/' + path
+        self._path = path
+        asyncio.ensure_future(self.disconnect('Changing path: %r' % self._path))
+
+    @property
+    def port(self):
+        """
+        Port of the Transmission RPC interface
+
+        Setting this property calls disconnect().
+        """
+        return self._port
+    @port.setter
+    def port(self, port):
+        self._port = int(port)
+        asyncio.ensure_future(self.disconnect('Changing port: %r' % self._port))
+
+    @property
+    def user(self):
+        """
+        Username for authenticating to the Transmission RPC interface or empty string
+
+        Setting this property calls disconnect().
+        """
+        return self._user
+    @user.setter
+    def user(self, user):
+        self._user = str(user)
+        asyncio.ensure_future(self.disconnect('Changing user: %r' % self._user))
+
+    @property
+    def password(self):
+        """
+        Password for authenticating to the Transmission RPC interface or empty string
+
+        Setting this property calls disconnect().
+        """
+        return self._password
+    @password.setter
+    def password(self, password):
+        self._password = str(password)
+        asyncio.ensure_future(self.disconnect('Changing password: %r' % self._password))
+
+    @property
+    def tls(self):
+        """
+        Whether to use HTTPS for connecting to the Transmission RPC interface
 
-    @url.setter
-    def url(self, url):
-        self.__url = TransmissionURL(url)
+        Setting this property calls disconnect().
+        """
+        return self._tls
+    @tls.setter
+    def tls(self, tls):
+        self._tls = bool(tls)
+        asyncio.ensure_future(self.disconnect('Changing tls: %r' % self._tls))
+
+    @property
+    def url(self):
+        """Schema, host, port, and path combined as a string"""
+        return '%s://%s:%d%s' % (
+            'https' if self.tls else 'http', self.host, self.port, self.path)
 
     @property
     def timeout(self):
         """Number of seconds to try to connect before giving up"""
-        return self.__timeout
-
+        return self._timeout
     @timeout.setter
     def timeout(self, timeout):
-        self.__timeout = timeout
+        self._timeout = float(timeout)
+
+    @property
+    def enabled(self):
+        """
+        Whether requests should connect
+
+        If this is set to False, requests will wait for it to be set to True.
+        This allows you to block any connection attempts until the connection
+        parameters (host, user, password, etc) are specified to prevent any
+        unwarranted error messages.
+        """
+        return self._enabled_event.is_set()
+    @enabled.setter
+    def enabled(self, enabled):
+        if enabled and not self.enabled:
+            log.debug('Enabling %r', self)
+            self._enabled_event.set()
+        elif not enabled and self.enabled:
+            log.debug('Disabling %r', self)
+            self._enabled_event.clear()
+            if self.connected:
+                asyncio.ensure_future(self.disconnect())
 
     @property
     def connected(self):
         """Return True if connected, False otherwise"""
-        return self.__session is not None and not self.__session.closed \
-            and self.__connection_tested
+        return (self._session is not None
+                and not self._session.closed
+                and self._connection_tested)
 
-    async def connect(self, url=None, timeout=None):
-        """Connect to running daemon
+    async def connect(self):
+        """
+        Connect to running daemon
 
-        url: URL to the Transmission RPC interface or None for default
-             (see TransmissionURL)
-        timeout: Maximum number of seconds before attempt to connect fails
+        If the `enabled` property is set to False, this method blocks until
+        `enabled` is set to True.
 
         Raises RPCError, ConnectionError or AuthError.
         """
-        if self.__connection_lock.locked():
-            # Someone else is currently connecting.  Wait for them to finish.
-            log.debug('Waiting for other connection to establish')
-            await self.__connection_lock.acquire()
-            log.debug('Other connect() call finished')
-            self.__connection_lock.release()
-
-            # Check if connection has the url we want
-            if url is not None and self.url != TransmissionURL(url):
-                log.debug('Reconnecting because %s != %s', self.__url, url)
-                await self.connect(url=url, timeout=timeout)
-
-            # The other connect() call croaked for some reason, and our caller
-            # expects the same exception.  Calling connect() again should
-            # raise the same error, but that's too much recursion for my tiny,
-            # little mind.
-            elif self.__connect_exception is not None:
-                log.debug('Raising exception of other connect() call: %r', self.__connect_exception)
-                raise self.__connect_exception
-
-            # Looks like we're connected.  Our intended timeout may differ
-            # from what the previous call set, but there's no need to
-            # re-connect.
-            elif timeout is not None and self.timeout != timeout:
-                self.timeout = timeout
+        log.debug('Connecting to %s (timeout=%ss)', self.url, self.timeout)
+        self._on_connecting.send(self)
 
-        else:
-            async with self.__connection_lock:
-                log.debug('Acquired connect() lock')
-                if timeout is not None:
-                    self.timeout = timeout
-
-                # Reconnect if URL is specified
-                if url is not None:
-                    if self.connected:
-                        await self.disconnect('reconnecting to %s' % url)
-                    self.__url = TransmissionURL(url)
-                self.__on_connecting.send(self.url)
+        if self._connecting_lock.locked():
+            if self._connection_exception is not None:
+                # The other connect() call failed
+                log.debug('Found connection error: %r', self._connection_exception)
+                raise self._connection_exception
 
-                # If we're not connected (because new URL or we weren't
-                # connected in the first place), create new session.
-                if not self.connected:
-                    log.debug('Connecting to %s (timeout=%ss)', self.url, self.timeout)
-                    session_args = {'loop': self.loop}
-                    # TODO: Remove this check when aiohttp2 is common.
-                    if aiohttp.__version__[0] == '2':
-                        session_args['connector'] = aiohttp.TCPConnector(limit_per_host=1)
-                    if self.__url.has_auth:
-                        session_args['auth'] = aiohttp.BasicAuth(self.__url.user,
-                                                                 self.__url.password)
-
-                    # It is possible that the connection test below was
-                    # interrupted, which leaves us with self.connected returning
-                    # False (self.__connection_tested is still False), but an
-                    # unclosed ClientSession in self.__session.  We must close
-                    # it before consigning it to the garbage collector so it
-                    # doesn't throw warnings around.
-                    if self.__session is not None and not self.__session.closed:
-                        log.debug('Closing leftover ClientSession before creating a new one: %r', self.__session)
-                        self.__session.close()
-                    self.__session = aiohttp.ClientSession(**session_args)
-                    skip_connected_callback = False
-                else:
-                    log.debug('Already connected to %s', self.url)
-                    skip_connected_callback = True
+            log.debug('Connection is already being established - Waiting ...')
+            try:
+                async with async_timeout.timeout(self.timeout):
+                    await self._enabled_event.wait()
+            except asyncio.TimeoutError:
+                raise TimeoutError(self.timeout, self.url)
+            else:
+                if self.connected:
+                    log.debug('Connection is up: %r', self.url)
+                    return
+
+        async with self._connecting_lock:
+            log.debug('Acquired connect() lock')
+
+            if self.connected:
+                await self.disconnect('Reconnecting')
+
+            # Block until we're enabled
+            await self._enabled_event.wait()
+
+            import aiohttp
+            session_args = {'loop': self.loop}
+            if self.user and self.password:
+                session_args['auth'] = aiohttp.BasicAuth(self.user, self.password,
+                                                         encoding='utf-8')
+            self._session = aiohttp.ClientSession(**session_args)
 
-                # Check if connection works.  If we were already connected, we
-                # still want to check if the old connection still works, but
-                # we don't want to report the working connection again to
-                # callbacks (skip_connected_callback).
-                log.debug('Initializing new connection to %s', self.url)
-                try:
-                    test_request = json.dumps({'method':'session-get'})
-                    info = await self.__send_request(test_request)
-                except ClientError as e:
-                    log.debug('Caught during initialization: %r', e)
-                    self.__connect_exception = e
-                    await self.__reset()
-                    self.__on_error.send(self.__url, error=e)
-                    raise
-                else:
-                    self.__version = info['version']
-                    self.__rpcversion = info['rpc-version']
-                    self.__rpcversionmin = info['rpc-version-minimum']
-                    self.__connection_tested = True
-                    self.__connect_exception = None
-                    log.debug('Connection established: %s', self.url)
-                    if not skip_connected_callback:
-                        self.__on_connected.send(self.__url)
+            # Check if connection works
+            log.debug('Testing connection to %s', self.url)
+            try:
+                test_request = json.dumps({'method':'session-get'})
+                info = await self._send_request(test_request)
+            except ClientError as e:
+                self._connection_exception = e
+                log.debug('Caught during connection test: %r', e)
+                await self._reset()
+                self._on_error.send(self, error=e)
+                raise
+            else:
+                self._version = info['version']
+                self._rpcversion = info['rpc-version']
+                self._rpcversionmin = info['rpc-version-minimum']
+                self._connection_tested = True
+                self._connection_exception = None
+                log.debug('Connection established: %s', self.url)
+                self._on_connected.send(self)
 
-                log.debug('Releasing connect() lock')
+            log.debug('Releasing connect() lock')
 
     async def disconnect(self, reason=None):
-        """Disconnect if connected
+        """
+        Disconnect if connected
 
         reason: Why are we disconnecting? Only used in a debugging message.
         """
         if self.connected:
-            await self.__reset()
-            log.debug('Disconnecting from %s (%s)',
-                      self.url, reason if reason is not None else 'for no reason')
-            log.debug('Calling "disconnected" callbacks for %s', self.url)
-            self.__on_disconnected.send(self.__url)
-
-    async def __reset(self):
-        if self.__session is not None:
-            await self.__session.close()
-        self.__session = None
-        self.__version = None
-        self.__rpcversion = None
-        self.__rpcversionmin = None
-        self.__connection_tested = False
+            await self._reset()
+            log.debug('Disconnecting from %s (%s)', self.url,
+                      reason if reason is not None else 'for no reason')
+            self._on_disconnected.send(self)
+
+    async def _reset(self):
+        if self._session is not None:
+            await self._session.close()
+        self._session = None
+        self._version = None
+        self._rpcversion = None
+        self._rpcversionmin = None
+        self._connection_tested = False
+
+    async def _post(self, data):
+        async with async_timeout.timeout(self.timeout):
+            response = await self._session.post(self.url, data=data, headers=self._headers)
+
+            if response.status == CSRF_ERROR_CODE:
+                # Send request again with CSRF header
+                self._headers[CSRF_HEADER] = response.headers[CSRF_HEADER]
+                log.debug('Setting CSRF header: %s = %s',
+                          CSRF_HEADER, response.headers[CSRF_HEADER])
+                await response.release()
+                return await self._post(data)
+
+            elif response.status == AUTH_ERROR_CODE:
+                await response.release()
+                log.debug('Authentication failed: %s: user=%r, password=%r',
+                          self.url, self.user, self.password)
+                raise AuthError(self.url)
 
-    async def __post(self, data):
-        with async_timeout.timeout(self.timeout):
-            try:
-                response = await self.__session.post(str(self.__url), data=data, headers=self.__headers)
-            except asyncio.CancelledError as e:
-                log.debug('Caught TimeoutError: %r', e)
-                raise ConnectionError('Timeout after {}s: {}'.format(self.timeout, self.url))
-            except aiohttp.ClientError as e:
-                log.debug('Caught during POST request: %r', e)
-                raise ConnectionError(str(self.url))
             else:
-                if response.status == CSRF_ERROR_CODE:
-                    # Send request again with CSRF header
-                    self.__headers[CSRF_HEADER] = response.headers[CSRF_HEADER]
-                    log.debug('Setting CSRF header: %s = %s',
-                              CSRF_HEADER, response.headers[CSRF_HEADER])
-                    await response.release()
-                    return await self.__post(data)
-
-                elif response.status == AUTH_ERROR_CODE:
-                    await response.release()
-                    log.debug('Authentication failed')
-                    raise AuthError(str(self.url))
-
+                import aiohttp
+                try:
+                    answer = await response.json()
+                except aiohttp.ClientResponseError:
+                    raise RPCError('Server sent malformed JSON: %s' % await response.text())
                 else:
-                    try:
-                        answer = await response.json()
-                    except aiohttp.ClientResponseError as e:
-                        text = textwrap.shorten(await response.text(),
-                                                50, placeholder='...')
-                        raise RPCError('Server sent malformed JSON: {}'.format(text))
-                    else:
-                        return answer
+                    return answer
 
-    async def __send_request(self, post_data):
-        """Send RPC POST request to daemon
+    async def _send_request(self, post_data):
+        """
+        Send RPC POST request to daemon
 
         post_data: Any valid RPC request as JSON string
 
         If applicable, returns response['arguments']['torrents'] or
         response['arguments'], otherwise response.
 
         Raises ClientError.
         """
+        import aiohttp
         try:
-            answer = await self.__post(post_data)
-        except OSError as e:
-            log.debug('Caught OSError: %r', e)
-            raise ConnectionError(str(self.url))
+            answer = await self._post(post_data)
+
+        # CancelledError is raised when we're writing on a "closing
+        # transport". Not sure if this happens in the real world, but it happens
+        # in the tests for some reason.
+        except (aiohttp.ClientError, asyncio.CancelledError) as e:
+            log.debug('Caught during POST request: %r', e)
+            raise ConnectionError(self.url)
+
+        except asyncio.TimeoutError as e:
+            raise TimeoutError(self.timeout, self.url)
+
         else:
             if answer['result'] != 'success':
                 raise RPCError(answer['result'].capitalize())
             else:
                 if 'arguments' in answer:
                     if 'torrents' in answer['arguments']:
                         return answer['arguments']['torrents']
                     else:
                         return answer['arguments']
                 return answer
 
     def __getattr__(self, method):
-        """Return asyncio coroutine that sends RPC request and returns response
+        """
+        Return asyncio coroutine that sends RPC request and returns response
 
         method: Any method from the RPC specs with every '-' replaced with '_'.
                 For arguments see the RPC specs.
 
         Example:
         >>> stats = await client.session_stats()
         >>> torrents = await client.torrent_get(ids=(1,2,3), fields=('status','name'))
 
         Raises RPCError, ConnectionError, AuthError
         """
-        async def request(arguments={}, autoconnect=True, **kwargs):
-            async with self.__request_lock:
+        async def request(arguments=None, **kwargs):
+            arguments = arguments or {}
+
+            async with self._request_lock:
                 if not self.connected:
-                    if autoconnect:
-                        log.debug('Autoconnecting for %r', method)
-                        await self.connect()
-                    else:
-                        log.debug('Not connected and autoconnect=%r - %r returns None',
-                                  autoconnect, method)
-                        return None
+                    log.debug('Autoconnecting for %r', method)
+                    await self.connect()
 
                 arguments.update(**kwargs)
                 rpc_request = json.dumps({'method'    : method.replace('_', '-'),
                                           'arguments' : arguments})
 
                 try:
-                    return await self.__send_request(rpc_request)
+                    return await self._send_request(rpc_request)
                 except ClientError as e:
                     log.debug('Caught ClientError in %r request: %r', method, e)
 
                     # RPCError does not mean host is unreachable, there was just a
                     # misunderstanding, so we're still connected.
                     if not isinstance(e, RPCError) and self.connected:
                         await self.disconnect(str(e))
 
-                    self.__on_error.send(self.__url, error=e)
+                    self._on_error.send(self, error=e)
                     raise
 
         request.__name__ = method
         request.__qualname__ = method
         return request
```

### Comparing `stig-0.8.3a0/stig/client/aiotransmission/api_status.py` & `stig-0.9.0a0/stig/client/aiotransmission/api_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from ...logging import make_logger
 log = make_logger(__name__)
 
 import blinker
 from collections import namedtuple
 
 from ..poll import RequestPoller
-from .. import convert
-from .. import constants as const
+from ..utils import (convert, const)
 
 
 TorrentCount = namedtuple('TorrentCount', ('active', 'downloading', 'isolated',
                                            'stopped', 'total', 'uploading'))
 
 
 class StatusAPI():
@@ -50,57 +49,55 @@
 
     @interval.setter
     def interval(self, interval):
         self._poller_stats.interval = interval
         self._poller_tcount.interval = interval
 
 
-    def __init__(self, srvapi, interval=1, autoconnect=True):
+    def __init__(self, srvapi, interval=1):
         self._session_stats_updated = False
         self._tcounts_updated = False
         self._reset_session_stats()
         self._reset_tcounts()
         self._on_update = blinker.Signal()
 
         self._poller_stats = RequestPoller(srvapi.rpc.session_stats,
-                                           autoconnect=autoconnect,
                                            interval=interval,
                                            loop=srvapi.loop)
         self._poller_stats.on_response(self._handle_session_stats)
         self._poller_stats.on_error(lambda e: log.debug('Ignoring exception: %r', e),
                                     autoremove=False)
 
         # 'session-stats' provides some counters, but not enough, so we
         # request a minimalistic torrent list.
         self._poller_tcount = RequestPoller(srvapi.torrent.torrents,
                                             keys=('rate-down', 'rate-up', 'status'),
-                                            autoconnect=autoconnect,
                                             interval=interval,
                                             loop=srvapi.loop)
-        self._poller_tcount.on_response(self._handle_tlist)
+        self._poller_tcount.on_response(self._handle_torrent_list)
 
     def _reset_session_stats(self):
         self._session_stats = None
 
     def _reset_tcounts(self):
-        self._tlist = None
+        self._torrent_list = None
 
     def _handle_session_stats(self, stats):
         if stats is None:
             self._reset_session_stats()
         else:
             self._session_stats = stats
         self._session_stats_updated = True
         self._maybe_run_callbacks()
 
-    def _handle_tlist(self, response):
+    def _handle_torrent_list(self, response):
         if response is None:
             self._reset_tcounts()
         else:
-            self._tlist = response.torrents
+            self._torrent_list = response.torrents
         self._tcounts_updated = True
         self._maybe_run_callbacks()
 
     def _maybe_run_callbacks(self):
         # We have two pollers, but we want to call callbacks once when both
         # have an update to report.
         if self._tcounts_updated and self._session_stats_updated:
@@ -118,15 +115,15 @@
         log.debug('Registering %r to receive status updates', callback)
         self._on_update.connect(callback, weak=autoremove)
 
     @property
     def count(self):
         """Torrent counts by category"""
         stats = self._session_stats
-        tlist = self._tlist
+        tlist = self._torrent_list
         tc_args = {field:const.DISCONNECTED for field in TorrentCount._fields}
         if stats is not None:
             tc_args.update(
                 total=stats['torrentCount'],
                 stopped=stats['pausedTorrentCount'],
                 active=stats['activeTorrentCount']
             )
@@ -141,15 +138,15 @@
         return TorrentCount(**tc_args)
 
     def _get_transfer_rate(self, direction):
         stats = self._session_stats
         if stats is None:
             return const.DISCONNECTED
         else:
-            return convert.bandwidth(self._session_stats[direction + 'loadSpeed'], unit='byte')
+            return convert.bandwidth(self._session_stats[direction + 'loadSpeed'], unit='B')
 
     @property
     def rate_down(self):
         """Total download rate or `constants.DISCONNECTED`"""
         return self._get_transfer_rate('down')
 
     @property
```

### Comparing `stig-0.8.3a0/stig/client/aiotransmission/__init__.py` & `stig-0.9.0a0/stig/client/aiotransmission/__init__.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/client/aiotransmission/api_torrent.py` & `stig-0.9.0a0/stig/client/aiotransmission/api_torrent.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 from ...logging import make_logger
 log = make_logger(__name__)
 
 from string import hexdigits as HEXDIGITS
 from collections import abc
 import os
 import base64
-import unicodedata
 
 from ..utils import (Response, URL)
 from .torrent import (TorrentFields, Torrent)
 from .. import ClientError
-from ..filters.tfilter import TorrentFilter
-from ..filters.ffilter import TorrentFileFilter
-from .. import convert
-from .. import constants as const
+from ..filters.torrent import TorrentFilter
+from ..filters.file import TorrentFileFilter
+from ..utils import (Bool, Bandwidth, BoolOrBandwidth)
 
 
 class _TorrentCache():
     def __init__(self, raw_torrents=()):
         self._tdict = {}  # Map torrent IDs to Torrent objects
 
     def update(self, raw_torrents):
@@ -89,72 +87,56 @@
         try:
             result = await method(*args, **kwargs)
         except ClientError as e:
             return Response(result=None, msgs=(e,), success=False)
         else:
             return Response(result=result, msgs=(), success=True)
 
-    @staticmethod
-    def _ensure_bytes(number, converter):
-        if number is const.UNLIMITED:
-            return number
-        elif not hasattr(number, 'unit'):
-            if isinstance(number, str):
-                number = converter.from_string(number)
-            else:
-                number = converter(number)
-        unit = number.unit
-        if unit == 'b':
-            number = number / 8
-            number.unit = 'B'
-            return number
-        elif unit == 'B':
-            return number
-        else:
-            raise RuntimeError('Cannot convert %r to bytes: %r', unit, number)
-
     async def _map_tid_to_torrent_values(self, torrents, keys):
-        """Map torrent ID to Torrent value(s)
+        """
+        Map torrent ID to Torrent value(s)
 
         If `keys` lists only one key, the returned map maps each torrent's ID to
         its value of that key.
 
         If `keys` lists two or more keys, the returned map maps torrent IDs to a
         dict with the keys `keys` and their corresponding values for each torrent.
 
+        The result is returned attached to a Response instance via the attribute
+        'torrent_values'.
+
         If request failed, return Response instance from `torrents` object.
         """
         response = await self.torrents(torrents, keys=('id',) + tuple(keys))
         if not response.success:
             return Response(success=False, torrent_values={}, msgs=response.msgs)
         else:
             if len(keys) == 1:
                 key = keys[0]
                 torrent_values = {t['id']:t[key] for t in response.torrents}
             else:
                 torrent_values = {t['id']:{key:t[key] for key in keys}
                                   for t in response.torrents}
             return Response(success=True, torrent_values=torrent_values)
 
-    async def _abs_download_path(self, path, autoconnect=True):
+    async def _abs_download_path(self, path):
         """Turn relative `path` into absolute path based on default download path"""
-        if not autoconnect and not self.rpc.connected:
-            return None
-        elif not os.path.isabs(path):
+        if not os.path.isabs(path):
             response = await self._request(self.rpc.session_get)
             if not response.success:
                 return Response(path=None, success=False, msgs=response.msgs)
             else:
                 download_dir = response.result['download-dir']
                 abs_path = os.path.normpath(os.path.join(download_dir, path))
                 return Response(path=abs_path, success=True)
         return Response(path=path, success=True)
 
     async def add(self, torrent, stopped=False, path=None):
-        """Add torrent from file, URL or hash
+        """
+        Add torrent from file, URL or hash
 
         torrent: Path to local file, web/magnet link or hash
         stopped: False to start downloading immediately, True otherise
         path:    Download directory or `None` for default directory
 
         Return Response with the following properties:
             torrent: Torrent object with the keys 'id' and 'name' if the
@@ -247,26 +229,23 @@
             # that we still have cached but don't exist anymore and purge them.
             if ids is None:
                 tids = tuple(t['id'] for t in raw_tlist)
                 self._tcache.purge(existing_tids=tids)
 
             return Response(success=True, raw_torrents=raw_tlist)
 
-    async def _get_torrents_by_ids(self, keys, ids=None, autoconnect=True):
-        """Return a Response object with 'torrents' set to a tuple of Torrents
+    async def _get_torrents_by_ids(self, keys, ids=None):
+        """
+        Return a Response object with 'torrents' set to a tuple of Torrents
 
         keys: 'ALL' for all supported Torrent keys or a sequence of key
               strings (see client.ttypes.TYPES for available keys)
         ids: None for all torrents or a sequence of wanted IDs
-        autoconnect: Wether to attempt to connect automatically if not
-                     connected; if False and not connected, return None
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-        elif keys == 'ALL':
+        if keys == 'ALL':
             fields = TorrentFields(keys)
         else:
             fields = TorrentFields(*keys)
 
         tlist = ()
         msgs = []
         success = False
@@ -294,24 +273,22 @@
                         msgs.append(ClientError('No torrent with ID: {}'.format(tid)))
 
             success = len(tlist) > 0 or not ids
 
             log.debug('Found %d torrents in %.3fms', len(tlist), (time()-start)*1e3)
         return Response(success=success, torrents=tlist, msgs=msgs)
 
-    async def _get_torrents_by_filter(self, keys, tfilter=None, autoconnect=True):
-        """Return a Response object with 'torrents' set to a tuple of Torrents
+    async def _get_torrents_by_filter(self, keys, tfilter=None):
+        """
+        Return a Response object with 'torrents' set to a tuple of Torrents
 
         keys: See _get_torrents_by_ids
         tfilter: A TorrentFilter instance or None
-        autoconnect: See _get_torrents_by_ids
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-        elif tfilter == None:
+        if tfilter is None:
             log.debug('Looking for all torrents with keys: %s', keys)
             # No filter specified - just return all torrents with the specified keys
             return await self._get_torrents_by_ids(keys=keys)
         else:
             log.debug('Looking for %s torrents with keys: %s', tfilter, keys)
             tlist = ()
             msgs = []
@@ -341,73 +318,66 @@
                 msgs.append(ClientError('No matching torrents: {}'.format(tfilter)))
             else:
                 msgs.append('Found {} {} torrent{}'.format(
                     len(tlist), tfilter, '' if len(tlist) == 1 else 's'))
 
             return Response(success=success, torrents=tlist, msgs=msgs)
 
-    async def torrents(self, torrents=None, keys='ALL', autoconnect=True):
-        """Fetch and return torrents
+    async def torrents(self, torrents=None, keys='ALL'):
+        """
+        Fetch and return torrents
 
         torrents: Iterator of torrent IDs, TorrentFilter object (or its string
                   representation) or None for all torrents
         keys: tuple of Torrent keys to fetch or 'ALL' for all torrents
-        autoconnect: Wether to attempt to connect automatically if not
-                     connected; if False and not connected, return None
 
         Return Response with the following properties:
             torrents: tuple of Torrent objects with requested torrents
             success: False if no torrents were found, True otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-        elif torrents is None:
+        if torrents is None:
             return await self._get_torrents_by_ids(keys)
         elif isinstance(torrents, (str, TorrentFilter)):
             return await self._get_torrents_by_filter(keys, tfilter=torrents)
         elif isinstance(torrents, abc.Sequence) and \
              all(isinstance(id, int) for id in torrents):
             return await self._get_torrents_by_ids(keys, ids=torrents)
         else:
             raise ValueError("Invalid 'torrents' argument: {!r}".format(torrents))
 
-    async def _torrent_action(self, method, torrents=None, method_args={}, check=None,
-                              keys_check=(), autoconnect=True):
-        """Helper method that operates on torrents (start, stop, remove, etc)
+    async def _torrent_action(self, method, torrents=None, method_args={},
+                              check=None, check_keys=()):
+        """
+        Helper method that operates on torrents (start, stop, remove, etc)
 
         method: Any method from TransmissionRPC that accepts torrent ids
         torrents: See `torrents` method
         method_args: Dictionary with keyword arguments for method (except 'ids')
         check: None or callable that is called with every torrent; must return
                a 2-tuple of (SUCCESS, MESSAGE) where SUCCESS is evaluated as
                bool and MESSAGE a string or None.  If SUCCESS evaluates to
                True, `method` is applied to the torrent, otherwise not.
-        keys_check: List of Torrent keys the check function needs ('id' and
+        check_keys: List of Torrent keys the check function needs ('id' and
                     'name' are always included)
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of Torrents that `method` was applied to with the
                       keys 'id' and 'name'
             success: True if `method` was successfully applied to at least one
                      torrent, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-
         tlist = []
         msgs = []
-        success = False
 
         # Always provide some basic keys
-        keys_check = set(tuple(keys_check) + ('id', 'name'))
+        check_keys = set(tuple(check_keys) + ('id', 'name'))
 
-        response = await self.torrents(torrents, keys=keys_check)
+        response = await self.torrents(torrents, keys=check_keys)
         if not response.success:
             return Response(success=False, torrents=(), msgs=response.msgs)
         else:
             msgs = list(response.msgs)
 
         if check is None:
             tlist = response.torrents
@@ -433,41 +403,40 @@
                 await method(ids=tuple(t['id'] for t in tlist), **method_args)
             except ClientError as e:
                 msgs.append(e)
                 return Response(success=False, torrents=(), msgs=msgs)
             else:
                 return Response(success=True, torrents=tuple(tlist), msgs=msgs)
 
-    async def stop(self, torrents, autoconnect=True):
-        """Stop down-/uploading torrents
+    async def stop(self, torrents):
+        """
+        Stop down-/uploading torrents
 
         torrents: See `torrents` method
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of stopped Torrents with the keys 'id' and 'name'
             success: True if any torrents were found and stopped, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
         def check(t):
             if t['status'].STOPPED in t['status']:
                 return (False, 'Already stopped: ' + t['name'])
             else:
                 return (True, 'Stopping ' + t['name'])
 
         return await self._torrent_action(self.rpc.torrent_stop, torrents,
-                                          check=check, keys_check=('status',),
-                                          autoconnect=autoconnect)
+                                          check=check, check_keys=('status',))
 
-    async def start(self, torrents, force=False, autoconnect=True):
-        """Start down-/uploading torrents
+    async def start(self, torrents, force=False):
+        """
+        Start down-/uploading torrents
 
         torrents: See `torrents` method
         force: Start downloading even if download queue is active and full
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of started Torrents with the keys 'id' and 'name'
             success: True if any torrents were found and started, False
                      otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
@@ -479,24 +448,23 @@
 
         if force:
             method = self.rpc.torrent_start_now
         else:
             method = self.rpc.torrent_start
 
         return await self._torrent_action(method, torrents,
-                                          check=check, keys_check=('status',),
-                                          method_args={'force':force},
-                                          autoconnect=autoconnect)
+                                          check=check, check_keys=('status',),
+                                          method_args={'force':force})
 
-    async def toggle_stopped(self, torrents, force=False, autoconnect=True):
-        """Start down-/uploading torrents
+    async def toggle_stopped(self, torrents, force=False):
+        """
+        Start down-/uploading torrents
 
         torrents: See `torrents` method
         force: See `start` method
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of toggled Torrents with the keys 'id' and 'name'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
         response = await self.torrents(torrents, keys=('status',))
@@ -520,19 +488,19 @@
             torrents += r.torrents
             msgs += r.msgs
 
         return Response(torrents=torrents,
                         success=len(torrents) > 0,
                         msgs=msgs)
 
-    async def verify(self, torrents, autoconnect=True):
-        """Verify torrents's downloaded data
+    async def verify(self, torrents):
+        """
+        Verify torrents's downloaded data
 
         torrents: See `torrents` method
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of to be verified Torrents with the keys 'id' and 'name'
             success: True if any torrents were found and will be verified,
                      False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
@@ -542,23 +510,22 @@
                     return (False, 'Already queued for verification: ' + t['name'])
                 else:
                     return (False, 'Already verifying: ' + t['name'])
             else:
                 return (True, 'Verifying ' + t['name'])
 
         return await self._torrent_action(self.rpc.torrent_verify, torrents,
-                                          check=check, keys_check=('status',),
-                                          autoconnect=autoconnect)
+                                          check=check, check_keys=('status',))
 
-    async def remove(self, torrents, delete=False, autoconnect=True):
-        """Remove torrents
+    async def remove(self, torrents, delete=False):
+        """
+        Remove torrents
 
         torrents: See `torrents` method
         delete: True if downloaded files should be deleted
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of removed Torrents  with the keys 'id' and 'name'
             success: True if any torrents were found and removed, False
                      otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
@@ -568,72 +535,65 @@
             msg = 'Removing %s (keeping files)'
 
         def create_info_msg(t):
             return (True, msg % t['name'])
 
         return await self._torrent_action(self.rpc.torrent_remove, torrents,
                                           check=create_info_msg,
-                                          method_args={'delete-local-data': delete},
-                                          autoconnect=autoconnect)
+                                          method_args={'delete-local-data': delete})
 
 
-    async def move(self, torrents, destination, autoconnect=True):
-        """Change torrents' location in the file system
+    async def move(self, torrents, destination):
+        """
+        Change torrents' location in the file system
 
         torrents: See `torrents` method
         destination: New path of the specified torrents; relative paths are
                      relative to the default download path
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of moved Torrents with the keys 'id' and 'name'
             success: True if any torrents were found and had matching files,
                      False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-
         # Transmission wants an absolute path
         response = await self._abs_download_path(destination)
         if not response.success:
             return Response(torrents=(), success=False, msgs=response.msgs)
         else:
             destination = response.path
 
         def create_info_msg(t):
             if t['path'] != destination:
                 return (True, 'Moving to %s: %s' % (destination, t['name']))
             else:
                 return (False, 'Already in %s: %s' % (destination, t['name']))
 
         return await self._torrent_action(self.rpc.torrent_set_location, torrents,
-                                          check=create_info_msg, keys_check=('path',),
+                                          check=create_info_msg, check_keys=('path',),
                                           method_args={'move': True, 'location': destination})
 
 
-    async def file_priority(self, torrents, files, priority, autoconnect=True):
-        """Change download priority of individual torrent files
+    async def file_priority(self, torrents, files, priority):
+        """
+        Change download priority of individual torrent files
 
         torrents: See `torrents` method
         files: TorrentFileFilter object (or its string representation), sequence
                of (torrent ID, file ID) tuples or None for all files
         priority: 'off', 'low', 'normal' or 'high'
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of matching Torrents with matching files with the
                       keys 'id', 'name' and 'files'
             success: True if any torrents were found and had matching files,
                      False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
-
         response = await self.torrents(torrents, keys=('name', 'files'))
         if not response.success:
             return Response(torrents=(), success=False, msgs=response.msgs)
         else:
             torrents = ()
             torrent_ids = []
             msgs = []
@@ -644,18 +604,17 @@
 
             # Set filter_files to a lambda that takes a TorrentFileTree and
             # returns a list of TorrentFiles.
             if files is None:
                 filter_files = lambda ftree: tuple(ftree.files)
             elif isinstance(files, TorrentFileFilter):
                 filter_files = lambda ftree: tuple(files.apply(ftree.files))
-            elif isinstance(files, abc.Sequence) and \
-                 all(isinstance(tid, int) and isinstance(fid, int) for tid,fid in files):
+            elif isinstance(files, abc.Sequence):
                 filter_files = lambda ftree: tuple(f for f in ftree.files
-                                                   if (f['tid'],f['id']) in files)
+                                                   if f['id'] in files)
             else:
                 raise ValueError("Invalid 'files' argument: {!r}".format(files))
 
             for t in sorted(response.torrents, key=lambda t: t['name'].lower()):
                 # Filter torrent's files
                 flist = filter_files(t['files'])
                 if files is None:
@@ -665,126 +624,109 @@
                     if not flist:
                         msgs.append(ClientError('No matching files: {}'.format(t['name'])))
                     else:
                         msgs.append('{} matching file{}: {}'
                                     .format(len(flist), '' if len(flist) == 1 else 's', t['name']))
                 success = len(flist) > 0 or success
 
-                # Transmission wants a list of file indexes; luckily, the
-                # file's ID is its index (see .torrent.TorrentFileTree).
-                findexes = tuple(f['id'] for f in flist)
+                # Transmission wants a list of file indexes.  For
+                # aiotransmission, the 'id' field of a TorrentFile is a tuple:
+                #     (<torrent ID>, <file index>)
+                # (See aiotransmission.torrent._create_TorrentFileTree())
+                findexes = tuple(f['id'][1] for f in flist)
                 if findexes:
                     response = await self._set_files_priority(priority, t['id'], findexes)
                     if response.success:
                         torrent_ids.append(t['id'])
                     msgs.extend(response.msgs)
 
         if torrent_ids:
             response = await self.torrents(torrent_ids, keys=('id', 'name', 'files'))
             if response.success:
                 torrents = response.torrents
         return Response(torrents=torrents, success=success, msgs=msgs)
 
-    async def _set_files_priority(self, priority, torrent_id, file_indexes, autoconnect=True):
+    async def _set_files_priority(self, priority, torrent_id, file_indexes):
         fi = tuple(file_indexes)
+        log.debug('Setting priority of torrent #%d: %r: %s', torrent_id, priority, file_indexes)
         if priority in ('high', 'normal', 'low'):
             return await self._torrent_action(
                 self.rpc.torrent_set, (torrent_id,),
-                method_args={'priority-%s' % priority: fi, 'files-wanted': fi},
-                autoconnect=autoconnect)
+                method_args={'priority-%s' % priority: fi, 'files-wanted': fi})
         elif priority == 'off':
             return await self._torrent_action(
                 self.rpc.torrent_set, (torrent_id,),
-                method_args={'files-unwanted': fi},
-                autoconnect=autoconnect)
+                method_args={'files-unwanted': fi})
         else:
             raise ValueError('Invalid priority: {!r}'.format(priority))
 
 
-    async def _limit_rate_absolute(self, torrents, direction, limit, autoconnect=True):
-        if not autoconnect and not self.rpc.connected:
-            return None
-
-        # Disable limits for negative values
+    async def _limit_rate_absolute(self, torrents, direction, limit):
+        if isinstance(limit, str):
+            try:
+                limit = BoolOrBandwidth(limit)
+            except ValueError as e:
+                return Response(torrents=(), success=False,
+                                msgs=[ClientError('%s: %r' % (e, limit))])
         if isinstance(limit, (float, int)):
-            limit = False if limit < 0 or limit >= float('inf') else limit
+            limit = BoolOrBandwidth(False) if limit < 0 or limit >= float('inf') else limit
 
-        log.debug('Setting new %sload limit for torrents %s: %r', direction, torrents, limit)
+        log.debug('Setting new %sload limit for torrents %s: %s', direction, torrents, limit)
         return await self._limit_rate(torrents, direction, get_new_limit=lambda _: limit)
 
-    async def _limit_rate_relative(self, torrents, direction, adjustment, autoconnect=True):
-        if not autoconnect and not self.rpc.connected:
-            return None
-
-        # Only numbers are allowed
-        if not isinstance(adjustment, (float, int)):
-            raise ValueError('Invalid rate limit adjustment: %r', adjustment)
+    async def _limit_rate_relative(self, torrents, direction, adjustment):
+        if isinstance(adjustment, str):
+            try:
+                adjustment = Bandwidth(adjustment)
+            except ValueError as e:
+                return Response(torrents=(), success=False,
+                                msgs=[ClientError('%s: %r' % (e, adjustment))])
 
         def add_to_current_limit(current_limit):
             log.debug('Adjusting %sload limit %r by %r', direction, current_limit, adjustment)
-            if isinstance(current_limit, (float, int)):
-                new_limit = current_limit + adjustment
-                new_limit = max(0, new_limit)
-            else:
-                new_limit = current_limit
-            return new_limit
+            return BoolOrBandwidth.adjust(current_limit, adjustment)
 
         return await self._limit_rate(torrents, direction, get_new_limit=add_to_current_limit)
 
     async def _limit_rate(self, torrents, direction, get_new_limit):
-        response = await self._map_tid_to_torrent_values(torrents, keys=('rate-limit-'+direction,))
+        response = await self._map_tid_to_torrent_values(torrents, keys=('limit-rate-'+direction,))
         if not response.success:
             return Response(success=False, torrent_set_args={}, errors=[], msgs=response.msgs)
         else:
             current_limits = response.torrent_values
             log.debug('Current %sload rate limits: %r', direction, current_limits)
 
-        def normalize_rate_limit(limit):
-            if limit >= float('inf') or \
-               any(limit is x for x in (None, False, const.DISABLED, const.UNLIMITED)):
-                return None
-            elif any(limit is x for x in (True, const.ENABLED)):
-                return True
-            else:
-                return self._ensure_bytes(convert.bandwidth(limit), convert.bandwidth)
-
         # Generate 'torrent-set' arguments for each torrent ID.  To de-duplicate
         # requests (same args for multiple torrents), we map the args to a list
         # of torrent IDs, so we just append another ID for existing args.
         torrent_set_args = {}
         errors = {}
         for tid,cur_limit in current_limits.items():
-            new_limit = get_new_limit(cur_limit)
-
-            # Ensure that both values are in bytes
-            new_limit_norm = normalize_rate_limit(new_limit)
-            cur_limit_norm = normalize_rate_limit(cur_limit)
+            cur_limit = BoolOrBandwidth(cur_limit)
+            new_limit = BoolOrBandwidth(get_new_limit(cur_limit))
 
-            if new_limit_norm == cur_limit_norm:
+            if new_limit == cur_limit:
                 log.debug('Nothing to set: new:%r == cur:%r', new_limit, cur_limit)
-                errors[tid] = ('Already %s' % cur_limit)
+                errors[tid] = 'Already %s' % cur_limit
                 continue
-            elif new_limit_norm is None:
-                log.debug('Disabling limit')
-                args = (('%sloadLimited' % direction, False),)
-            elif new_limit_norm is True:
-                if cur_limit_norm not in (False, None):
-                    errors[tid] = ('Already enabled (%s)' % cur_limit)
+            elif isinstance(new_limit, Bool):
+                if new_limit and isinstance(cur_limit, (float, int)) and cur_limit < float('inf'):
+                    errors[tid] = 'Already limited'
                     continue
                 else:
-                    log.debug('Enabling limit')
-                    args = (('%sloadLimited' % direction, True),)
+                    log.debug('%sabling limit', 'En' if new_limit else 'Dis')
+                    args = (('%sloadLimited' % direction, bool(new_limit)),)
             else:
-                log.debug('Setting new limit: %r -> %r', new_limit, new_limit_norm)
-                if new_limit_norm >= float('inf'):
+                log.debug('Setting new limit: %r', new_limit)
+                if new_limit >= float('inf'):
                     args = (('%sloadLimited' % direction, False),)
                 else:
-                    rpc_value = int(round(new_limit_norm/1000))
+                    raw_limit = round(int(new_limit.copy(convert_to='B'))/1000)  # Transmission expects kilobytes
                     args = (('%sloadLimited' % direction, True),
-                            ('%sloadLimit' % direction, rpc_value))  # Transmission expects kilobytes
+                            ('%sloadLimit' % direction, raw_limit))
 
             if args in torrent_set_args:
                 torrent_set_args[args].append(tid)
             else:
                 torrent_set_args[args] = [tid]
 
         # Send one 'torrent-set' request for each list of torrent IDs
@@ -792,105 +734,96 @@
             response = await self._torrent_action(self.rpc.torrent_set, tids,
                                                   method_args=dict(args))
             if not response.success:
                 return Response(success=False, torrents=(), msgs=response.msgs)
 
         # Fetch torrents again and return Response with new rate limit messages
         all_tids = sum(torrent_set_args.values(), []) + list(errors)
-        response = await self.torrents(all_tids, keys=('name', 'id', 'rate-limit-'+direction))
+        response = await self.torrents(all_tids, keys=('name', 'id', 'limit-rate-'+direction))
         if not response.success:
             return Response(success=False, torrents=(), msgs=response.msgs)
         msgs = []
         success = False
         for t in response.torrents:
             if t['id'] in errors:
                 msgs.append(ClientError('%s %sload rate: %s' %
                                         (t['name'], direction, errors[t['id']])))
             else:
                 success = True
-                limit = t['rate-limit-'+direction]
-                limit_str = str(limit) if const.is_constant(limit) else limit.with_unit
-                msgs.append('%s %sload rate: %s' % (t['name'], direction, limit_str))
+                msgs.append('%s %sload rate: %s' % (t['name'], direction, t['limit-rate-'+direction]))
         return Response(torrents=response.torrents, success=success, msgs=msgs)
 
-    async def set_rate_limit_up(self, torrents, limit, autoconnect=True):
-        """Limit upload rate for individual torrent(s)
+    async def set_limit_rate_up(self, torrents, limit):
+        """
+        Limit upload rate for individual torrent(s)
 
         torrents: See `torrents` method
-        limit: Allowed values:
-                 - Any positive number (bytes per second) sets the new limit to
-                   that
-                 - A negative number, `None`, `False` and the constants DISABLED
-                   and UNLIMITED disable the current limit
-                 - `True` and the constant ENABLED enable a previously disabled
-                   limit
-        autoconnect: See `torrents` method
+        limit: Passed to `utils.BoolOrBandwidth`
 
         Return Response with the following properties:
-            torrents: tuple of Torrents with the keys 'id', 'name' and 'rate-limit-up'
+            torrents: tuple of Torrents with the keys 'id', 'name' and 'limit-rate-up'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
-
         """
-        return await self._limit_rate_absolute(torrents, 'up', limit, autoconnect)
+        return await self._limit_rate_absolute(torrents, 'up', limit)
 
-    async def set_rate_limit_down(self, torrents, limit, autoconnect=True):
-        """Limit download rate for individual torrent(s)
+    async def set_limit_rate_down(self, torrents, limit):
+        """
+        Limit download rate for individual torrent(s)
 
         torrents: See `torrents` method
-        limit: See `set_rate_limit_up` method
-        autoconnect: See `torrents` method
+        limit: See `set_limit_rate_up` method
 
         Return Response with the following properties:
-            torrents: tuple of Torrents with the keys 'id', 'name' and 'rate-limit-down'
+            torrents: tuple of Torrents with the keys 'id', 'name' and 'limit-rate-down'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        return await self._limit_rate_absolute(torrents, 'down', limit, autoconnect)
+        return await self._limit_rate_absolute(torrents, 'down', limit)
 
-    async def adjust_rate_limit_up(self, torrents, adjustment, autoconnect=True):
-        """Same as `set_rate_limit_up` but set new limit relative to current limit
+    async def adjust_limit_rate_up(self, torrents, adjustment):
+        """
+        Same as `set_limit_rate_up` but set new limit relative to current limit
 
         adjustment: Negative or positive number to add to the current limit of
-                    each matching torrent
+                    each matching torrent; passed to `utils.Bandwidth`
         """
-        return await self._limit_rate_relative(torrents, 'up', adjustment, autoconnect)
+        return await self._limit_rate_relative(torrents, 'up', adjustment)
 
-    async def adjust_rate_limit_down(self, torrents, adjustment, autoconnect=True):
-        """Same as `set_rate_limit_down` but set new limit relative to current limit
+    async def adjust_limit_rate_down(self, torrents, adjustment):
+        """
+        Same as `set_limit_rate_down` but set new limit relative to current limit
 
-        adjustment: See `adjust_rate_limit_up` method
+        adjustment: See `adjust_limit_rate_up` method
         """
-        return await self._limit_rate_relative(torrents, 'down', adjustment, autoconnect)
+        return await self._limit_rate_relative(torrents, 'down', adjustment)
 
 
-    async def tracker_add(self, torrents, urls, autoconnect=True):
-        """Add tracker(s) to torrents
+    async def tracker_add(self, torrents, urls):
+        """
+        Add tracker(s) to torrents
 
         torrents: See `torrents` method
         urls: Iterable of announce URLs
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of Torrents with the keys 'id' and 'name'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
         if not urls:
             return Response(success=False, torrents=(), msgs=[ClientError('No URLs given')])
 
         # Transmission returns 'Invalid argument' if we try to add an existing
         # tracker, so first we check if any of our URLs already exist.
         response = await self.torrents(torrents, keys=('id', 'name', 'trackers',))
         if not response.success:
             return Response(success=False, torrents=(), msgs=response.msgs)
         else:
-            tordict = {tor['id']:tor for tor in  response.torrents}
+            tordict = {tor['id']:tor for tor in response.torrents}
 
         # Map torrent IDs to currently used URLs by that torrent
         old_url_dict = {torid:tuple(trk['url-announce'] for trk in torrent['trackers'])
                         for torid,torrent in tordict.items()}
 
         # Make sure URLs are comparable
         new_urls = [URL(url) for url in urls]
@@ -916,31 +849,28 @@
         response = await self._torrent_action(self.rpc.torrent_set, torrents,
                                               method_args=args)
         if not response.success:
             return Response(success=False, torrents=(), msgs=msgs + list(response.msgs))
         else:
             return Response(success=True, torrents=response.torrents, msgs=msgs)
 
-    async def tracker_remove(self, torrents, urls, partial_match=False, autoconnect=True):
-        """Remove tracker(s) from torrents
+    async def tracker_remove(self, torrents, urls, partial_match=False):
+        """
+        Remove tracker(s) from torrents
 
         torrents: See `torrents` method
         urls: Iterable of announce URLs
         partial_match: True if given URLs match existing URLs partially
                        (e.g. 'example.org' matches 'http://tracker.example.org/')
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of Torrents with the keys 'id' and 'name'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
-
         """
-        if not autoconnect and not self.rpc.connected:
-            return None
         if not urls:
             return Response(success=False, torrents=(), msgs=[ClientError('No URLs given')])
 
         # Get wanted torrent IDs
         response = await self.torrents(torrents, keys=('id',))
         if not response.success:
             return Response(success=False, torrents=(), msgs=response.msgs)
@@ -990,19 +920,19 @@
         # Get new torrent list with newly added trackers
         response = await self.torrents(tuple(remove_ids), keys=('id', 'name', 'trackers'))
         if not response.success:
             return Response(success=False, torrents=(), msgs=msgs + list(response.msgs))
         else:
             return Response(success=True, torrents=response.torrents, msgs=msgs)
 
-    async def announce(self, torrents, autoconnect=True):
-        """Announce torrents' to its tracker(s)
+    async def announce(self, torrents):
+        """
+        Announce torrents' to its tracker(s)
 
         torrents: See `torrents` method
-        autoconnect: See `torrents` method
 
         Return Response with the following properties:
             torrents: tuple of Torrents with the keys 'id' and 'name'
             success: True if any torrents were found, False otherwise
             msgs: list of strings/`ClientError`s caused by the request
         """
         import time
@@ -1015,10 +945,9 @@
                 return (False, ('Not allowing manual announce until %s (in %s): %r' %
                                 (t['time-manual-announce-allowed'],
                                  t['time-manual-announce-allowed'].delta, t['name'])))
             else:
                 return (True, 'Announcing: %s' % t['name'])
 
         return await self._torrent_action(self.rpc.torrent_reannounce, torrents,
-                                          check=check, keys_check=('status', 'trackers',
-                                                                   'time-manual-announce-allowed'),
-                                          autoconnect=autoconnect)
+                                          check=check, check_keys=('status', 'trackers',
+                                                                   'time-manual-announce-allowed'))
```

### Comparing `stig-0.8.3a0/stig/client/aiotransmission/torrent.py` & `stig-0.9.0a0/stig/client/aiotransmission/torrent.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """Torrent class and value modifiers for compatibility with ttypes"""
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
 from .. import ttypes
-from .. import utils
+from ..utils import LazyDict
 from .. import base
 
 
 # Some values need to be modified to comply with our internal standards
 
 def _modify_ratio(t):
     #define TR_RATIO_NA  -1
@@ -175,91 +175,95 @@
                                        Status.DOWNLOAD,
                                        Status.VERIFY)):
         statuses.append(Status.IDLE)
 
     return statuses
 
 
-def _create_TorrentFileTree(t):
-    fileStats = t['fileStats']
-    if len(fileStats) < 1:
-        # filelist is empty if torrent was added by hash and metadata isn't
-        # downloaded yet.
-        files = [{'name': t['name'], 'priority': 0, 'length': 0,
-                  'wanted': True, 'id': 0, 'bytesCompleted': 0}]
-    else:
-        # Combine 'files' and 'fileStats' fields and add the 'id' key to each
-        # file, which is the index in the list provided by Transmission.
-        files = ({'id': i, **f, **fS}
-                 for i,(f,fS) in enumerate(zip(t['files'], fileStats)))
-    return TorrentFileTree(t['id'], entries=files)
-
 import os
 class TorrentFileTree(base.TorrentFileTreeBase):
-    def __init__(self, torrent_id, entries, path=[]):
-        log.debug('Creating new TorrentFileTree for torrent %r', torrent_id)
+    @classmethod
+    def create(cls, raw_torrent):
+        fileStats = raw_torrent['fileStats']
+        if len(fileStats) < 1:
+            # filelist is empty if torrent was added by hash and metadata isn't
+            # downloaded yet.
+            filelist = [{'tid': -1, 'id': (-1, -1), 'name': raw_torrent['name'], 'priority': 0,
+                         'length': 0, 'wanted': True, 'bytesCompleted': 0}]
+        else:
+            # Combine 'files' and 'fileStats' fields and add the 'id' key to each
+            # file, which is a (torrent ID, file list index) tuple
+            tid = raw_torrent['id']
+            filelist = ({'id': (tid, i), **f, **fS}
+                        for i,(f,fS) in enumerate(zip(raw_torrent['files'], fileStats)))
+        return cls(raw_torrent['id'], raw_torrent['downloadDir'], filelist, path=())
+
+    def __init__(self, torrent_id, torrent_location, filelist, path):
+        log.debug('Creating new TorrentFileTree for torrent %r: %r', torrent_id, path)
+        super().__init__(path)
 
-        self._path = os.sep.join(path)
         items = {}
         subdirs = {}
 
-        for entry in entries:
+        for entry in filelist:
             parts = entry['name'].split(os.sep, 1)
             if len(parts) == 1:
                 filename = parts[0]
                 items[filename] = ttypes.TorrentFile(
                     tid=torrent_id, id=entry['id'],
-                    name=entry['name'], path=path,
+                    name=entry['name'], path=path, location=torrent_location,
                     size_total=entry['length'],
                     size_downloaded=entry['bytesCompleted'],
                     is_wanted=entry['wanted'],
                     priority=entry['priority'])
 
             elif len(parts) == 2:
                 subdir, subpath = parts
                 if subdir not in subdirs:
                     subdirs[subdir] = []
                 entry['name'] = subpath
                 subdirs[subdir].append(entry)
             else:
                 raise RuntimeError(parts)
 
-        for subdir,entries in subdirs.items():
-            items[subdir] = TorrentFileTree(torrent_id, entries, path=path+[subdir])
+        for subdir,filelist in subdirs.items():
+            items[subdir] = TorrentFileTree(torrent_id, torrent_location,
+                                            filelist, path=path+(subdir,))
         self._items = items
 
     def update(self, raw_torrent):
         def update_files(ftree, fileStats):
             if not fileStats:
-                # If fileStats is empty (e.g. no metadata yet), there is a dummy
-                # entry in ftree created by _create_TorrentFileTree().
+                # We don't have any metadata yet, so there is nothing to update
                 return
 
             for entry in ftree.values():
                 if isinstance(entry, ttypes.TorrentFile):
                     # File ID is its index in the list provided by
                     # Transmission (see _create_TorrentFileTree)
-                    fstats = fileStats[entry['id']]
+                    index = entry['id'][1]
+                    fstats = fileStats[index]
                     entry.update({'size-downloaded': fstats['bytesCompleted'],
                                   'is-wanted': fstats['wanted'],
-                                  'priority': fstats['priority']})
+                                  'priority': fstats['priority'],
+                                  'location': raw_torrent['downloadDir']})
                 else:
                     update_files(entry, fileStats)
 
         update_files(self._items, raw_torrent['fileStats'])
 
 
 
 class PeerList(tuple):
     def __new__(cls, t):
         TorrentPeer = ttypes.TorrentPeer
         return super().__new__(cls,
             (TorrentPeer(tid=t['id'], tname=t['name'], tsize=t['totalSize'],
                          ip=p['address'], port=p['port'], client=p['clientName'],
-                         progress=p['progress']*100,
+                         pdownloaded=p['progress']*100,
                          rate_up=p['rateToPeer'], rate_down=p['rateToClient'])
              for p in t['peers'])
         )
 
 
 
 class TrackerList(tuple):
@@ -287,15 +291,16 @@
     @staticmethod
     def _error_scrape(tracker):
         msg = tracker['lastScrapeResult'] if tracker['hasScraped'] else ''
         return '' if msg == 'Success' else msg
 
     @staticmethod
     def _next_time(tracker, which):
-        """Handle next(Announce|Scrape)Time RPC key
+        """
+        Handle next(Announce|Scrape)Time RPC key
 
         `which` must be 'Scrape' or 'Announce'.
 
         transmission.h says:
             /* when the next periodic (announce|scrape) message will be sent out.
                if (announce|scrape)State isn't TR_TRACKER_WAITING, this field is undefined */
         """
@@ -307,15 +312,16 @@
         elif state == 2:  # Announce/scrape is queued
             return ttypes.Timestamp.SOON
         else:
             return ttypes.Timestamp.NOW
 
     @staticmethod
     def _last_time(tracker, which):
-        """Handle last(Announce|Scrape)Time RPC key
+        """
+        Handle last(Announce|Scrape)Time RPC key
 
         `which` must be 'Scrape' or 'Announce'.
 
         transmission.h says:
             /* when the last (announce|scrape) was completed.
                if "has(Announced|Scraped)" is false, this field is undefined */
         """
@@ -323,25 +329,25 @@
             return tracker['last%sTime' % which]
         else:
             return ttypes.Timestamp.NEVER
 
     def __new__(cls, raw_torrent):
         return super().__new__(cls,
             (ttypes.TorrentTracker(
-                (utils.LazyDict({
+                (LazyDict({
+                    'id'                 : (raw_torrent['id'], raw_tracker['id']),
                     'tid'                : raw_torrent['id'],
                     'tname'              : raw_torrent['name'],
-                    'id'                 : (raw_torrent['id'], raw_tracker['id']),
                     'tier'               : raw_tracker['tier'],
 
                     'url-announce'       : raw_tracker['announce'],
                     'url-scrape'         : raw_tracker['scrape'],
 
-                    'state-announce'     : cls._STATES_ANNOUNCE[raw_tracker['announceState']],
-                    'state-scrape'       : cls._STATES_SCRAPE[raw_tracker['scrapeState']],
+                    'status-announce'    : cls._STATES_ANNOUNCE[raw_tracker['announceState']],
+                    'status-scrape'      : cls._STATES_SCRAPE[raw_tracker['scrapeState']],
 
                     'error-announce'     : lambda: cls._error_announce(raw_tracker),
                     'error-scrape'       : lambda: cls._error_scrape(raw_tracker),
 
                     'count-downloads'    : raw_tracker['downloadCount'],
                     'count-leeches'      : raw_tracker['leecherCount'],
                     'count-seeds'        : raw_tracker['seederCount'],
@@ -389,30 +395,30 @@
     'time-started'                 : ('startDate',),
     'time-activity'                : ('activityDate',),
     'time-completed'               : ('doneDate', 'percentDone', 'eta'),
     'time-manual-announce-allowed' : ('manualAnnounceTime',),
 
     'rate-down'                    : ('rateDownload',),
     'rate-up'                      : ('rateUpload',),
-    'rate-limit-down'              : ('downloadLimited', 'downloadLimit'),
-    'rate-limit-up'                : ('uploadLimited', 'uploadLimit'),
+    'limit-rate-down'              : ('downloadLimited', 'downloadLimit'),
+    'limit-rate-up'                : ('uploadLimited', 'uploadLimit'),
 
     'size-final'                   : ('sizeWhenDone',),
     'size-total'                   : ('totalSize',),
     'size-downloaded'              : ('downloadedEver',),
     'size-uploaded'                : ('uploadedEver',),
     'size-available'               : ('leftUntilDone', 'desiredAvailable', 'haveValid', 'haveUnchecked'),
     'size-left'                    : ('leftUntilDone',),
     'size-corrupt'                 : ('corruptEver',),
     'size-piece'                   : ('pieceSize',),
 
     'error'                        : ('errorString', 'error', 'trackerStats'),
     'trackers'                     : ('trackerStats', 'name', 'id'),
     'peers'                        : ('peers', 'totalSize', 'name'),
-    'files'                        : ('files', 'fileStats',),
+    'files'                        : ('files', 'fileStats', 'downloadDir'),
 }
 
 # Map our keys to callables that adjust the raw RPC values or create new
 # values from existing RPC values.
 _MODIFY = {
     '%downloaded'                  : lambda raw: raw['percentDone'] * 100,
     '%uploaded'                    : _percent_uploaded,
@@ -421,16 +427,16 @@
     '%available'                   : _percent_available,
     'status'                       : _make_status,
     'peers-seeding'                : _count_seeds,
     'ratio'                        : _modify_ratio,
     'size-available'               : _bytes_available,
 
     # Transmission provides rate limits in kilobytes - we want bytes
-    'rate-limit-down'              : lambda raw: None if not raw['downloadLimited'] else raw['downloadLimit'] * 1000,
-    'rate-limit-up'                : lambda raw: None if not raw['uploadLimited']   else raw['uploadLimit']   * 1000,
+    'limit-rate-down'              : lambda raw: None if not raw['downloadLimited'] else raw['downloadLimit'] * 1000,
+    'limit-rate-up'                : lambda raw: None if not raw['uploadLimited']   else raw['uploadLimit']   * 1000,
 
     'timespan-eta'                 : _modify_eta,
     'time-created'                 : lambda raw: _modify_timestamp(raw, 'dateCreated',
                                                                    zero_means=ttypes.Timestamp.UNKNOWN),
     'time-added'                   : lambda raw: _modify_timestamp(raw, 'addedDate',
                                                                    zero_means=ttypes.Timestamp.UNKNOWN),
     'time-started'                 : lambda raw: _modify_timestamp(raw, 'startDate',
@@ -439,46 +445,47 @@
                                                                    zero_means=ttypes.Timestamp.NEVER),
     'time-completed'               : lambda raw: _modify_timestamp_completed(raw),
     'time-manual-announce-allowed' : lambda raw: _modify_timestamp(raw, 'manualAnnounceTime'),
 
     'error'                        : _find_error,
     'trackers'                     : TrackerList,
     'peers'                        : PeerList,
-    'files'                        : _create_TorrentFileTree,
+    'files'                        : TorrentFileTree.create,
 }
 
 class Torrent(base.TorrentBase):
-    """Information about a torrent as a mapping
+    """
+    Information about a torrent as a mapping
 
     The available keys are specified in DEPENDENCIES and ttypes.TYPES.
     """
 
     def __init__(self, raw_torrent):
         self._raw = raw_torrent
         self._cache = {}
 
     def update(self, raw_torrent):
         cache = self._cache
         raw_old = self._raw
 
         # Remove cached values if their original/raw value(s) differ
-        for k,v in tuple(cache.items()):
+        for k in tuple(cache):
             # Each key depends on one or more RPC field
             fields = DEPENDENCIES[k]
             for field in fields:
                 new_value = raw_torrent.get(field)
                 old_value = raw_old.get(field)
                 if new_value is not None and new_value != old_value:
                     # log.debug('Invalidating cached %s: %r -> %r', k, old_value, new_value)
                     # New and previous value differ - if we are dealing with
                     # more complex data structures (e.g. a file tree), use the
                     # update() method to update the object in cache instead of
                     # removing it from the cache.
                     value = cache[k]
-                    if hasattr(value, 'update'):
+                    if hasattr(value, 'update') and all(field in raw_torrent for field in fields):
                         value.update(raw_torrent)
                     else:
                         del cache[k]
                     break
 
         # Now we can forget the old values
         raw_old.update(raw_torrent)
@@ -531,15 +538,16 @@
         return hash(self._raw['id'])
 
     def clearcache(self):
         self._cache = {}
 
 
 class TorrentFields(tuple):
-    """Convert Torrent keys to those specified in rpc-spec.txt
+    """
+    Convert Torrent keys to those specified in rpc-spec.txt
 
     The resulting tuple has no duplicates and the keys 'id' and 'name' are
     always included.
     """
     _RPC_FIELDS = ('activityDate', 'addedDate', 'announceResponse', 'announceURL',
                    'bandwidthPriority', 'comment', 'corruptEver', 'creator',
                    'dateCreated', 'desiredAvailable', 'doneDate', 'downloadDir',
```

### Comparing `stig-0.8.3a0/stig/client/base.py` & `stig-0.9.0a0/stig/client/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,23 +56,25 @@
         return len(tuple(iter(self)))
 
     def __hash__(self):
         return hash(self['id'])
 
 
 from collections import abc
+import os
 class TorrentFileTreeBase(abc.Mapping):
     """Nested mapping of a Torrent's files"""
 
     # Distinguish subtrees from files without comparing classes everywhere
     # ("parent" or "leaf")
     nodetype = 'parent'
 
-    def __init__(self, *args, **kwargs):
-        raise NotImplementedError()
+    def __init__(self, path, *args, **kwargs):
+        self._path = os.sep.join(path)
+        self._items = NotImplemented
 
     @property
     def files(self):
         """Yield all TorrentFiles recursively"""
         for entry in self._items.values():
             if entry.nodetype == 'leaf':
                 yield entry
@@ -87,14 +89,18 @@
                 yield (name, entry)
                 yield from entry.directories
 
     @property
     def path(self):
         return self._path
 
+    @property
+    def id(self):
+        return tuple(f['id'] for f in self.files)
+
     def __repr__(self):
         return '<%s %r>' % (type(self).__name__, self._items)
 
     def __getitem__(self, key):
         return self._items[key]
 
     def __iter__(self):
```

### Comparing `stig-0.8.3a0/stig/client/utils.py` & `stig-0.9.0a0/stig/tui/views/setting_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,212 +5,195 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
+from ...logging import make_logger
+log = make_logger(__name__)
 
-class PerfectInterval():
-    """Remove processing time from intervals"""
+import urwid
 
-    def __init__(self, loop):
-        self._loop = loop
-        self._last_timestamp = 0
-
-    def __call__(self, seconds):
-        now = self._loop.time()
-        if self._last_timestamp <= 0:
-            self._last_timestamp = int(now)
-            return seconds
-        else:
-            expected = self._last_timestamp + seconds
-            diff = now - expected
-            interval = seconds - diff
-            self._last_timestamp += seconds
-            return interval
-
-
-import asyncio
-class SleepUneasy():
-    """Asynchronous sleep() that can be aborted"""
-
-    def __init__(self, loop):
-        self.loop = loop
-        self._interrupt = asyncio.Event(loop=self.loop)
-        self._perfint = PerfectInterval(self.loop)
-
-    async def sleep(self, seconds):
-        """Sleep for `seconds` or until `interrupt` is called"""
-        self._interrupt.clear()
-        # Remove processing time from seconds
-        seconds = self._perfint(seconds)
-        try:
-            await asyncio.wait_for(self._interrupt.wait(), timeout=seconds)
-        except asyncio.TimeoutError:
-            pass  # Interval passed without interrupt
-        finally:
-            self._interrupt.clear()
-
-    def interrupt(self):
-        """Stop sleeping"""
-        self._interrupt.set()
-
-
-from types import SimpleNamespace
-class Response(SimpleNamespace):
-    """Response to an API call
-
-    All API implementations should use this class to provide return values to
-    API calls.
-
-    success: Whether the call was a success
-    msgs: Sequence of messages; either strings or ClientError exceptions
-
-    Any other keyword arguments are made available as attributes.
-    """
-    def __init__(self, success=False, msgs=(), **kwargs):
-        super().__init__(success=bool(success), msgs=tuple(msgs), **kwargs)
-
-
-def lazy_property(after_creation=None):
-    """Property that replaces itself with the requested object when accessed
-
-    `after_creation` is called with the instance of the property.
-    """
-    # https://stackoverflow.com/a/6849299
-    class _lazy_property():
-        def __init__(self, fget):
-            self.fget = fget
-            self.func_name = fget.__name__
-            self.after_creation = after_creation
-
-        def __get__(self, obj, cls):
-            if obj is None:
-                return None
-            value = self.fget(obj)
-            setattr(obj, self.func_name, value)
-            if self.after_creation is not None:
-                self.after_creation(obj)
-            return value
-
-    return _lazy_property
-
-
-class LazyDict(dict):
-    """Dictionary with callables as values that return the actual value on demand"""
-    def __getitem__(self, key):
-        value = dict.__getitem__(self, key)
-        if callable(value):
-            value = value()
-            dict.__setitem__(self, key, value)
-        return value
-
-
-from urllib.parse import urlsplit
-from .errors import URLParserError
-class URL():
-    """Wrapper around `urllib.parse.urlsplit`"""
-
-    @staticmethod
-    def _parse_url(url_string):
-        # If no scheme is given, urlsplit() thinks the whole string is the path
-        if '://' not in str(url_string):
-            url_string = 'http://' + str(url_string)
+from .setting import TUICOLUMNS
+from . import (ItemWidgetBase, ListWidgetBase)
+from ...main import (localcfg, remotecfg, srvapi, aioloop)
+from ...utils.usertypes import (Bool, Option)
+
+
+def _change_setting(name, new_value, on_success=None):
+    remote_name = name[4:]  # Remove 'srv.'
 
-        # urlsplit() can raise all kinds of errors, and some of them only occur
-        # when accessing its attributes, e.g. when port is not a number
+    if name in localcfg:
         try:
-            url = urlsplit(url_string)
+            localcfg[name] = new_value
+        except ValueError as e:
+            log.error('Cannot set %s = %r: %s', name, new_value, e)
+        else:
+            if on_success is not None:
+                on_success()
+
+    elif remote_name in remotecfg:
+        async def setter():
             try:
-                url.port
-            except ValueError:
-                raise ValueError('Port is not an integer')
-            url_dict = {
-                'scheme': url.scheme, 'host': url.hostname, 'port': url.port, 'path': url.path,
-                'user': url.username, 'password': url.password,
-            }
-        except Exception as e:
-            raise URLParserError('%r: %s' % (url_string, e))
-
-        # Undefined parts should be None
-        for key in url_dict:
-            if url_dict[key] == '':
-                url_dict[key] = None
-
-        return url_dict
-
-    _obj_cache = {}
-    def __new__(cls, url):
-        if isinstance(url, cls):
-            return url
-
-        cache_id = url
-        cache = cls._obj_cache
-        url_dict = cache.get(cache_id)
-        if url_dict is None:
-            url_dict = cache[cache_id] = cls._parse_url(url)
-
-        obj = super().__new__(cls)
-        for attr in ('scheme', 'host', 'port', 'path', 'user', 'password'):
-            setattr(obj, attr, url_dict[attr])
-        return obj
-
-    @property
-    def has_auth(self):
-        """Whether user and password properties are set"""
-        return self.user is not None and self.password is not None
-
-    @property
-    def domain(self):
-        """TLD Domain"""
-        if not hasattr(self, '_domain_cached'):
-            host = self.host
-            if not host:
-                self._domain_cached = None
+                await remotecfg.set(remote_name, new_value)
+            except (ValueError, srvapi.ClientError) as e:
+                log.error('Cannot set %s = %r: %s', name, new_value, e)
             else:
-                if host.count('.') <= 1:
-                    self._domain_cached = host
-                else:
-                    parts = host.rsplit('.', maxsplit=2)
-                    self._domain_cached = '.'.join(parts[-2:])
-        return self._domain_cached
-
-    def __str__(self):
-        if not hasattr(self, '_cached_string'):
-            parts = []
-            if self.scheme:
-                parts.append('%s://' % self.scheme)
-            if self.user:
-                parts.append('%s' % self.user)
-                if self.password:
-                    parts.append(':%s' % self.password)
-                parts.append('@')
-            if self.host:
-                parts.append(self.host)
-            if self.port:
-                parts.append(':%s' % self.port)
-            if self.path:
-                parts.append('%s' % self.path)
-            self._cached_string = ''.join(parts)
-        return self._cached_string
-
-    def __setattr__(self, name, value):
-        super().__setattr__(name, value)
-        if name[0] != '_':
-            # Clear caches
-            if hasattr(self, '_cached_string'):
-                del self._cached_string
-            if name == 'host' and hasattr(self, '_domain_cached'):
-                del self._domain_cached
-
-    def __repr__(self):
-        return '<%s %s>' % (type(self).__name__, str(self))
+                if on_success is not None:
+                    on_success()
+        aioloop.create_task(setter())
+
+    else:
+        raise RuntimeError('Not a setting name: %r' % name)
+
+
+class SettingItemWidget(ItemWidgetBase):
+    palette_unfocused = 'settinglist'
+    palette_focused   = 'settinglist.focused'
+    columns_focus_map = {}
+    for col in TUICOLUMNS.values():
+        columns_focus_map.update(col.style.focus_map)
 
-    def __hash__(self):
-        return hash(str(self))
+    @property
+    def id(self):
+        return self.data['id']
+
+    def selectable(self):
+        return True
+
+    @property
+    def name(self):
+        if self._cells.exists('name'):
+            return self._cells.name.text.text
+
+    @property
+    def value_widget(self):
+        if self._cells.exists('value'):
+            return self._cells.value.base_widget
+
+    @property
+    def current_value(self):
+        if self._cells.exists('value'):
+            value_widget = self.value_widget
+            if isinstance(value_widget, urwid.Edit):
+                return value_widget.edit_text
+            elif hasattr(value_widget, 'get_tui_value'):
+                return value_widget.get_tui_value()
 
-    def __eq__(self, other):
-        return str(self) == str(other)
+    @property
+    def edit_mode(self):
+        if self._cells.exists('value'):
+            return isinstance(self._cells.value.base_widget, urwid.Edit)
+        return False
+
+    def keypress(self, size, key):
+        current_value = self.current_value
+        if current_value is None:
+            return key
+        elif isinstance(current_value, Bool):
+            return self._keypress_bool(size, key)
+        elif isinstance(current_value, Option):
+            return self._keypress_option(size, key)
+        else:
+            return self._keypress_string(size, key)
+
+    def _keypress_bool(self, size, key):
+        cmd = self._command_map[key]
+        if cmd is urwid.ACTIVATE:
+            new_value = not self.current_value
+            _change_setting(self.name, new_value)
+        else:
+            return key
+
+    def _keypress_option(self, size, key):
+        cmd = self._command_map[key]
+        if cmd is urwid.ACTIVATE:
+            current_value = self.current_value
+            options = current_value.options
+            index = options.index(current_value)
+            if index < len(options)-1:
+                index += 1
+            else:
+                index = 0
+            new_value = options[index]
+            _change_setting(self.name, new_value)
+        else:
+            return key
+
+    def _keypress_string(self, size, key):
+        cells = self._cells
+        cmd = self._command_map[key]
+        current_value = self.current_value
+        value_widget = self.value_widget
+
+        def edit():
+            attrmap = self._cells.value.attrmap
+            edit_widget = urwid.AttrMap(urwid.Edit(edit_text=str(current_value)),
+                                        attr_map=attrmap.attr_map,
+                                        focus_map=attrmap.focus_map)
+            cells.replace('value', edit_widget)
+            self._value_widget_temp = value_widget
+
+        def unedit():
+            cells.replace('value', self._value_widget_temp)
+            delattr(self, '_value_widget_temp')
+
+        if cmd is urwid.ACTIVATE:
+            if not self.edit_mode:
+                edit()
+            else:
+                new_value = value_widget.edit_text
+                _change_setting(self.name, new_value, on_success=unedit)
+        elif cmd is urwid.CANCEL:
+            if self.edit_mode:
+                unedit()
+        elif self.edit_mode:
+            key = super().keypress(size, key)
+            cmd = self._command_map[key]
+            # Don't allow user to focus next/previous setting when editing
+            if cmd not in (urwid.CURSOR_DOWN, urwid.CURSOR_UP):
+                return key
+        else:
+            return key
+
+
+class SettingListWidget(ListWidgetBase):
+    tuicolumns      = TUICOLUMNS
+    ListItemClass   = SettingItemWidget
+    keymap_context  = 'setting'
+    palette_name    = 'settinglist'
+    focusable_items = True
+
+    def __init__(self, srvapi, keymap, sort=None, columns=None, title='Settings'):
+        super().__init__(srvapi, keymap, columns=columns, sort=sort, title=title)
+        self._sort = sort
+        localcfg.on_change(self._handle_update)
+        remotecfg.on_update(self._handle_update)
+        self.refresh()
+
+    def _handle_update(self, *_, **__):
+        self._data_dict = {
+            **{k: {'id': k,
+                   'value': v,
+                   'default': localcfg.default(k),
+                   'description': localcfg.description(k)}
+               for k,v in localcfg.items()},
+            **{'srv.'+k: {'id': 'srv.'+k,
+                          'value': v,
+                          'default': '',
+                          'description': remotecfg.description(k)}
+               for k,v in remotecfg.items()},
+        }
+        self._invalidate()
+
+    def refresh(self):
+        remotecfg.poll()
+
+    @property
+    def sort(self):
+        return self._sort
 
-    def __ne__(self, other):
-        return str(self) != str(other)
+    @sort.setter
+    def sort(self, sort):
+        ListWidgetBase.sort.fset(self, sort)
+        self.refresh()
```

### Comparing `stig-0.8.3a0/stig/client/constants.py` & `stig-0.9.0a0/stig/client/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
+from .utils import Float
 
 class ConstantBase():
     pass
 
 def is_constant(obj):
     return isinstance(obj, ConstantBase)
 
@@ -38,11 +39,8 @@
         if init_value is not None:
             _constants_cache[name] = cls(init_value)
         else:
             _constants_cache[name] = cls()
     return _constants_cache[name]
 
 DISCONNECTED = get_constant('disconnected', repr='<disconnected>')
-UNLIMITED = get_constant('unlimited', bases=(float,), init_value='inf')
-DISABLED = get_constant('disabled', attrs={'__bool__': lambda self: False})
-ENABLED = get_constant('enabled', attrs={'__bool__': lambda self: True})
-RANDOM = get_constant('random', repr="'random'")
+UNLIMITED = get_constant('unlimited', bases=(Float,), init_value='inf')
```

### Comparing `stig-0.8.3a0/stig/client/poll.py` & `stig-0.9.0a0/stig/client/poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,18 @@
     @property
     def interval(self):
         """Seconds between polls"""
         return self._interval
 
     @interval.setter
     def interval(self, interval):
-        self._interval = interval
+        self._interval = float(interval)
         if self.running:
             self.poll()
 
     def __repr__(self):
-        return '<%s %s, callbacks=%s, error_callbacks=%s>' % (
-            type(self).__name__, self._debug_info['request'],
-            self._debug_info['update_cbs'], self._debug_info['error_cbs'])
+        if hasattr(self, '_debug_info'):
+            return '<%s %s, callbacks=%s, error_callbacks=%s>' % (
+                type(self).__name__, self._debug_info.get('request'),
+                self._debug_info.get('update_cbs'), self._debug_info.get('error_cbs'))
+        else:
+            return '<%s>' % type(self).__name__
```

### Comparing `stig-0.8.3a0/stig/client/trequestpool.py` & `stig-0.9.0a0/stig/client/trequestpool.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,48 +11,42 @@
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 import blinker
 import operator
 from functools import reduce
-from collections import abc
 
 from .poll import RequestPoller
-from .filters.tfilter import TorrentFilter
 
 
 class TorrentRequestPool(RequestPoller):
     """Combine multiple `TorrentAPI.torrents` requests into one
 
     The wanted Torrent keys from all subscribers are combined and added to the
     needed keys for TorrentFilter from all subscribers.
 
     After the combined torrents have arrived, split it back up by using each
     subscriber's filter and provide it to its callbacks as tuples.
     """
-    def __init__(self, srvapi, interval=1, autoconnect=True):
+    def __init__(self, srvapi, interval=1):
         self._api = srvapi.torrent
         self._tfilters = {}
         self._keys = {}
-        self._autoconnect = autoconnect
         super().__init__(request=None, interval=interval, loop=srvapi.loop)
-        self.on_response(self._handle_tlist)
+        self.on_response(self._handle_torrent_list)
 
     def register(self, sid, callback, keys=(), tfilter=None):
         """Add new request to request pool
 
         sid: Subscriber ID (any hashable)
         callback: Callable that receives a tuple of Torrents on updates
         keys: Wanted Torrent keys
         tfilter: None for all torrents or TorrentFilter instance
         """
-        if isinstance(tfilter, abc.Sequence):
-            tfilter = TorrentFilter('|'.join('id=%s' % tid for tid in tfilter))
-
         log.debug('Registering subscriber: %s', sid)
         event = blinker.signal(sid)
         event.connect(callback)
         self._keys[event] = tuple(keys)
         self._tfilters[event] = tfilter
 
         # It's possible that a currently ongoing request doesn't collect the
@@ -85,20 +79,19 @@
             kwargs['keys'] = reduce(operator.__add__, self._keys.values())
             # Filters also need certain keys
             for f in all_filters:
                 if f is not None:
                     kwargs['keys'] += f.needed_keys
 
             kwargs['keys'] = tuple(set(kwargs['keys']))
-            kwargs['autoconnect'] = self._autoconnect
             log.debug('Combined filters: %s', kwargs['torrents'])
             log.debug('Combined keys: %s', kwargs['keys'])
             self.set_request(self._api.torrents, **kwargs)
 
-    def _handle_tlist(self, response):
+    def _handle_torrent_list(self, response):
         # If the request failed, response is None and tlist is empty.
         tlist = response.torrents if response is not None else ()
 
         dead_subscribers = []
         def has_subscribers(event):
             if not bool(event.receivers):
                 dead_subscribers.append(event.name)
```

### Comparing `stig-0.8.3a0/stig/client/sorters/__init__.py` & `stig-0.9.0a0/stig/client/sorters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,35 +34,36 @@
             else:
                 items = sorted(items, key=key_getter, reverse=reverse)
 
         return items
 
 
 class SorterBase():
+    INVERT_CHARS = ('!', '.')
     SORTSPECS = NotImplemented
     DEFAULT_SORT = None
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
 
         # Map aliases to their original name
-        obj._aliases = {alias: sname
-                       for sname,s in cls.SORTSPECS.items()
-                       for alias in s.aliases}
+        obj._aliases = {alias:sname
+                        for sname,s in cls.SORTSPECS.items()
+                        for alias in s.aliases}
         return obj
 
     def __init__(self, sortstrings=()):
         sortspecs = []
         sortfuncs = []
-        strings = []         # String representations of sortspecs
+        strings = []   # String representations of sortspecs
 
         # Go through items in reverse because to want to deduplicate sort orders
         # while keeping the most recent one.
         for sortstring in reversed(sortstrings):
-            if sortstring[0] in ('!', '.'):
+            if sortstring[0] in self.INVERT_CHARS:
                 sortspecname, reverse = sortstring[1:], True
             else:
                 sortspecname, reverse = sortstring, False
 
             # Resolve alias
             if sortspecname in self._aliases:
                 sortspecname = self._aliases[sortspecname]
@@ -71,15 +72,15 @@
                 raise ValueError('Unknown sort order: {!r}'.format(sortspecname))
             else:
                 sortspec = self.SORTSPECS[sortspecname]
                 if sortspec not in sortspecs:
                     sortfunc = partial(sortspec, reverse=reverse)
                     sortspecs.insert(0, sortspec)
                     sortfuncs.insert(0, sortfunc)
-                    strings.insert(0, ('!' if reverse else '') + sortspecname)
+                    strings.insert(0, (self.INVERT_CHARS[0] if reverse else '') + sortspecname)
         self._strings = tuple(strings)
 
         # Unless we already sort by DEFAULT_SORT, insert it as the first one.
         if self.DEFAULT_SORT is not None:
             default_sortspec = self.SORTSPECS[self.DEFAULT_SORT]
             if default_sortspec not in sortspecs:
                 sortfuncs.insert(0, default_sortspec)
```

### Comparing `stig-0.8.3a0/stig/client/sorters/tsorter.py` & `stig-0.9.0a0/stig/client/sorters/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,103 +19,112 @@
         description = 'Sort torrents by %s' % description
         super().__init__(*args, description=description, **kwargs)
         self.needed_keys = needed_keys
 
 
 class TorrentSorter(SorterBase):
     SORTSPECS = {
+        'id':                _SortSpec(lambda t: t['id'],
+                                       needed_keys=('id',),
+                                       description='ID'),
         'name':              _SortSpec(lambda t: t['name'].lower(),
-                                       aliases=('torrent',),
+                                       aliases=('n',),
                                        needed_keys=('name',),
                                        description='name'),
         'path':              _SortSpec(lambda t: t['path'],
                                        aliases=('dir',),
                                        needed_keys=('path',),
                                        description='download location'),
         'status':            _SortSpec(lambda t: t['status'],
-                                       aliases=('state',),
+                                       aliases=('st',),
                                        needed_keys=('status',),
                                        description='current status (idle, uploading, verifying, etc.)'),
         'error':             _SortSpec(lambda t: t['error'],
+                                       aliases=('err',),
                                        needed_keys=('error',),
                                        description='error message'),
+        'uploaded':          _SortSpec(lambda t: t['size-uploaded'],
+                                       aliases=('up',),
+                                       needed_keys=('size-uploaded',),
+                                       description='number of uploaded bytes'),
+        'downloaded':        _SortSpec(lambda t: t['size-downloaded'],
+                                       aliases=('dn',),
+                                       needed_keys=('size-downloaded',),
+                                       description='number of downloaded bytes'),
+        '%downloaded':       _SortSpec(lambda t: t['%downloaded'],
+                                       lambda t: t['%metadata'],
+                                       lambda t: t['%verified'],
+                                       aliases=('%dn',),
+                                       needed_keys=('%downloaded', '%metadata', '%verified'),
+                                       description='downloading or verifying progress'),
         'size':              _SortSpec(lambda t: t['size-final'],
+                                       aliases=('sz',),
                                        needed_keys=('size-final',),
                                        description='number of bytes of all wanted files'),
         'peers':             _SortSpec(lambda t: t['peers-connected'],
+                                       aliases=('prs',),
                                        needed_keys=('peers-connected',),
                                        description='connected peers'),
         'seeds':             _SortSpec(lambda t: t['peers-seeding'],
+                                       aliases=('sds',),
                                        needed_keys=('peers-seeding',),
                                        description='highest number of seeds reported by any tracker'),
         'ratio':             _SortSpec(lambda t: t['ratio'],
+                                       aliases=('rto',),
                                        needed_keys=('ratio',),
                                        description='upload/download ratio'),
-        'rate-down':         _SortSpec(lambda t: t['rate-down'],
-                                       aliases=('rdn',),
-                                       needed_keys=('rate-down',),
-                                       description='download rate'),
         'rate-up':           _SortSpec(lambda t: t['rate-up'],
                                        aliases=('rup',),
                                        needed_keys=('rate-up',),
                                        description='upload rate'),
+        'rate-down':         _SortSpec(lambda t: t['rate-down'],
+                                       aliases=('rdn',),
+                                       needed_keys=('rate-down',),
+                                       description='download rate'),
         'rate':              _SortSpec(lambda t: t['rate-up'] + t['rate-down'],
+                                       aliases=('r',),
                                        needed_keys=('rate-up', 'rate-down'),
                                        description='combined download and upload rate'),
-        'rate-limit-down':   _SortSpec(lambda t: t['rate-limit-down'],
-                                       aliases=('rldn',),
-                                       needed_keys=('rate-limit-down',),
-                                       description='download rate limit'),
-        'rate-limit-up':     _SortSpec(lambda t: t['rate-limit-up'],
-                                       aliases=('rlup',),
-                                       needed_keys=('rate-limit-up',),
+        'limit-rate-up':     _SortSpec(lambda t: t['limit-rate-up'],
+                                       aliases=('lrup',),
+                                       needed_keys=('limit-rate-up',),
                                        description='upload rate limit'),
-        'rate-limit':        _SortSpec(lambda t: t['rate-limit-up'] + t['rate-limit-down'],
-                                       aliases=('rl',),
-                                       needed_keys=('rate-limit-up', 'rate-limit-down'),
+        'limit-rate-down':   _SortSpec(lambda t: t['limit-rate-down'],
+                                       aliases=('lrdn',),
+                                       needed_keys=('limit-rate-down',),
+                                       description='download rate limit'),
+        'limit-rate':        _SortSpec(lambda t: t['limit-rate-up'] + t['limit-rate-down'],
+                                       aliases=('lr',),
+                                       needed_keys=('limit-rate-up', 'limit-rate-down'),
                                        description='combined download and upload rate limit'),
-        'uploaded':          _SortSpec(lambda t: t['size-uploaded'],
-                                       aliases=('up',),
-                                       needed_keys=('size-uploaded',),
-                                       description='number of uploaded bytes'),
-        'downloaded':        _SortSpec(lambda t: t['size-downloaded'],
-                                       aliases=('dn',),
-                                       needed_keys=('size-downloaded',),
-                                       description='number of downloaded bytes'),
-        'progress':          _SortSpec(lambda t: t['%downloaded'],
-                                       lambda t: t['%metadata'],
-                                       lambda t: t['%verified'],
-                                       aliases=('%',),
-                                       needed_keys=('%downloaded', '%metadata', '%verified'),
-                                       description='downloading or verifying progress'),
         'tracker':           _SortSpec(lambda t: t['trackers'][0]['url-announce'].domain if t['trackers'] else '',
                                        aliases=('trk',),
                                        needed_keys=('trackers',),
                                        description='domain of first tracker'),
         'eta':               _SortSpec(lambda t: t['timespan-eta'],
                                        needed_keys=('timespan-eta',),
                                        description='estimated time to finish downloading'),
-        'time-created':      _SortSpec(lambda t: t['time-created'],
-                                       aliases=('t-create',),
+        'created':           _SortSpec(lambda t: t['time-created'],
+                                       aliases=('tcrt',),
                                        needed_keys=('time-created',),
                                        description='creation time'),
-        'time-added':        _SortSpec(lambda t: t['time-added'],
-                                       aliases=('t-add',),
+        'added':             _SortSpec(lambda t: t['time-added'],
+                                       aliases=('tadd',),
                                        needed_keys=('time-added',),
                                        description='time of addition'),
-        'time-started':      _SortSpec(lambda t: t['time-started'],
-                                       aliases=('t-start',),
+        'started':           _SortSpec(lambda t: t['time-started'],
+                                       aliases=('tsta',),
                                        needed_keys=('time-started',),
                                        description='start time'),
-        'time-activity':     _SortSpec(lambda t: t['time-activity'],
-                                       aliases=('t-active',),
+        'activity':          _SortSpec(lambda t: t['time-activity'],
+                                       aliases=('tact',),
                                        needed_keys=('time-activity',),
                                        description='time of latest upload/download activity'),
-        'time-completed':    _SortSpec(lambda t: t['time-completed'],
-                                       aliases=('t-comp',),
+        'completed':         _SortSpec(lambda t: t['time-completed'],
+                                       aliases=('tcmp',),
                                        needed_keys=('time-completed',),
                                        description='time of completion'),
     }
     DEFAULT_SORT = 'name'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `stig-0.8.3a0/stig/client/sorters/trksorter.py` & `stig-0.9.0a0/stig/client/sorters/tracker.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,33 +20,38 @@
 class TorrentTrackerSorter(SorterBase):
     SORTSPECS = {
         'torrent':         _SortSpec(lambda t: t['tname'].lower(),
                                      description='torrent name'),
         'tier':            _SortSpec(lambda t: t['tier'],
                                      description='tier number'),
         'domain':          _SortSpec(lambda t: t['domain'],
-                                     description='domain from announce URL',
-                                     aliases=('host',)),
-        'state':           _SortSpec(lambda t: t['state'],
-                                     description='tracker state'),
+                                     aliases=('dom',),
+                                     description='domain from announce URL'),
+        'status':          _SortSpec(lambda t: t['status'],
+                                     aliases=('st',),
+                                     description='tracker status'),
         'error':           _SortSpec(lambda t: t['error'],
+                                     aliases=('err',),
                                      description='error message'),
         'downloads':       _SortSpec(lambda t: t['count-downloads'],
+                                     aliases=('dns',),
                                      description='number of known downloads'),
         'leeches':         _SortSpec(lambda t: t['count-leeches'],
+                                     aliases=('lcs',),
                                      description='number of known downloading peers'),
         'seeds':           _SortSpec(lambda t: t['count-seeds'],
+                                     aliases=('sds',),
                                      description='number of known seeding peers'),
         'last-announce':   _SortSpec(lambda t: t['time-last-announce'],
-                                     aliases=('l-an',),
+                                     aliases=('lan',),
                                      description='last time the torrent was successfully announce'),
         'next-announce':   _SortSpec(lambda t: t['time-next-announce'],
-                                     aliases=('n-an',),
+                                     aliases=('nan',),
                                      description='next time the torrent is announced'),
         'last-scrape':     _SortSpec(lambda t: t['time-last-scrape'],
-                                     aliases=('l-sc',),
+                                     aliases=('lsc',),
                                      description='last time the torrent was successfully scrape'),
         'next-scrape':     _SortSpec(lambda t: t['time-next-scrape'],
-                                     aliases=('n-sc',),
+                                     aliases=('nsc',),
                                      description='next time the torrent is scraped'),
     }
     DEFAULT_SORT = 'torrent'
```

### Comparing `stig-0.8.3a0/stig/client/sorters/psorter.py` & `stig-0.9.0a0/stig/client/sorters/peer.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,36 +18,38 @@
     def __init__(self, *args, description='', **kwargs):
         description = 'Sort peers by %s' % description
         super().__init__(*args, description=description, **kwargs)
 
 
 class TorrentPeerSorter(SorterBase):
     SORTSPECS = {
-        'ip'        : _SortSpec(lambda t: t['ip'],
-                                description='IP address (alphabetically)'),
-        'port'      : _SortSpec(lambda t: t['port'],
-                                description='port number'),
-        'client'    : _SortSpec(lambda t: t['client'].lower(),
-                                description='client name'),
-        'country'   : _SortSpec(lambda t: t['country'].lower(),
-                                description='country'),
-        'progress'  : _SortSpec(lambda t: t['progress'],
-                                aliases=('%',),
-                                description='downloading progress'),
-        'rate-up'   : _SortSpec(lambda t: t['rate-up'],
-                                aliases=('rup',),
-                                description='upload rate (from your perspective)'),
-        'rate-down' : _SortSpec(lambda t: t['rate-down'],
-                                aliases=('rdn',),
-                                description='download rate (from your perspective)'),
-        'rate'      : _SortSpec(lambda t: t['rate-up'] + t['rate-down'],
-                                description='combined download and upload rate'),
-        'eta'       : _SortSpec(lambda t: t['eta'],
-                                description='estimated time they need to finish'),
-        'rate-est'  : _SortSpec(lambda t: t['rate-est'],
-                                aliases=('rdn',),
-                                description='estimated overall download rate of peer'),
-        'torrent'   : _SortSpec(lambda t: t['tname'].lower(),
-                                aliases=('name',),
-                                description='torrent name'),
+        'torrent'     : _SortSpec(lambda t: t['tname'].lower(),
+                                  description='torrent name'),
+        '%downloaded' : _SortSpec(lambda t: t['%downloaded'],
+                                  aliases=('%dn',),
+                                  description="peer's download progress"),
+        'rate-up'     : _SortSpec(lambda t: t['rate-up'],
+                                  aliases=('rup',),
+                                  description='upload rate (from our perspective)'),
+        'rate-down'   : _SortSpec(lambda t: t['rate-down'],
+                                  aliases=('rdn',),
+                                  description='download rate (from our perspective)'),
+        'rate-est'    : _SortSpec(lambda t: t['rate-est'],
+                                  aliases=('re',),
+                                  description="peer's estimated overall download rate"),
+        'rate'        : _SortSpec(lambda t: t['rate-up'] + t['rate-down'],
+                                  aliases=('r',),
+                                  description='combined download and upload rate'),
+        'eta'         : _SortSpec(lambda t: t['eta'],
+                                  description="peer's estimated remaining download time"),
+        'client'      : _SortSpec(lambda t: t['client'].lower(),
+                                  aliases=('cl',),
+                                  description="peer's client name"),
+        'country'     : _SortSpec(lambda t: t['country'].lower(),
+                                  aliases=('cn',),
+                                  description="peer's country"),
+        'ip'          : _SortSpec(lambda t: t['ip'],
+                                  description="peer's IP address (alphabetically)"),
+        'port'        : _SortSpec(lambda t: t['port'],
+                                  description="peer's port number"),
     }
     DEFAULT_SORT = 'torrent'
```

### Comparing `stig-0.8.3a0/stig/client/filters/trkfilter.py` & `stig-0.9.0a0/stig/client/filters/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """Filtering TrackerList items by various values"""
 
 from ..ttypes import TorrentTracker
 VALUETYPES = TorrentTracker.TYPES
-from . import (BoolFilterSpec, CmpFilterSpec, Filter, FilterChain, make_cmp_filter)
+from . import (BoolFilterSpec, Filter, FilterChain, make_cmp_filter)
 
 
 def _make_cmp_filter(*args, **kwargs):
     return make_cmp_filter(TorrentTracker.TYPES, *args, **kwargs)
 
 class SingleTrackerFilter(Filter):
     DEFAULT_FILTER = 'domain'
@@ -25,51 +25,57 @@
     # Filters without arguments
     BOOLEAN_FILTERS = {
         'all': BoolFilterSpec(
             lambda trk: True,
             aliases=('*',),
             description='All trackers'),
         'alive': BoolFilterSpec(
-            lambda trk: trk['error'] == '' or trk['state'] == 'inactive',
+            lambda trk: trk['error'] == '' or trk['status'] == 'inactive',
             description='Trackers we are trying to connect to'),
     }
 
     COMPARATIVE_FILTERS = {
         'tier'           : _make_cmp_filter('tier',
                                             description='Match VALUE against torrent tier'),
-        'domain'         : _make_cmp_filter('domain', aliases=('host',),
+        'domain'         : _make_cmp_filter('domain',
+                                            aliases=('dom',),
                                             description='Match VALUE against domain from announce URL'),
         'url-announce'   : _make_cmp_filter('url-announce',
-                                            aliases=('u-an',),
+                                            aliases=('an',),
                                             description='Match VALUE against announce URL'),
         'url-scrape'     : _make_cmp_filter('url-scrape',
-                                            aliases=('u-sc',),
+                                            aliases=('sc',),
                                             description='Match VALUE against scrape URL'),
-        'state'          : _make_cmp_filter('state',
-                                            description=('Match VALUE against tracker state '
-                                                         '(inactive, waiting, queued, announcing, scraping)')),
+        'status'         : _make_cmp_filter('status',
+                                            aliases=('st',),
+                                            description=('Match VALUE against tracker status '
+                                                         '(stopped, idle, queued, announcing, scraping)')),
         'error'          : _make_cmp_filter('error',
+                                            aliases=('err',),
                                             description='Match VALUE against error message from tracker'),
         'downloads'      : _make_cmp_filter('count-downloads',
+                                            aliases=('dns',),
                                             description='Match VALUE against number of known downloads'),
         'leeches'        : _make_cmp_filter('count-leeches',
+                                            aliases=('lcs',),
                                             description='Match VALUE against number of known downloading peers'),
         'seeds'          : _make_cmp_filter('count-seeds',
+                                            aliases=('sds',),
                                             description='Match VALUE against number of known seeding peers'),
         'last-announce'  : _make_cmp_filter('time-last-announce',
-                                            aliases=('l-an',),
+                                            aliases=('lan',),
                                             description='Match VALUE against time of last announce'),
         'next-announce'  : _make_cmp_filter('time-next-announce',
-                                            aliases=('n-an',),
+                                            aliases=('nan',),
                                             description='Match VALUE against time of next announce'),
         'last-scrape'    : _make_cmp_filter('time-last-scrape',
-                                            aliases=('l-sc',),
+                                            aliases=('lsc',),
                                             description='Match VALUE against time of last scrape'),
         'next-scrape'    : _make_cmp_filter('time-next-scrape',
-                                            aliases=('n-sc',),
+                                            aliases=('nsc',),
                                             description='Match VALUE against time of next scrape'),
     }
 
 
 class TorrentTrackerFilter(FilterChain):
     """One or more filters combined with & and | operators"""
     filterclass = SingleTrackerFilter
```

### Comparing `stig-0.8.3a0/stig/client/filters/__init__.py` & `stig-0.9.0a0/stig/client/filters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     DEFAULT_FILTER = None
 
     BOOLEAN_FILTERS = {}
     COMPARATIVE_FILTERS = {}
 
     @classmethod
     def _check_value(cls, name, value, op):
-        """Convert `value` to correct type for comparative filter `name`
+        """
+        Convert `value` to correct type for comparative filter `name`
 
         Also ensure operator `op` is compatible with `value`.
 
         Raises ValueError
         """
         if name not in cls.COMPARATIVE_FILTERS:
             return value
@@ -129,15 +130,15 @@
             if match is None:
                 raise ValueError('Invalid filter: {!r}'.format(filter_str))
             else:
                 name = match.group('name')
                 op = match.group('op') or None
                 invert = bool(match.group('invert1')) ^ bool(match.group('invert2'))
                 value = match.group('value')
-                value = None if value.strip() == '' else value
+                value = None if value == '' else value
 
         # No operator but a value doesn't make any sense
         if op is None and value is not None:
             raise ValueError('Malformed filter expression: {!r}'.format(filter_str))
 
         # Handle spaces around operator: If there's a space before the
         # operator, strip value.  Otherwise, preserve them.  In any case,
@@ -226,14 +227,16 @@
             return 'all'
         elif self._value is None:
             return ('!' if self._invert else '') + self._name
         else:
             name = self._name if self._name != self.DEFAULT_FILTER else ''
             op = ('!' if self._invert else '') + self._op
             val = str(self._value)
+            if val[0] == ' ' or val[-1] == ' ':
+                val = repr(val)
             return name + op + val
 
     @property
     def needed_keys(self):
         return self._needed_keys
 
     def __eq__(self, other):
@@ -253,15 +256,15 @@
 
 
 
 class FilterChain():
     """One or more filters combined with AND and OR operators"""
 
     filterclass = None
-    _op_regex = re.compile(r'([&|])')
+    _op_regex = re.compile(r'(?<!\\)([&|])')
 
     def __init__(self, filters=''):
         if not isinstance(self.filterclass, type) or not issubclass(self.filterclass, Filter):
             raise RuntimeError('Attribute "filterclass" must be set to a Filter class, not {!r}'
                                .format(self.filterclass))
 
         if isinstance(filters, str):  # Because str is also instance of abc.Sequence
@@ -287,14 +290,16 @@
             filters = []
             ops = []
             expect = 'filter'
             nofilter = self.filterclass()
             for i,part in enumerate(parts):
                 if expect is 'filter':
                     if part not in '&|':
+                        # Remove backslashes from escaped operators
+                        part = part.replace('\&', '&').replace('\|', '|')
                         f = self.filterclass(part)
                         if f == nofilter:
                             # part is something like 'all' or '*' - this
                             # disables all other filters
                             filters = []
                             ops = []
                             break
```

### Comparing `stig-0.8.3a0/stig/client/filters/pfilter.py` & `stig-0.9.0a0/stig/client/filters/peer.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,45 +29,47 @@
             aliases=('upg',),
             description='Peers we are uploading to'),
         'downloading': BoolFilterSpec(
             lambda p: p['rate-down'] > 0,
             aliases=('dng',),
             description='Peers we are downloading from'),
         'seeding': BoolFilterSpec(
-            lambda p: p['progress'] >= 100,
+            lambda p: p['%downloaded'] >= 100,
             aliases=('sdg',),
             description='Peers that have downloaded all data'),
     }
 
     COMPARATIVE_FILTERS = {
+        'downloaded': CmpFilterSpec(
+            lambda p, op, v: op(p['tsize'] * (p['%downloaded']/100), v),
+            aliases=('dn',),
+            description='Match VALUE against number of bytes peer has downloaded',
+            value_type=TorrentPeer.TYPES['tsize']),
+        '%downloaded': CmpFilterSpec(
+            lambda p, op, v: op(p['%downloaded'], v),
+            aliases=('%dn',),
+            description='Match VALUE against percentage of bytes peer has downloaded',
+            value_type=TorrentPeer.TYPES['%downloaded']),
         'client': CmpFilterSpec(
             lambda p, op, v: op(p['client'], v),
+            aliases=('cl',),
             description='Match VALUE against peer client',
             value_type=TorrentPeer.TYPES['client']),
         'country': CmpFilterSpec(
             lambda p, op, v: op(p['country'], v),
+            aliases=('cn',),
             description='Match VALUE against peer country',
             value_type=TorrentPeer.TYPES['country']),
         'ip': CmpFilterSpec(
             lambda p, op, v: op(p['ip'], v),
             description='Match VALUE against peer IP address',
             value_type=TorrentPeer.TYPES['ip']),
         'port': CmpFilterSpec(
             lambda p, op, v: op(p['port'], v),
             description='Match VALUE against peer port',
             value_type=TorrentPeer.TYPES['port']),
-        'downloaded': CmpFilterSpec(
-            lambda p, op, v: op(p['tsize'] * (p['progress']/100), v),
-            aliases=('dn',),
-            description='Match VALUE against number of bytes peer has downloaded',
-            value_type=TorrentPeer.TYPES['tsize']),
-        '%downloaded': CmpFilterSpec(
-            lambda p, op, v: op(p['progress'], v),
-            aliases=('%dn',),
-            description='Match VALUE against percentage of bytes peer has downloaded',
-            value_type=TorrentPeer.TYPES['progress']),
     }
 
 
 class TorrentPeerFilter(FilterChain):
     """One or more filters combined with & and | operators"""
     filterclass = SingleTorrentPeerFilter
```

### Comparing `stig-0.8.3a0/stig/client/filters/ffilter.py` & `stig-0.9.0a0/stig/client/filters/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """Filtering TorrentFiles by various values"""
 
-from ..ttypes import (TorrentFile, TorrentFilePriority)
+from ..ttypes import TorrentFile
 from . import (BoolFilterSpec, make_cmp_filter, Filter, FilterChain)
 
 
 def _make_cmp_filter(*args, **kwargs):
     return make_cmp_filter(TorrentFile.TYPES, *args, **kwargs)
 
 class SingleTorrentFileFilter(Filter):
@@ -27,27 +27,27 @@
             lambda f: True,
             aliases=('*',),
             description='All files'),
         'wanted': BoolFilterSpec(
             lambda f: f['is-wanted'],
             description='Wanted files'),
         'complete': BoolFilterSpec(
-            lambda f: f['progress'] >= 100,
+            lambda f: f['%downloaded'] >= 100,
             aliases=('comp',),
             description='Fully downloaded files'),
     }
 
     COMPARATIVE_FILTERS = {
-        'file'        : _make_cmp_filter('name', 'Match VALUE against file name', aliases=('name',)),
+        'name'        : _make_cmp_filter('name', 'Match VALUE against file name', aliases=('n',)),
         'path'        : _make_cmp_filter('path', 'Match VALUE against path in torrent', aliases=('dir',)),
-        'size'        : _make_cmp_filter('size-total', 'Match VALUE against file size'),
+        'size'        : _make_cmp_filter('size-total', 'Match VALUE against file size', aliases=('sz',)),
         'downloaded'  : _make_cmp_filter('size-downloaded',
                                          'Match VALUE against number of downloaded bytes',
                                          aliases=('dn',)),
-        '%downloaded' : _make_cmp_filter('progress',
+        '%downloaded' : _make_cmp_filter('%downloaded',
                                          'Match VALUE against percentage of downloaded bytes',
                                          aliases=('%dn',)),
         'priority'    : _make_cmp_filter('priority',
                                          'Match VALUE against download priority (off, low, normal, high)',
                                          aliases=('prio',)),
     }
```

### Comparing `stig-0.8.3a0/stig/client/filters/tfilter.py` & `stig-0.9.0a0/stig/client/filters/torrent.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """Filtering Torrents by their values"""
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
-import re
-
 from . import (BoolFilterSpec, CmpFilterSpec, make_cmp_filter,
                Filter, FilterChain)
 
 from ..ttypes import TYPES as VALUETYPES
 def _make_cmp_filter(*args, **kwargs):
     return make_cmp_filter(VALUETYPES, *args, **kwargs)
 
@@ -44,74 +42,71 @@
 class SingleTorrentFilter(Filter):
     DEFAULT_FILTER = 'name'
 
     # Filters without arguments
     BOOLEAN_FILTERS = {
         'all': BoolFilterSpec(
             lambda t: True,
+            aliases=('*',),
             description='All torrents',
-            needed_keys=(),
-            aliases=('*',)),
-
-        'leeching': BoolFilterSpec(
-            lambda t: t['%downloaded'] < 100 and _STATUS_STOPPED not in t['status'],
-            aliases=('lcg',),
-            description='Unstopped torrents downloading or waiting for seeds',
-            needed_keys=('%downloaded', 'status')),
-        'seeding': BoolFilterSpec(
-            lambda t: t['%downloaded'] >= 100 and _STATUS_STOPPED not in t['status'],
-            aliases=('sdg',),
-            description='Unstopped torrents with all wanted files downloaded',
-            needed_keys=('%downloaded', 'status')),
+            needed_keys=()),
         'complete': BoolFilterSpec(
             lambda t: t['%downloaded'] >= 100,
-            aliases=('comp',),
+            aliases=('cmp',),
             description='Torrents with all wanted files downloaded',
             needed_keys=('%downloaded',)),
         'incomplete': BoolFilterSpec(
             lambda t: t['%downloaded'] < 100,
-            aliases=('incomp',),
+            aliases=('inc',),
             description='Torrents with some wanted files not fully downloaded',
             needed_keys=('%downloaded',)),
         'stopped': BoolFilterSpec(
             lambda t: _STATUS_STOPPED in t['status'],
-            aliases=('stp', 'paused'),
+            aliases=('stp',),
             description='Torrents not allowed to up- or download',
             needed_keys=('status',)),
-
         'active': BoolFilterSpec(
             lambda t: t['peers-connected'] > 0 or _STATUS_VERIFY in t['status'],
             description='Torrents connected to peers or being verified',
             needed_keys=('peers-connected', 'status')),
-        'downloading': BoolFilterSpec(
-            lambda t: t['rate-down'] > 0,
-            aliases=('dng',),
-            description='Torrents using download bandwidth',
-            needed_keys=('rate-down',)),
         'uploading': BoolFilterSpec(
             lambda t: t['rate-up'] > 0,
             aliases=('upg',),
             description='Torrents using upload bandwidth',
             needed_keys=('rate-up',)),
+        'downloading': BoolFilterSpec(
+            lambda t: t['rate-down'] > 0,
+            aliases=('dng',),
+            description='Torrents using download bandwidth',
+            needed_keys=('rate-down',)),
         'verifying': BoolFilterSpec(
             lambda t: _STATUS_VERIFY in t['status'],
-            aliases=('vrf',),
+            aliases=('vfg',),
             description='Torrents being verified or queued for verification',
             needed_keys=('status',)),
+        'leeching': BoolFilterSpec(
+            lambda t: t['%downloaded'] < 100 and _STATUS_STOPPED not in t['status'],
+            aliases=('lcg',),
+            description='Unstopped torrents downloading or waiting for seeds',
+            needed_keys=('%downloaded', 'status')),
+        'seeding': BoolFilterSpec(
+            lambda t: t['%downloaded'] >= 100 and _STATUS_STOPPED not in t['status'],
+            aliases=('sdg',),
+            description='Unstopped torrents with all wanted files downloaded',
+            needed_keys=('%downloaded', 'status')),
         'idle': BoolFilterSpec(
             lambda t: (_STATUS_IDLE in t['status'] and
                        _STATUS_STOPPED not in t['status']),
             description='Unstopped torrents not using any bandwidth',
             needed_keys=('status',)),
         'isolated': BoolFilterSpec(
             lambda t: _STATUS_ISOLATED in t['status'],
             aliases=('isl',),
             description='Torrents that cannot discover new peers in any way',
             needed_keys=('status',)),
-
         'private': BoolFilterSpec(
             lambda t: t['private'],
             aliases=('prv',),
             description='Torrents connectable through trackers only',
             needed_keys=('private',)),
         'public': BoolFilterSpec(
             lambda t: not t['private'],
@@ -119,27 +114,39 @@
             description='Torrents connectable through DHT and/or PEX',
             needed_keys=('private',)),
     }
 
 
     # Filters with arguments
     COMPARATIVE_FILTERS = {
-        'connections': _make_cmp_filter('peers-connected', _desc('... number of connected peers'), aliases=('con',)),
-        '%downloaded': _make_cmp_filter('%downloaded', _desc('... percentage of downloaded bytes'), aliases=('%dn',)),
-        'downloaded':  _make_cmp_filter('size-downloaded', _desc('... number of downloaded bytes'), aliases=('dn',)),
-        'error':       _make_cmp_filter('error', _desc('... error message')),
-        'id':          _make_cmp_filter('id', _desc('... ID')),
-        'name':        _make_cmp_filter('name', _desc('... name'), aliases=('torrent',)),
-        'path':        _make_cmp_filter('path', _desc('... full path to download directory'), aliases=('dir',)),
-        'ratio':       _make_cmp_filter('ratio', _desc('... uploaded/downloaded ratio')),
-        'rate-down':   _make_cmp_filter('rate-down', _desc('... download rate'), aliases=('rdn',)),
-        'rate-up':     _make_cmp_filter('rate-up', _desc('... upload rate'), aliases=('rup',)),
-        'seeds':       _make_cmp_filter('peers-seeding', _desc('... largest number of seeds reported by any tracker')),
-        'size':        _make_cmp_filter('size-final', _desc('... combined size of all wanted files')),
-        'uploaded':    _make_cmp_filter('size-uploaded', _desc('... number of uploaded bytes'), aliases=('up',)),
+        'id'          : _make_cmp_filter('id', _desc('... ID')),
+        'name'        : _make_cmp_filter('name', _desc('... name'),
+                                         aliases=('n',)),
+        'path'        : _make_cmp_filter('path', _desc('... full path to download directory'),
+                                         aliases=('dir',)),
+        'error'       : _make_cmp_filter('error', _desc('... error message'),
+                                         aliases=('err',)),
+        'uploaded'    : _make_cmp_filter('size-uploaded', _desc('... number of uploaded bytes'),
+                                         aliases=('up',)),
+        'downloaded'  : _make_cmp_filter('size-downloaded', _desc('... number of downloaded bytes'),
+                                         aliases=('dn',)),
+        '%downloaded' : _make_cmp_filter('%downloaded', _desc('... percentage of downloaded bytes'),
+                                         aliases=('%dn',)),
+        'size'        : _make_cmp_filter('size-final', _desc('... combined size of all wanted files'),
+                                         aliases=('sz',)),
+        'peers'       : _make_cmp_filter('peers-connected', _desc('... number of connected peers'),
+                                         aliases=('prs',)),
+        'seeds'       : _make_cmp_filter('peers-seeding', _desc('... largest number of seeds reported by any tracker'),
+                                         aliases=('sds',)),
+        'ratio'       : _make_cmp_filter('ratio', _desc('... uploaded/downloaded ratio'),
+                                         aliases=('rto',)),
+        'rate-up'     : _make_cmp_filter('rate-up', _desc('... upload rate'),
+                                         aliases=('rup',)),
+        'rate-down'   : _make_cmp_filter('rate-down', _desc('... download rate'),
+                                         aliases=('rdn',)),
 
         'tracker': CmpFilterSpec(
             lambda t, op, v: any(op(tracker['url-announce'].domain, v)
                                  for tracker in t['trackers']),
             aliases=('trk',),
             description=_desc('... domain of the announce URL of trackers'),
             needed_keys=('trackers',),
@@ -149,49 +156,49 @@
         'eta': CmpFilterSpec(
             lambda t, op, v: t['timespan-eta'].is_known and op(t['timespan-eta'], v),
             description=_desc('... estimated time for torrent to finish'),
             needed_keys=('timespan-eta',),
             value_type=VALUETYPES['timespan-eta'],
             value_convert=VALUETYPES['timespan-eta'].from_string,
         ),
-        'time-created': CmpFilterSpec(
+        'created': CmpFilterSpec(
             lambda t, op, v: t['time-created'].is_known and op(t['time-created'], v),
-            aliases=('t-create',),
+            aliases=('tcrt',),
             description=_desc('... time torrent was created'),
             needed_keys=('time-created',),
             value_type=VALUETYPES['time-created'],
             value_convert=VALUETYPES['time-created'].from_string,
         ),
-        'time-added': CmpFilterSpec(
+        'added': CmpFilterSpec(
             lambda t, op, v: t['time-added'].is_known and op(t['time-added'], v),
-            aliases=('t-add',),
+            aliases=('tadd',),
             description=_desc('... time torrent was added'),
             needed_keys=('time-added',),
             value_type=VALUETYPES['time-added'],
             value_convert=VALUETYPES['time-added'].from_string,
         ),
-        'time-started': CmpFilterSpec(
+        'started': CmpFilterSpec(
             lambda t, op, v: t['time-started'].is_known and op(t['time-started'], v),
-            aliases=('t-start',),
+            aliases=('tsta',),
             description=_desc('... last time torrent was started'),
             needed_keys=('time-started',),
             value_type=VALUETYPES['time-started'],
             value_convert=VALUETYPES['time-started'].from_string,
         ),
-        'time-activity': CmpFilterSpec(
+        'activity': CmpFilterSpec(
             lambda t, op, v: t['time-activity'].is_known and op(t['time-activity'], v),
-            aliases=('t-active',),
+            aliases=('tact',),
             description=_desc('... last time torrent was active'),
             needed_keys=('time-activity',),
             value_type=VALUETYPES['time-activity'],
             value_convert=VALUETYPES['time-activity'].from_string,
         ),
-        'time-completed': CmpFilterSpec(
+        'completed': CmpFilterSpec(
             lambda t, op, v: t['time-completed'].is_known and op(t['time-completed'], v),
-            aliases=('t-comp',),
+            aliases=('tcmp',),
             description=_desc('... time all wanted files where downloaded'),
             needed_keys=('time-completed',),
             value_type=VALUETYPES['time-completed'],
             value_convert=VALUETYPES['time-completed'].from_string,
         ),
     }
```

### Comparing `stig-0.8.3a0/stig/__init__.py` & `stig-0.9.0a0/stig/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-from .version import __version__
-APPNAME = 'stig'
+from .__version__ import __version__
+__appname__ = __name__.split('.')[0]
+__url__ = 'https://github.com/rndusr/stig'
 
 def run():
-    from . import main
-    if main.cliargs['profile_file'] is not None:
-        main.logging.start_profiling(main.run,
-                                     filepath=main.cliargs['profile_file'],
-                                     statistical=False)
-    else:
-        main.run()
+    try:
+        from . import main
+        if main.cliargs['profile_file'] is not None:
+            main.logging.start_profiling(main.run,
+                                         filepath=main.cliargs['profile_file'],
+                                         statistical=False)
+        else:
+            main.run()
+    except KeyboardInterrupt:
+        pass
```

### Comparing `stig-0.8.3a0/stig/cliopts.py` & `stig-0.9.0a0/stig/cliopts.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/__main__.py` & `stig-0.9.0a0/stig/__main__.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/main.py` & `stig-0.9.0a0/stig/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,68 +5,84 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
+# Remove python from process name when running inside tmux
+import os
+if 'TMUX' in os.environ:
+    try:
+        from setproctitle import setproctitle
+    except ImportError:
+        pass
+    else:
+        from . import __appname__
+        setproctitle(__appname__)
+
+
 import sys
 import asyncio
 aioloop = asyncio.get_event_loop()
 
 
 from . import cliopts
-from . import logging
 cliargs, clicmds = cliopts.parse()
 
 
+from . import logging
 logging.setup(debugmods=cliargs['debug'], filepath=cliargs['debug_file'])
 logging.redirect_level('INFO', sys.stdout)
 log = logging.make_logger()
 
 
 from . import settings
-cfg = settings.Settings()
-settings.init_defaults(cfg)
-
-def _log_cfg_change(setting):
-    msg = '{} = {!s}'.format(setting.name, setting)
-    if setting.value == setting.default:
-        msg += ' (default)'
-    log.debug(msg)
-cfg.on_change(_log_cfg_change)
+localcfg = settings.Settings()
+settings.init_defaults(localcfg)
 
 
 from .helpmgr import HelpManager
 helpmgr = HelpManager()
-helpmgr.settings = cfg
+helpmgr.localcfg = localcfg
 
 
 from .client import API
-srvapi = API(url=cfg['srv.url'].value,
-             interval=cfg['tui.poll'].value,
+srvapi = API(host=localcfg['connect.host'],
+             port=localcfg['connect.port'],
+             path=localcfg['connect.path'],
+             user=localcfg['connect.user'],
+             password=localcfg['connect.password'],
+             tls=localcfg['connect.tls'],
+             interval=localcfg['tui.poll'],
              loop=aioloop)
-srvapi.bandwidth_unit = cfg['unit.bandwidth'].value
-srvapi.bandwidth_prefix = cfg['unitprefix.bandwidth'].value
-srvapi.size_unit = cfg['unit.size'].value
-srvapi.size_prefix = cfg['unitprefix.size'].value
+remotecfg = srvapi.settings
+helpmgr.remotecfg = remotecfg
+
 
-settings.init_server_defaults(cfg, srvapi.settings)
+from .client import geoip
+if geoip.available:
+    geoip.cachedir = localcfg['geoip.dir']
+else:
+    localcfg['geoip'] = False
+geoip.enabled = localcfg['geoip']
 
 
 from .commands import CommandManager
 cmdmgr = CommandManager(loop=aioloop)
 cmdmgr.resources.update(aioloop=aioloop,
                         srvapi=srvapi,
-                        cfg=cfg,
+                        cfg=localcfg,
+                        srvcfg=srvapi.settings,
                         helpmgr=helpmgr)
-helpmgr.commands = cmdmgr
 cmdmgr.load_cmds_from_module(
     'stig.commands.cli', 'stig.commands.tui',
 )
+helpmgr.cmdmgr = cmdmgr
+
 
 def _pre_run_hook(cmdline):
     # Change command before it is executed
 
     # If there is '-h' or '--help' in the arguments, replace it with 'help
     # <cmd>'.  This is dirty but easier than forcing argparse to ignore all
     # other arguments without calling sys.exit().
@@ -112,15 +128,15 @@
     # Decide if we run as a TUI or CLI
     if cliargs['tui']:
         cmdmgr.active_interface = 'tui'
     elif cliargs['notui']:
         cmdmgr.active_interface = 'cli'
     else:
         try:
-            cmdmgr.active_interface = guess_ui(clicmds, cmdmgr, cfg)
+            cmdmgr.active_interface = guess_ui(clicmds, cmdmgr)
         except UIGuessError as e:
             log.error('Unable to guess user interface')
             log.error('Provide one of these options: --tui/-t or --no-tui/-T')
             sys.exit(1)
         except CmdError as e:
             log.error(e)
             sys.exit(1)
@@ -135,25 +151,38 @@
                 return False
 
         # Exit if CLI commands fail
         if clicmds:
             success = cmdmgr.run_sync(clicmds, on_error=log.error)
             if not success:
                 return False
+
         return True
 
     exit_code = 0
 
     # Run commands either in CLI or TUI mode
     if cmdmgr.active_interface == 'cli':
         # Exit when pipe is closed (e.g. `stig help | head -1`)
         import signal
         signal.signal(signal.SIGPIPE, signal.SIG_DFL)
-        if not run_commands():
-            exit_code = 1
+
+        # Load geoip database
+        if localcfg['geoip']:
+            try:
+                aioloop.run_until_complete(geoip.load(loop=aioloop))
+            except geoip.GeoIPError as e:
+                log.error(e)
+                exit_code = 1
+
+        try:
+            if not run_commands():
+                exit_code = 1
+        except KeyboardInterrupt:
+            log.debug('Caught SIGINT')
 
     elif cmdmgr.active_interface == 'tui':
         from .tui import main as tui
         cmdmgr.resources.update(tui=tui)
         if not tui.run(run_commands):
             exit_code = 1
 
@@ -166,10 +195,26 @@
             task.cancel()
             try:
                 aioloop.run_until_complete(asyncio.wait_for(task, timeout=None))
                 task.result()
             except (asyncio.CancelledError, asyncio.TimeoutError):
                 pass
 
+    _cancel_unfinished_tasks()
     aioloop.run_until_complete(srvapi.rpc.disconnect('Quit'))
-    aioloop.close()
+    # # Closing the event loop raises "RuntimeError: Event loop is closed" (not
+    # # always) when a `run_in_executor` command (i.e. a thread) is cancelled.
+    # # https://github.com/python/asyncio/issues/258
+    # aioloop.close()
     sys.exit(exit_code)
+
+
+def _cancel_unfinished_tasks():
+    pending = (task for task in asyncio.Task.all_tasks() if not task.done())
+    for task in pending:
+        log.debug('Cancelling pending task: %r', task)
+        task.cancel()
+        try:
+            log.debug('Finishing pending task: %r', task)
+            aioloop.run_until_complete(task)
+        except asyncio.CancelledError:
+            pass
```

### Comparing `stig-0.8.3a0/stig/tui/scroll.py` & `stig-0.9.0a0/stig/tui/scroll.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,17 +122,17 @@
             self._scroll_action = SCROLL_LINE_DOWN
 
         elif command_map[key] == urwid.CURSOR_PAGE_UP:
             self._scroll_action = SCROLL_PAGE_UP
         elif command_map[key] == urwid.CURSOR_PAGE_DOWN:
             self._scroll_action = SCROLL_PAGE_DOWN
 
-        elif command_map[key] == urwid.CURSOR_MAX_LEFT:  # 'home'
+        elif command_map[key] == urwid.CURSOR_MAX_LEFT:   # 'home'
             self._scroll_action = SCROLL_TO_TOP
-        elif command_map[key] == urwid.CURSOR_MAX_RIGHT: # 'end'
+        elif command_map[key] == urwid.CURSOR_MAX_RIGHT:  # 'end'
             self._scroll_action = SCROLL_TO_END
 
         else:
             return key
 
         self._invalidate()
 
@@ -246,15 +246,15 @@
 class ScrollBar(urwid.WidgetDecoration):
     def sizing(self):
         return frozenset((BOX,))
 
     def selectable(self):
         return True
 
-    def __init__(self, widget, thumb_char='\u2588', trough_char=' ',
+    def __init__(self, widget, thumb_char=u'\u2588', trough_char=' ',
                  side=SCROLLBAR_RIGHT, width=1):
         """Box widget that adds a scrollbar to `widget`
 
         `widget` must be a box widget with the following methods:
           - `get_scrollpos` takes the arguments `size` and `focus` and returns
             the index of the first visible row.
           - `set_scrollpos` (optional; needed for mouse click support) takes the
@@ -296,15 +296,15 @@
 
         # Thumb shrinks/grows according to the ratio of
         # <number of visible lines> / <number of total lines>
         thumb_weight = min(1, maxrow / max(1, ow_rows_max))
         thumb_height = max(1, round(thumb_weight * maxrow))
 
         # Thumb may only touch top/bottom if the first/last row is visible
-        top_weight = pos / max(1, posmax)
+        top_weight = float(pos) / max(1, posmax)
         top_height = int((maxrow-thumb_height) * top_weight)
         if top_height == 0 and top_weight > 0:
             top_height = 1
 
         # Bottom part is remaining space
         bottom_height = maxrow - thumb_height - top_height
         assert thumb_height + top_height + bottom_height == maxrow
@@ -372,17 +372,17 @@
         ow = self._original_widget
         ow_size = self._original_widget_size
         handled = False
         if hasattr(ow, 'mouse_event'):
             handled = ow.mouse_event(ow_size, event, button, col, row, focus)
 
         if not handled and hasattr(ow, 'set_scrollpos'):
-            if button == 4: # scroll wheel up
+            if button == 4:    # scroll wheel up
                 pos = ow.get_scrollpos(ow_size)
                 ow.set_scrollpos(pos - 1)
                 return True
-            elif button == 5: # scroll wheel down
+            elif button == 5:  # scroll wheel down
                 pos = ow.get_scrollpos(ow_size)
                 ow.set_scrollpos(pos + 1)
                 return True
 
         return False
```

### Comparing `stig-0.8.3a0/stig/tui/urwidpatches.py` & `stig-0.9.0a0/stig/tui/urwidpatches.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,21 +56,72 @@
 
 urwid.command_map[Key('enter')]          = urwid.ACTIVATE
 urwid.command_map[Key('escape')]         = urwid.CANCEL
 urwid.command_map[Key('ctrl-g')]         = urwid.CANCEL
 urwid.command_map[Key('ctrl-l')]         = urwid.REDRAW_SCREEN
 
 
+import re
+import operator
+class Edit_readline(urwid.Edit):
+    def keypress(self, size, key):
+        def move_to_next_word(forward=True):
+            if forward:
+                match_iterator  = re.finditer(r'(\b\W+|$)', self.edit_text, flags=re.UNICODE)
+                match_positions = (m.start() for m in match_iterator)
+                op = operator.gt
+            else:
+                match_iterator  = re.finditer(r'(\w+\b|^)', self.edit_text, flags=re.UNICODE)
+                match_positions = reversed([m.start() for m in match_iterator])
+                op = operator.lt
+            for pos in match_positions:
+                if op(pos, self.edit_pos):
+                    self.set_edit_pos(pos)
+                    return pos
+
+        cmd = self._command_map[key]
+        if cmd is urwid.DELETE_TO_EOL:
+            self.edit_text = self.edit_text[:self.edit_pos]
+            return None
+        elif cmd is urwid.DELETE_LINE:
+            self.set_edit_text('')
+            return None
+        elif cmd is urwid.DELETE_CHAR_UNDER_CURSOR:
+            return super().keypress(size, 'delete')
+        elif cmd is urwid.CURSOR_WORD_RIGHT:
+            move_to_next_word(forward=True)
+            return None
+        elif cmd is urwid.CURSOR_WORD_LEFT:
+            move_to_next_word(forward=False)
+            return None
+        elif cmd is urwid.DELETE_WORD_LEFT:
+            start_pos = self.edit_pos
+            end_pos = move_to_next_word(forward=True)
+            if end_pos is not None:
+                self.set_edit_text(self.edit_text[:start_pos] + self.edit_text[end_pos:])
+            self.edit_pos = start_pos
+            return None
+        elif cmd is urwid.DELETE_WORD_RIGHT:
+            end_pos = self.edit_pos
+            start_pos = move_to_next_word(forward=False)
+            if start_pos is not None:
+                self.set_edit_text(self.edit_text[:start_pos] + self.edit_text[end_pos:])
+            return None
+        elif key == 'space':
+            return super().keypress(size, ' ')
+        else:
+            return super().keypress(size, key)
+
+urwid.Edit = Edit_readline
+
 
 # Limit the impact of the high CPU load bug
 # https://github.com/urwid/urwid/pull/86
 # https://github.com/urwid/urwid/issues/90
-from distutils.version import LooseVersion
-if LooseVersion(urwid.__version__) <= LooseVersion('1.3.1'):
-    urwid.AsyncioEventLoop._idle_emulation_delay = 1/25
+urwid.AsyncioEventLoop._idle_emulation_delay = 1/25
 
 
 # Raise UnicodeDecodeError properly
 # https://github.com/urwid/urwid/pull/92
 # https://github.com/urwid/urwid/pull/196
 class AsyncioEventLoop_patched(urwid.AsyncioEventLoop):
     def _exception_handler(self, loop, context):
@@ -92,39 +143,14 @@
         if self._exc_info:
             raise self._exc_info
 
 urwid.AsyncioEventLoop = AsyncioEventLoop_patched
 
 
 class ListBox_patched(urwid.ListBox):
-    def keypress(self, size, key):
-        # Offer key to focused widget first
-        # https://github.com/urwid/urwid/pull/233
-        focused_widget = self.focus
-        if focused_widget is not None and focused_widget.selectable() and \
-           focused_widget.keypress((size[0],), key) is None:
-            return None
-
-        # Add support for home/end keys
-        # https://github.com/urwid/urwid/pull/229
-        key = super().keypress(size, key)
-        if self.focus is not None:
-            if key == 'home':
-                self.focus_position = next(iter(self.body.positions()))
-                self.set_focus_valign('top')
-                self._invalidate()
-                return None
-            elif key == 'end':
-                self.focus_position = next(iter(self.body.positions(reverse=True)))
-                self.set_focus_valign('bottom')
-                self._invalidate()
-                return None
-        return key
-
-
     # Add support for ScrollBar class (see stig.tui.scroll)
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._rows_max = None
 
     def _invalidate(self):
         super()._invalidate()
```

### Comparing `stig-0.8.3a0/stig/tui/cli.py` & `stig-0.9.0a0/stig/tui/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 import urwid
-import re
-import operator
 import os
 
 
 class CLIEditWidget(urwid.Edit):
     """Edit widget with readline keybindings callbacks and a history"""
 
     def __init__(self, *args, on_change=None, on_accept=None, on_cancel=None,
@@ -32,85 +30,43 @@
         self._history = []
         self._history_size = history_size
         self._history_pos = -1
         self.history_file = history_file
         return super().__init__(*args, **kwargs)
 
     def keypress(self, size, key):
-        size = (size[0],)
         text_before = self.get_edit_text()
-        if self._command_map[key] is urwid.CURSOR_UP:
+        cmd = self._command_map[key]
+        if cmd is urwid.CURSOR_UP:
             self._set_history_prev()
             key = None
-        elif self._command_map[key] is urwid.CURSOR_DOWN:
+        elif cmd is urwid.CURSOR_DOWN:
             self._set_history_next()
             key = None
-        elif self._command_map[key] is urwid.DELETE_TO_EOL:
-            self.edit_text = self.edit_text[:self.edit_pos]
-            key = None
-        elif self._command_map[key] is urwid.DELETE_LINE:
-            self.set_edit_text('')
-            key = None
-        elif self._command_map[key] is urwid.DELETE_CHAR_UNDER_CURSOR:
-            return super().keypress(size, 'delete')
-        elif self._command_map[key] is urwid.CURSOR_WORD_RIGHT:
-            self.move_to_next_word(forward=True)
-            key = None
-        elif self._command_map[key] is urwid.CURSOR_WORD_LEFT:
-            self.move_to_next_word(forward=False)
-            key = None
-        elif self._command_map[key] is urwid.DELETE_WORD_LEFT:
-            start_pos = self.edit_pos
-            end_pos = self.move_to_next_word(forward=True)
-            if end_pos != None:
-                self.set_edit_text(self.edit_text[:start_pos] + self.edit_text[end_pos:])
-            self.edit_pos = start_pos
-            key = None
-        elif self._command_map[key] is urwid.DELETE_WORD_RIGHT:
-            end_pos = self.edit_pos
-            start_pos = self.move_to_next_word(forward=False)
-            if start_pos != None:
-                self.set_edit_text(self.edit_text[:start_pos] + self.edit_text[end_pos:])
-            key = None
-        elif self._command_map[key] is urwid.ACTIVATE:
+        elif cmd is urwid.ACTIVATE:
             self._append_to_history(self.edit_text)
             if self._on_accept is not None:
                 self._on_accept(self)
             self._history_pos = -1
             key = None
-        elif self._command_map[key] is urwid.CANCEL:
+        elif cmd is urwid.CANCEL:
             if self._on_cancel is not None:
                 self._on_cancel(self)
             self._history_pos = -1
             key = None
         elif key == 'space':
             return super().keypress(size, ' ')
         else:
             key = super().keypress(size, key)
+
         text_after = self.get_edit_text()
         if self._on_change is not None and text_before != text_after:
             self._on_change(self)
         return key
 
-    def move_to_next_word(self, forward=True):
-        if forward:
-            match_iterator  = re.finditer(r'(\b\W+|$)', self.edit_text,
-                                          flags=re.UNICODE)
-            match_positions = [m.start() for m in match_iterator]
-            op = operator.gt
-        else:
-            match_iterator  = re.finditer(r'(\w+\b|^)', self.edit_text,
-                                          flags=re.UNICODE)
-            match_positions = reversed([m.start() for m in match_iterator])
-            op = operator.lt
-        for pos in match_positions:
-            if op(pos, self.edit_pos):
-                self.set_edit_pos(pos)
-                return pos
-
     def _set_history_prev(self):
         # Remember whatever is currently in line when user starts exploring history
         if self._history_pos == -1:
             self._edit_text_cache = self.edit_text
         if self._history_pos+1 < len(self._history):
             self._history_pos += 1
             self.edit_text = self._history[self._history_pos]
```

### Comparing `stig-0.8.3a0/stig/tui/keymap.py` & `stig-0.9.0a0/stig/tui/keymap.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,28 +158,26 @@
         return '<KeyChain %s>' % str(self)
 
 
 class Keymapped():
     """Mixin class that provides a keypress method"""
 
     def keypress(self, size, key_orig):
-        keymap     = self.__keymap
-        context    = self.__context
-        callback   = self.__callback
-        parent_cls = self.__parent_cls
-
+        keymap   = self.__keymap
+        context  = self.__context
+        callback = self.__callback
         key_eval = Key(key_orig)
 
         def try_parent_class(key, sup=super()):
             if sup.selectable():
-                mro = sup.__self_class__.mro()
-                super_cls = mro[mro.index(sup.__thisclass__) + 1]
-                log.debug('%s: Offering %r to %s.keypress()', context, key, super_cls.__name__)
+                # mro = sup.__self_class__.mro()
+                # super_cls = mro[mro.index(sup.__thisclass__) + 1]
+                # log.debug('%s: Offering %r to %s.keypress()', context, key, super_cls.__name__)
                 key = sup.keypress(size, key)
-                log.debug('%s: %s.keypress() returned %r', context, super_cls.__name__, key)
+                # log.debug('%s: %s.keypress() returned %r', context, super_cls.__name__, key)
             return key
 
         log.debug('%s: %r / %r pressed', context, key_orig, key_eval)
 
         # Any started keychains have the highest priority
         if keymap.any_keychain_started:
             log.debug('%s: Advancing started keychain(s)', context)
@@ -191,17 +189,20 @@
         # Offer original key to original keypress() for built-in keys like up/down
         key_ = try_parent_class(key_orig)
         if key_ is None:
             return None
 
         # Offer our own key format to original keypress() in case there are any
         # Key instances in urwid.command_map
-        key_ = try_parent_class(key_eval)
-        if key_ is None:
-            return None
+        if str(key_orig) != str(key_eval):
+            key_ = try_parent_class(key_eval)
+            if key_ is None:
+                return None
+        else:
+            log.debug('%s: Not feeding %r to parent again (%r == %r)', context, key_eval, key_orig, key_eval)
 
         # Offer key to KeyMap
         key_ = keymap.evaluate(key_eval, context=context, callback=callback, widget=self)
         if key_ is None:
             # Key was evaluated() to some action
             return None
         elif key_ != key_eval:
@@ -214,18 +215,14 @@
         log.debug('%s: Returning %r', context, key_eval)
         return key_eval
 
     def selectable(self):
         return True
 
 
-NO_CONTEXT      = object()
-ALL_CONTEXTS    = object()
-DEFAULT_CONTEXT = 'default'
-
 class KeyMap():
     """Bind keys to actions in different contexts
 
     To bind keys to widgets, a new class is created that accepts user input by
     adding the methods `keypress` and `selectable` to the original class:
 
     >>> keymap = KeyMap()
@@ -237,22 +234,26 @@
     urwid.Edit_Keymapped
 
     Now you can use Password like any regular Edit widget:
 
     >>> pw = Password('', 'Enter password or <Alt-g> to generate one')
     """
 
+    NO_CONTEXT      = object()
+    ALL_CONTEXTS    = object()
+    DEFAULT_CONTEXT = 'default'
+
     def __init__(self, callback=None):
         self._default_callback = callback
-        self._actions = {DEFAULT_CONTEXT: {}}
+        self._actions = {self.DEFAULT_CONTEXT: {}}
 
         self._bindunbind_callbacks = blinker.Signal()
         self._keychain_callbacks = blinker.Signal()
         self._keychain_partial = []
-        self._keychain_context = NO_CONTEXT
+        self._keychain_context = self.NO_CONTEXT
 
     def clear(self):
         """Remove all keybindings"""
         contexts = self._actions
         for context in contexts:
             log.debug('%s: Removing all keybindings', context)
             contexts[context] = {}
@@ -299,15 +300,15 @@
         key = self.mkkey(key)
         if context not in self._actions:
             raise ValueError('Unknown context: {!r}'.format(context))
         elif key in self._actions[context]:
             del self._actions[context][key]
             log.debug('%s: Unmapped %r', context, key)
         else:
-            if context == DEFAULT_CONTEXT:
+            if context == self.DEFAULT_CONTEXT:
                 key_removed = self._unbind_from_urwid_command_map(key)
             else:
                 key_removed = False
 
             for k in tuple(self._actions[context]):
                 if isinstance(k, KeyChain) and k.startswith(key):
                     del self._actions[context][k]
@@ -335,15 +336,15 @@
         if not self.any_keychain_started:
             log.debug('%s: Evaluating %r as single key for widget %r', context, key, widget)
             action = self._get_single_key_action(key, context)
 
         # Try to advance keychains only if no keychain was started previously or
         # if that previously started keychain was in the same context as we're
         # in now.
-        if action is None and (self._keychain_context == NO_CONTEXT or
+        if action is None and (self._keychain_context == self.NO_CONTEXT or
                                self._keychain_context == context):
             log.debug('%s: Evaluating %r as chain key for widget %r', context, key, widget)
             action = self._get_keychain_action(key, context)
             if action is KeyChain.ADVANCE:
                 log.debug('%s:   %r was used to advance a keychain; locking context', context, key)
                 self._keychain_context = context
                 self._keychain_partial.append(key)
@@ -395,16 +396,16 @@
             raise RuntimeError('No callback given - unable to handle {!r}'.format(action))
 
     def _get_single_key_action(self, key, context=DEFAULT_CONTEXT):
         actions = self._actions[context]
         if key in actions:
             return actions[key]
 
-        if context is not DEFAULT_CONTEXT:
-            actions = self._actions[DEFAULT_CONTEXT]
+        if context is not self.DEFAULT_CONTEXT:
+            actions = self._actions[self.DEFAULT_CONTEXT]
             if key in actions:
                 return actions[key]
 
     def _get_keychain_action(self, key, context):
         partial = self._keychain_partial
         candidate = tuple(partial) + (key,)
         log.debug('%s: Getting keychain action for %s + %s:',
@@ -424,45 +425,45 @@
 
     def _keychains(self, context=ALL_CONTEXTS):
         def keychains_from(cntxt):
             for kc,action in self._actions[cntxt].items():
                 if isinstance(kc, KeyChain):
                     yield (kc, action)
 
-        if context is ALL_CONTEXTS:
+        if context is self.ALL_CONTEXTS:
             for cntxt in self.contexts:
                 yield from keychains_from(cntxt)
         else:
             yield from keychains_from(context)
 
     def _started_keychains(self, context=ALL_CONTEXTS):
         keychain_partial = self._keychain_partial
         for kc,action in self._keychains(context):
             if kc.startswith(keychain_partial):
                 yield (kc, action)
 
     def _reset_keychains(self, context=ALL_CONTEXTS):
         log.debug('%s: Resetting keychains', context)
         self._keychain_partial.clear()
-        self._keychain_context = NO_CONTEXT
+        self._keychain_context = self.NO_CONTEXT
         self._run_keychain_callbacks()
 
     @property
     def any_keychain_started(self):
         """Whether any keychain was started"""
         return bool(self._keychain_partial)
 
     @property
     def current_keychain(self):
         """Tuple of currently collected keychain keys"""
         return tuple(self._keychain_partial)
 
     def _run_keychain_callbacks(self):
         context = self._keychain_context
-        if context is NO_CONTEXT:
+        if context is self.NO_CONTEXT:
             self._keychain_callbacks.send(self, active_keychains=(), keys_given=())
         else:
             self._keychain_callbacks.send(self,
                                           active_keychains=self._started_keychains(context),
                                           keys_given=self.current_keychain)
 
     def on_keychain(self, callback):
@@ -490,16 +491,15 @@
         context: A descriptive string (or any other hashable object)
         """
         if context not in self._actions:
             self._actions[context] = {}
         clsname = cls.__name__ + '_Keymapped'
         return type(clsname,
                     (Keymapped, cls),
-                    {'_Keymapped__parent_cls': cls,
-                     '_Keymapped__keymap': self,
+                    {'_Keymapped__keymap': self,
                      '_Keymapped__context': context,
                      '_Keymapped__callback': staticmethod(callback)})
 
     _KEY_SPLIT_SPACE = re.compile(r' +')
     def mkkey(self, string):
         """Create Key or KeyChain instance from `string`
```

### Comparing `stig-0.8.3a0/stig/tui/__init__.py` & `stig-0.9.0a0/stig/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/tui/infobar.py` & `stig-0.9.0a0/stig/tui/infobar.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 import urwid
 
 from ..main import srvapi
-from ..main import cfg
+from ..main import localcfg
 from . import main as tui
 from ..client import constants as const
 
 
+# Workaround for urwid bug: When a Text widget is initialized with an empty
+# string, subsequent set_text() calls have no effect.
+EMPTY_TEXT = ' '
+
+
 class KeyChainsWidget(urwid.WidgetWrap):
     _selectable = False
     _sizing = ['flow']
 
     def __init__(self):
         self._pile = urwid.Pile([])
         super().__init__(urwid.AttrMap(self._pile, 'keychains'))
@@ -98,14 +103,15 @@
             if key is not None:
                 items.append([('topbar.help.space',  '   '),
                               ('topbar.help.key',    str(key)),
                               ('topbar.help.equals', ' '),
                               ('topbar.help.label',  label)])
 
         items = []
+        maybe_add_entry(items, 'Settings', get_key('tab set', contexts=('main', None)))
         maybe_add_entry(items, 'Prompt', get_key('tui show cli', contexts=('main', None)))
         maybe_add_entry(items, 'Quit', get_key('quit', contexts=('main', None)))
         maybe_add_entry(items, 'Help', get_first_key('tab help', contexts=('main', None)))
         self.set_text(items) if items else self.set_text('')
 
 
 class ConnectionStatusWidget(urwid.WidgetWrap):
@@ -114,27 +120,34 @@
         self._attrmap = urwid.AttrMap(self._text, 'topbar.host.disconnected')
         super().__init__(self._attrmap)
         srvapi.rpc.on('connecting', self._handle_connecting)
         srvapi.rpc.on('connected', self._handle_connected)
         srvapi.rpc.on('disconnected', self._handle_disconnected)
         srvapi.rpc.on('error', self._handle_error)
 
-    def _handle_connecting(self, url):
-        self._text.set_text('Connecting to {}:{}'.format(url.host, url.port))
+    @staticmethod
+    def _connection_string(rpc):
+        string = '%s:%s' % (rpc.host, int(rpc.port))
+        if rpc.tls:
+            string = 'https://' + string
+        return string
+
+    def _handle_connecting(self, rpc):
+        self._text.set_text('Connecting to %s' % self._connection_string(rpc))
         self._attrmap.set_attr_map({None: 'topbar.host.connecting'})
 
-    def _handle_connected(self, url):
-        self._text.set_text('{}:{} Transmission {}'.format(url.host, url.port, srvapi.rpc.version))
+    def _handle_connected(self, rpc):
+        self._text.set_text('%s Transmission %s' % (self._connection_string(rpc), rpc.version))
         self._attrmap.set_attr_map({None: 'topbar.host.connected'})
 
-    def _handle_disconnected(self, url):
-        self._text.set_text(str(url))
+    def _handle_disconnected(self, rpc):
+        self._text.set_text(self._connection_string(rpc))
         self._attrmap.set_attr_map({None: 'topbar.host.disconnected'})
 
-    def _handle_error(self, url, error):
+    def _handle_error(self, rpc, error):
         from ..client import RPCError
         if not isinstance(error, RPCError):
             self._text.set_text(str(error))  # error should also contain url
             self._attrmap.set_attr_map({None: 'topbar.host.disconnected'})
 
 
 class BandwidthStatusWidget(urwid.Widget):
@@ -178,29 +191,29 @@
             self._text_dn.set_text((dn_attrs, dn.without_unit))
             self._connected = True
         else:
             self._connected = False
         self._invalidate()
 
     def _update_rate_limits(self, settings):
-        up = settings['rate-limit-up']
-        dn = settings['rate-limit-down']
+        up = settings['limit.rate.up']
+        dn = settings['limit.rate.down']
 
         # Empty display if DISCONNECTED or UNLIMITED
         as_str = lambda rate: '' if rate in (const.DISCONNECTED, const.UNLIMITED) \
                               else '/%s' % rate.without_unit
         self._text_up_limit.set_text(as_str(up))
         self._text_dn_limit.set_text(as_str(dn))
 
         self._up_limit_width = len(self._text_up_limit.text)
         self._dn_limit_width = len(self._text_dn_limit.text)
         self._invalidate()
 
     def _mk_tail_canv(self, direction, icon):
-        unit = {'bit': 'b', 'byte': 'B'}[cfg['unit.bandwidth'].value]
+        unit = {'bit': 'b', 'byte': 'B'}[localcfg['unit.bandwidth']]
         text = urwid.Text('%s/s%s' % (unit, icon))
         attr_text = urwid.AttrMap(text, 'bottombar.bandwidth.%s' % direction)
         return attr_text.render((self._TAIL_WIDTH,))
 
     def render(self, size, focus=False):
         if not self._connected:
             size = self.pack(size)
@@ -242,15 +255,15 @@
                self._dn_limit_width + self._up_limit_width + \
                self._SPACER_WIDTH
         return (cols, 1)
 
 
 class TorrentCountersWidget(urwid.WidgetWrap):
     def __init__(self):
-        self._text = urwid.Text(' ')
+        self._text = urwid.Text(EMPTY_TEXT)
         super().__init__(urwid.AttrMap(self._text, 'bottombar'))
         tui.srvapi.status.on_update(self._update_counters)
 
     def _update_counters(self, status):
         counters = status.count
         if const.DISCONNECTED in counters:
             self._text.set_text('')
@@ -265,8 +278,24 @@
         text = ['%s torrents' % counters.total]
         if parts:
             text[-1] += ': ' + ', '.join(parts)
 
         if counters.isolated > 0:
             text[-1] += ', '
             text.append(('bottombar.important', '%s isolated' % counters.isolated))
+
         self._text.set_text(text)
+
+
+class MarkedItemsWidget(urwid.WidgetWrap):
+    def __init__(self):
+        self._text = urwid.Text('.')
+        super().__init__(urwid.AttrMap(self._text, 'bottombar.marked'))
+
+    def update(self, count):
+        if count > 0:
+            new_text = '%d marked' % count
+        else:
+            new_text = EMPTY_TEXT
+
+        if new_text != self._text.text:
+            self._text.set_text(new_text)
```

### Comparing `stig-0.8.3a0/stig/tui/tabs.py` & `stig-0.9.0a0/stig/tui/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 import urwid
 import collections
 
-from ..utils import strwidth
+from ..utils.string import strwidth
 
 
 class TabID(int):
     def __repr__(self):
         return '<TabID %d>' % self
 
 
@@ -356,24 +356,25 @@
         return True
 
     def keypress(self, size, key):
         focus_widget = self.focus
 
         if focus_widget is not None:
             if len(size) > 1:
-                #       maxcol   maxrow (-1 for the tab bar)
-                size = (size[0], size[1]-1)
+                cols, rows = size
+                size = (cols, rows - self._tabbar.rows((cols,)))
             else:
                 size = (size[0],)
 
             if focus_widget.selectable():
                 key = focus_widget.keypress(size, key)
 
         if key is not None:
             focus_pos = self.focus_position
-            if key == 'left' and focus_pos > 0:
+            cmd = self._command_map[key]
+            if cmd == urwid.CURSOR_LEFT and focus_pos > 0:
                 self.focus_position -= 1
                 key = None
-            elif key == 'right' and focus_pos < len(self._contents)-1:
+            elif cmd == urwid.CURSOR_RIGHT and focus_pos < len(self._contents)-1:
                 self.focus_position += 1
                 key = None
         return key
```

### Comparing `stig-0.8.3a0/stig/tui/main.py` & `stig-0.9.0a0/stig/tui/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,50 +10,41 @@
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
 import urwid
 from . import urwidpatches
-from ..main import (aioloop, cfg, cmdmgr, srvapi, helpmgr)
+from ..main import (aioloop, localcfg, cmdmgr, srvapi, geoip)
 
 
-#
 # Keybindings
-#
-
-KEYMAP_CONTEXTS = ('main', 'tabs', 'torrentlist', 'torrent', 'filelist', 'file',
-                   'peerlist', 'trackerlist', 'tracker')
-
 from ..settings.defaults import DEFAULT_KEYMAP
 from .keymap import KeyMap
 keymap = KeyMap(callback=lambda cmd,widget: cmdmgr.run_task(cmd, on_error=log.error))
 for args in DEFAULT_KEYMAP:
     if args['action'][0] == '<' and args['action'][-1] == '>':
         args['action'] = keymap.mkkey(args['action'])
     keymap.bind(**args)
-helpmgr.keymap = keymap
 
 
-#
 # Widgets
-#
-
 MAX_TAB_TITLE_WIDTH = 50
 
 from .group import Group
 from .tabs import (Tabs, TabBar)
 from .cli import CLIEditWidget
 from .logger import LogWidget
 from .infobar import (KeyChainsWidget, QuickHelpWidget, ConnectionStatusWidget,
-                      BandwidthStatusWidget, TorrentCountersWidget)
+                      BandwidthStatusWidget, TorrentCountersWidget, MarkedItemsWidget)
 from . import theme
 
 def load_theme(themeobj):
-    """Load theme from `themeobj`
+    """
+    Load theme from `themeobj`
 
     themeobj: See `theme.load`
 
     If `themeobj` is a string, does not have a path and does not exist in the
     current working directory, try to load it from the same path as the rc file.
     """
     import os
@@ -66,27 +57,42 @@
         themefilepath = os.path.join(os.path.dirname(rcfilepath), themeobj)
         if os.path.exists(themefilepath):
             theme.load(themefilepath, urwidscreen)
             return
     theme.load(themeobj, urwidscreen)
 
 
+
+def load_geoip_db():
+    """
+    Load geolocation database in a background task
+    """
+    def _handle_geoip_load_result(task):
+        try:
+            task.result()
+        except geoip.GeoIPError as e:
+            log.error(e)
+    task = aioloop.create_task(geoip.load(loop=aioloop))
+    task.add_done_callback(_handle_geoip_load_result)
+
+
+
 def _create_cli_widget():
     def on_cancel(widget):
         widget.set_edit_text('')
         widgets.hide('cli')
 
     def on_accept(widget):
         cmd = widget.get_edit_text()
         on_cancel(widget)
         cmdmgr.run_task(cmd, on_error=log.error)
 
     return CLIEditWidget(':',
                          on_accept=on_accept, on_cancel=on_cancel,
-                         history_file=cfg['tui.cli.history-file'].value)
+                         history_file=localcfg['tui.cli.history-file'])
 
 
 def _greedy_spacer():
     return urwid.Padding(urwid.Text(''))
 
 
 topbar = Group(cls=urwid.Columns)
@@ -96,21 +102,23 @@
 
 tabs = keymap.wrap(Tabs, context='tabs')(
     tabbar=urwid.AttrMap(TabBar(), 'tabs.unfocused')
 )
 
 bottombar = Group(cls=urwid.Columns)
 bottombar.add(name='counters', widget=TorrentCountersWidget(), options='pack')
-bottombar.add(name='spacer', widget=urwid.AttrMap(_greedy_spacer(), 'bottombar'))
+bottombar.add(name='spacer1', widget=urwid.AttrMap(_greedy_spacer(), 'bottombar'))
+bottombar.add(name='marked', widget=MarkedItemsWidget(), options='pack')
+bottombar.add(name='spacer2', widget=urwid.AttrMap(_greedy_spacer(), 'bottombar'))
 bottombar.add(name='bandwidth', widget=BandwidthStatusWidget(), options='pack')
 
 cli = urwid.AttrMap(_create_cli_widget(), 'cli')
 
-logwidget = LogWidget(height=cfg['tui.log.height'].value,
-                      autohide_delay=cfg['tui.log.autohide'].value)
+logwidget = LogWidget(height=int(localcfg['tui.log.height']),
+                      autohide_delay=localcfg['tui.log.autohide'])
 
 keychains = KeyChainsWidget()
 keymap.on_keychain(keychains.update)
 
 widgets = keymap.wrap(Group, context='main')(cls=urwid.Pile)
 widgets.add(name='topbar', widget=topbar, options='pack')
 widgets.add(name='main', widget=tabs)
@@ -121,71 +129,68 @@
 
 
 def unhandled_input(key):
     key = keymap.evaluate(key)
     if key is not None:
         log.debug('Unhandled key: %s', key)
 
-class ScreenRaw(urwid.raw_display.Screen):
-    """Set raw mode so that ctrl-c doesn't raise KeyboardInterrupt"""
-    def _start(self, *args, **kwargs):
-        super()._start(*args, **kwargs)
-        import os, tty
-        fd = self._term_input_file.fileno()
-        if os.isatty(fd):
-            tty.setraw(fd)
-
-urwidscreen = ScreenRaw()
+urwidscreen = urwid.raw_display.Screen()
 urwidloop = urwid.MainLoop(widgets,
                            screen=urwidscreen,
                            event_loop=urwid.AsyncioEventLoop(loop=aioloop),
                            unhandled_input=unhandled_input,
                            handle_mouse=False)
 
 
 def run(command_runner):
-    """Run commands and start TUI
+    """
+    Run commands and start TUI
 
     Return False if any of the commands failed, True otherwise.
     """
     # Don't catch theme.ParserError - a broken default theme should make us
     # croak obviously and horribly
-    theme.init(cfg['tui.theme'].default, urwidscreen)
+    theme.init(localcfg.default('tui.theme'), urwidscreen)
 
     # Load tui-specific hooks before commands run (commands may trigger hooks)
     from . import hooks
 
     try:
         if not command_runner():
             return False
     # Make 'quit' behave as expected
     except urwid.ExitMainLoop:
         return True
 
+    # Load/Download GeoIP database
+    if geoip.available and localcfg['geoip']:
+        load_geoip_db()
+
     # Start logging to TUI widget instead of stdout/stderr
     logwidget.enable()
 
     topbar.help.update()
 
     # If no tab has been opened by cli or rc file, open default tabs
     if len(tabs) <= 0:
-        for cmd in ( 'tab ls -c size,ratio,seeds,status,tracker,path,name,time-activity',
-                     'tab ls active|incomplete',
-                    ('tab ls downloading -c size,downloaded,progress,'
-                     'rate-down,time-completed,eta,path,name'),
-                    ('tab ls uploading -c size,uploaded,ratio,'
-                     'rate-up,connections,seeds,tracker,path,name -s ratio'),
-                    'tab ls stopped -c size,progress,seeds,time-activity,path,name',
-                    'tab ls isolated -c error,tracker,path,name -s tracker',
-                    'tab -t peers lsp -s eta,torrent',):
+        for cmd in ('tab ls -c seeds,status,ratio,path,name,tracker',
+                    'tab ls active|incomplete',
+                    'tab ls downloading -c size,downloaded,%downloaded,rate-down,completed,eta,path,name',
+                    'tab ls uploading -c size,ratio,uploaded,rate-up,peers,seeds,tracker,path,name',
+                    'tab -t peers lsp -s torrent',
+                    'tab ls stopped -s ratio,path -c size,%downloaded,seeds,ratio,activity,path,name',
+                    'tab ls isolated -c error,tracker,path,name -s tracker'):
             cmdmgr.run_sync(cmd, on_error=log.error)
         tabs.focus_position = 1
 
     try:
         # Start polling torrent lists, counters, bandwidth usage, etc.
         aioloop.run_until_complete(srvapi.start_polling())
+        old = urwidscreen.tty_signal_keys('undefined','undefined',
+                                          'undefined','undefined','undefined')
         urwidloop.run()
     finally:
+        urwidscreen.tty_signal_keys(*old)
         logwidget.disable()
         aioloop.run_until_complete(srvapi.stop_polling())
 
     return True
```

### Comparing `stig-0.8.3a0/stig/tui/group.py` & `stig-0.9.0a0/stig/tui/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         size_len = len(size)
         if size_len == 0:
             size = (0, 0)
         elif size_len == 1:
             size = (size[0], 0)
         return super().render(size, focus=False)
 
+    def rows(self, size, focus=False):
+        return 0
+
 
 class Group(urwid.WidgetWrap):
     """Wrapper aroung Pile or Columns widget
 
     The purpose of this class it o make adding/removing, hiding/showing and
     accessing widgets simpler.
     """
@@ -37,15 +40,14 @@
         Each mapping is then provided to the `add` method as keyword
         arguments.
 
         cls: `Columns` or `Pile` (or derivatives of either)
 
         All other keyword arguments are forwarded to `cls` on instantiation.
         """
-        self._cls = cls
         self._main = cls([], **kwargs)
         self._items_list = []
         self._items_dict = {}
         # Add initial widgets
         for widget in widgets:
             self.add(**widget)
         super().__init__(self._main)
@@ -137,18 +139,18 @@
         Raises ValueError if `name` already exists.
         """
         if self.exists(name):
             raise ValueError('Already added: {!r}'.format(name))
         else:
             options = self._parse_options(options)
             item = dict(
-                name = name,           # Descriptive, unique handle
-                widget = widget,       # Bare widget
-                options = options,     # urwid options tuple, e.g. ('given',10) or ('weight',50)
-                removable = removable, # Wether this item can be deleted
+                name = name,            # Descriptive, unique handle
+                widget = widget,        # Bare widget
+                options = options,      # urwid options tuple, e.g. ('given',10) or ('weight',50)
+                removable = removable,  # Wether this item can be deleted
             )
 
             if position == 'start':
                 position = 0
             elif position == 'end':
                 position = len(self._items_list)
 
@@ -230,39 +232,47 @@
                 contents.append(content)
             else:
                 contents[position] = content
 
             if item['widget'].selectable():
                 self.focus_name = item['name']
 
-    def hide(self, name):
-        """Hide widget specified by `name` and focus next selectable widget"""
+    def hide(self, name, free_space=True):
+        """
+        Hide widget specified by `name` and focus next selectable widget
+
+        If `free_space` is False, the widget's space is still occupied but
+        empty.  This only works for widgets with a relative size.
+        """
         if not self.exists(name):
             raise ValueError('Unknown item name: {!r}'.format(name))
         elif self.visible(name):
             position = self.get_position(name)
             item = self._get_item_by_name(name)
             opts = item['options']
 
+            if not free_space and opts[0] == 'weight':
+                placeholder_size = str(opts[1])
+            else:
+                placeholder_size = 0
+
             if len(self._items_list) == 1:
                 content = (_Fill(), self._parse_options('100'))
-            elif opts[0] == 'weight':
-                content = (_Fill(), self._parse_options(str(opts[1])))
             else:
-                content = (_Fill(), self._parse_options(0))
+                content = (_Fill(), self._parse_options(placeholder_size))
             self._main.contents[position] = content
 
             # Try to focus next selectable item
             self.focus_selectable(forward=False)
             self.focus_selectable(forward=True)
 
-    def toggle(self, name):
-        """Show widget if it's hidden and vice versa"""
+    def toggle(self, name, free_space=True):
+        """Show widget if it's hidden and vice versa (see also `hide`)"""
         if self.exists(name):
-            self.hide(name) if self.visible(name) else self.show(name)
+            self.hide(name, free_space=free_space) if self.visible(name) else self.show(name)
         else:
             raise ValueError('Unknown item name: {!r}'.format(name))
 
     def visible(self, name):
         """Whether widget is hidden or not"""
         item = self._get_item_by_name(name)
         content = (item['widget'], item['options'])
```

### Comparing `stig-0.8.3a0/stig/tui/views/trackerlist.py` & `stig-0.9.0a0/stig/tui/views/tracker_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-import urwid
-
-from ..scroll import ScrollBar
-from .trklist_columns import TUICOLUMNS
+from .tracker import TUICOLUMNS
 from . import (ItemWidgetBase, ListWidgetBase, stringify_torrent_filter)
 
 
 class TrackerItemWidget(ItemWidgetBase):
     palette_unfocused = 'trackerlist'
-    palette_focused   ='trackerlist.focused'
+    palette_focused   = 'trackerlist.focused'
     columns_focus_map = {}
     for col in TUICOLUMNS.values():
         columns_focus_map.update(col.style.focus_map)
 
+    @property
+    def id(self):
+        return self.data['tid']
+
+    @property
+    def torrent_id(self):
+        return self.data['tid']
+
 
 class TrackerListWidget(ListWidgetBase):
     tuicolumns      = TUICOLUMNS
     ListItemClass   = TrackerItemWidget
     keymap_context  = 'tracker'
     palette_name    = 'trackerlist'
     focusable_items = True
@@ -42,16 +47,15 @@
                 yield from trkfilter.apply(trackers)
         else:
             def filter_trackers(trackers):
                 yield from trackers
         self._maybe_filter_trackers = filter_trackers
 
         self._poller = self._srvapi.create_poller(
-            self._srvapi.torrent.torrents, torfilter, keys=('trackers', 'name', 'id'),
-            autoconnect=False
+            self._srvapi.torrent.torrents, torfilter, keys=('trackers', 'name', 'id')
         )
         self._poller.on_response(self._handle_trackers)
 
     def _handle_trackers(self, response):
         if response is None or not response.torrents:
             self.clear()
         else:
@@ -61,21 +65,28 @@
                 if self._trkfilter:
                     self._title_name += ' %s' % self._trkfilter
 
             # Create list items our base widget can handle
             def trackers_combined(torrents):
                 for t in torrents:
                     yield from self._maybe_filter_trackers(t['trackers'])
-            self._items = {trk['id']:trk for trk in trackers_combined(response.torrents)}
+            self._data_dict = {trk['id']:trk for trk in trackers_combined(response.torrents)}
         self._invalidate()
 
     def refresh(self):
         self._poller.poll()
 
     @property
     def sort(self):
         return self._sort
 
     @sort.setter
     def sort(self, sort):
         ListWidgetBase.sort.fset(self, sort)
         self._poller.poll()
+
+    @property
+    def focused_torrent_id(self):
+        """Torrent ID of the currently focused tracker or `None`"""
+        focused_widget = self._listbox.focus
+        if focused_widget is not None:
+            return focused_widget.torrent_id
```

### Comparing `stig-0.8.3a0/stig/tui/views/summary.py` & `stig-0.9.0a0/stig/tui/views/summary.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,37 +73,45 @@
             return urwid.Pile([('pack', header), section])
 
         grid = urwid.GridFlow([], cell_width=1, h_sep=3, v_sep=1, align='left')
         for section in sections:
             opts = grid.options('given', section.width)
             section_wrapped = add_title(section.title, section)
             grid.contents.append((section_wrapped, opts))
+        self._grid = grid
+        self._content = Scrollable(grid)
 
-        grid_sb = urwid.AttrMap(
-            ScrollBar(urwid.AttrMap(Scrollable(grid), 'torrentsummary')),
+        super().__init__(urwid.AttrMap(
+            ScrollBar(urwid.AttrMap(self._content, 'torrentsummary')),
             'scrollbar'
-        )
-        super().__init__(grid_sb)
+        ))
 
         # Register new request in request pool
         keys = set(('name',)).union(key for w in sections for key in w.needed_keys)
         self._poller = srvapi.create_poller(srvapi.torrent.torrents, (tid,), keys=keys)
         self._poller.on_response(self._handle_response)
+        self._poller.on_error(self._handle_error)
 
     def _handle_response(self, response):
         if response is not None and response.success:
             self._torrent = response.torrents[0]
+            self._content.original_widget = self._grid
             for w in self._sections.values():
                 w.update(self._torrent)
 
             # Set new tab title if necessary
             if self.title_updater is not None:
                 self.title_updater(self.title)
-        else:
-            self._torrent = {}
+        elif response is not None:
+            self._handle_error(*response.msgs)
+
+    def _handle_error(self, *errors):
+        self._torrent = {'name': None, 'id': None}
+        pile = urwid.Pile(urwid.Text(('torrentsummary.error', str(e))) for e in errors)
+        self._content.original_widget = pile
 
     @property
     def title(self):
         # self._title is user-specified title
         if self._title is not None:
             return self._title
         elif 'name' in self._torrent:
```

### Comparing `stig-0.8.3a0/stig/tui/views/plist_columns.py` & `stig-0.9.0a0/stig/tui/views/peer.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 """Column classes that display information in peer lists"""
 
 import urwid
 
 from ..table import ColumnHeaderWidget
 from . import (Style, CellWidgetBase)
-from ...views.peerlist import COLUMNS as _COLUMNS
+from ...views.peer import COLUMNS as _COLUMNS
 
 
 TUICOLUMNS = {}
 
-class TorrentName(_COLUMNS['torrent'], CellWidgetBase):
+class Torrent(_COLUMNS['torrent'], CellWidgetBase):
     width = ('weight', 100)
     style = Style(prefix='peerlist.torrent', focusable=False,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['torrent'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['torrent'] = TorrentName
+TUICOLUMNS['torrent'] = Torrent
 
 
 class Client(_COLUMNS['client'], CellWidgetBase):
     width = 30
     style = Style(prefix='peerlist.client', focusable=False,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['client'].header),
@@ -46,95 +46,97 @@
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['country'].header),
                            style.attrs('header'))
 
 TUICOLUMNS['country'] = Country
 
 
-class IPAddress(_COLUMNS['ip'], CellWidgetBase):
+class IP(_COLUMNS['ip'], CellWidgetBase):
+    width = ('weight', 50)
     style = Style(prefix='peerlist.ip', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['ip'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['ip'] = IPAddress
+    def update(self, data):
+        # Set IP address initially
+        super().update(data)
+
+        # Lookup hostname once per instance
+        from ...main import localcfg
+        if localcfg['reverse-dns']:
+            def set_hostname(hostname):
+                if self.text.text != hostname:
+                    self.text.set_text(hostname)
+            from ...client import rdns
+            rdns.query(data['ip'], callback=set_hostname)
+
+TUICOLUMNS['ip'] = IP
 
 
 class Port(_COLUMNS['port'], CellWidgetBase):
     style = Style(prefix='peerlist.port', focusable=False,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['port'].header),
                            style.attrs('header'))
 
 TUICOLUMNS['port'] = Port
 
 
-class Progress(_COLUMNS['progress'], CellWidgetBase):
-    style = Style(prefix='peerlist.progress', focusable=False,
+class PercentDownloaded(_COLUMNS['%downloaded'], CellWidgetBase):
+    style = Style(prefix='peerlist.%downloaded', focusable=False,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['progress'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['%downloaded'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value < 100 else None
 
-TUICOLUMNS['progress'] = Progress
+TUICOLUMNS['%downloaded'] = PercentDownloaded
 
 
-class RateDown(_COLUMNS['rate-down'], CellWidgetBase):
-    style = Style(prefix='peerlist.rate-down', focusable=False,
+class RateUp(_COLUMNS['rate-up'], CellWidgetBase):
+    style = Style(prefix='peerlist.rate-up', focusable=False,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-down'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-up'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value > 0 else None
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-down'].header['right']
-
-TUICOLUMNS['rate-down'] = RateDown
+TUICOLUMNS['rate-up'] = RateUp
 
 
-class RateUp(_COLUMNS['rate-up'], CellWidgetBase):
-    style = Style(prefix='peerlist.rate-up', focusable=False,
+class RateDown(_COLUMNS['rate-down'], CellWidgetBase):
+    style = Style(prefix='peerlist.rate-down', focusable=False,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-up'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-down'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value > 0 else None
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-up'].header['right']
-
-TUICOLUMNS['rate-up'] = RateUp
+TUICOLUMNS['rate-down'] = RateDown
 
 
 class ETA(_COLUMNS['eta'], CellWidgetBase):
     style = Style(prefix='peerlist.eta', focusable=False,
                   extras=('header',), modes=('highlighted',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['eta'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if bool(self.value) else None
 
 TUICOLUMNS['eta'] = ETA
 
 
-class EstimatedPeerRate(_COLUMNS['rate-est'], CellWidgetBase):
+class RateEst(_COLUMNS['rate-est'], CellWidgetBase):
     style = Style(prefix='peerlist.rate-est', focusable=False,
                   extras=('header',), modes=('highlighted',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-est'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value > 0 else None
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-est'].header['right']
-
-TUICOLUMNS['rate-est'] = EstimatedPeerRate
+TUICOLUMNS['rate-est'] = RateEst
```

### Comparing `stig-0.8.3a0/stig/tui/views/__init__.py` & `stig-0.9.0a0/stig/tui/views/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 import urwid
 import collections
 
+from ..table import ColumnHeaderWidget
+from ..main import bottombar
+
 
 class Style():
     """Map standard attributes to those defined in a urwid palette
 
     prefix: common prefix of all attributes
     extras: additional attributes (e.g. 'header')
     modes: additional subsections with 'focused' and 'unfocused' attributes
@@ -64,102 +67,103 @@
 
     @staticmethod
     def dotify(*strings):
         """Join non-empty strings with a '.'"""
         return '.'.join(x for x in (strings) if x)
 
 
-# TODO: It would be great if some columns (e.g. rate-up/down) would shrink to
-#       the widest visible value (including its header).  Other columns would
-#       share the remaining width using ('weight', x), giving some of them
-#       (e.g. name) more space than others (e.g. path).
 class CellWidgetBase(urwid.WidgetWrap):
     """Base class for cells in items in Torrent/File/Peer/... lists"""
 
     style = collections.defaultdict(lambda: 'default')
-    header = urwid.Padding(urwid.Text('NO HEADER SPECIFIED'))
+    header = urwid.AttrMap(ColumnHeaderWidget(left='', right=''), 'header')
     width = ('weight', 100)
     align = 'right'
 
     def __init__(self):
         self.value = None
-        self.text = urwid.Text('', wrap='clip', align=self.align)
+        self.text = urwid.Text('', wrap=self.wrap, align=self.align)
         self.attrmap = urwid.AttrMap(self.text, self.style.attrs('unfocused'))
         return super().__init__(self.attrmap)
 
     def update(self, data):
         self.data = data
         new_value = self.get_value()
         if self.value != new_value:
             self.value = new_value
             self.text.set_text(str(new_value))
             attr = self.style.attrs(self.get_mode(), focused=False)
             self.attrmap.set_attr_map({None: attr})
 
-    def get_value(self):
-        raise NotImplementedError()
-
     def get_mode(self):
         return None
 
+    @classmethod
+    def set_header(cls, left=None, right=None):
+        if left is not None:
+            cls.header.base_widget.left = str(left)
+        if right is not None:
+            cls.header.base_widget.right = str(right)
+
 
 class ItemWidgetBase(urwid.WidgetWrap):
     """Base class for items in Torrent/File/Peer/... lists"""
 
     # Derived classes must set these class attributes; lists with unfocusable
     # items (e.g. peer lists) don't have to set palette_focused and
     # columns_focus_map.
     columns_focus_map = NotImplemented
     palette_unfocused = NotImplemented
     palette_focused   = NotImplemented
 
-    def __init__(self, item, cells):
-        self._item = item    # Info of torrent/tracker/file/peer/...
+    def __init__(self, data, cells):
+        self._data = data    # Info of torrent/tracker/file/peer/... as mapping
         self._cells = cells  # Group instance that combines widgets horizontally
 
         # Create focusable or unfocusable item widget
         if self.columns_focus_map is not NotImplemented:
-            itemw = urwid.AttrMap(urwid.AttrMap(cells, attr_map=None, focus_map=self.columns_focus_map),
-                                  self.palette_unfocused, self.palette_focused)
+            item_widget = urwid.AttrMap(
+                urwid.AttrMap(cells, attr_map=None, focus_map=self.columns_focus_map),
+                self.palette_unfocused, self.palette_focused
+            )
         else:
-            itemw = urwid.AttrMap(cells, self.palette_unfocused)
-        urwid.WidgetWrap.__init__(self, itemw)
+            item_widget = urwid.AttrMap(cells, self.palette_unfocused)
+        urwid.WidgetWrap.__init__(self, item_widget)
 
         # Initialize cell widgets
-        self.update(item)
+        self.update(data)
 
-    def update(self, item):
+    def update(self, data):
         for widget in self._cells.widgets:
-            widget.update(item)
-        self._item = item
+            if hasattr(widget, 'update'):
+                widget.update(data)
+        self._data = data
 
     @property
     def id(self):
-        """ID of the displayed item"""
-        return self._item['id']
-
-    @property
-    def torrent_id(self):
-        """ID of the torrent the displayed item belongs to"""
-        item = self._item
-        return item['tid'] if 'tid' in item else item['id']
+        """Unique, hashable ID of the displayed item"""
+        raise NotImplementedError()
 
     @property
-    def item(self):
+    def data(self):
         """Displayed data in dictionary form"""
-        return self._item
+        return self._data
 
     @property
     def is_marked(self):
         """Whether this item has been marked by the user"""
-        return self._cells.marked.is_marked
+        if self._cells.exists('marked'):
+            return self._cells.marked.is_marked
+        else:
+            return False
 
     @is_marked.setter
     def is_marked(self, is_marked):
-        self._cells.marked.is_marked = bool(is_marked)
+        if self._cells.exists('marked'):
+            self._cells.marked.is_marked = bool(is_marked)
 
 
 
 from ..table import Table
 from ..scroll import ScrollBar
 class ListWidgetBase(urwid.WidgetWrap):
     """Base class for Torrent/File/Peer/... lists"""
@@ -176,26 +180,25 @@
         self._keymap = keymap
 
         if self.focusable_items:
             self._ListItemClass = keymap.wrap(self.ListItemClass, context=self.keymap_context)
         else:
             self._ListItemClass = self.ListItemClass
 
-        self._items = ()
+        self._data_dict = ()
         self._marked = set()
 
-        self._columns = columns or []
         self._sort = sort
         self._sort_orig = sort
 
         self._title_name = title
         self.title_updater = None
 
         self._table = Table(**self.tuicolumns)
-        self._table.columns = self._columns
+        self._table.columns = columns or ()
 
         if self.focusable_items:
             walker = urwid.SimpleFocusListWalker([])
         else:
             walker = urwid.SimpleListWalker([])
         self._listbox = keymap.wrap(urwid.ListBox, context=self.keymap_context + 'list')(walker)
 
@@ -216,57 +219,61 @@
         if self.title_updater is not None:
             # First argument can be cropped if too long, second argument is fixed
             # self.title_updater(self.title, ' [%d]' % self.count)
             self.title_updater(self.title, ' [%d]' % self.count)
         super()._invalidate()
 
     def render(self, size, focus=False):
-        if self._items is not None:
+        if self._data_dict is not None:
             self._update_listitems()
-            self._items = None
-        # focus=True because we always want to display the focused torrent, for
+            self._data_dict = None
+
+        # Update number of marked items in this list
+        bottombar.marked.update(len(self._marked))
+
+        # focus=True because we always want to highlight the focused item, for
         # example when the CLI is open
         return super().render(size, focus=True)
 
     def _update_listitems(self):
         # Remember focused item widget in case items get added or removed
         focusedw = self.focused_widget
 
         walker = self._listbox.body
-        item_dict = self._items
+        data_dict = self._data_dict
         dead_items = []
         for w in walker:  # w = *ItemWidget instance
             id = w.id
             try:
                 # Update existing *ItemWidget instances with new data
-                w.update(item_dict[id])
-                del item_dict[id]
+                w.update(data_dict[id])
+                del data_dict[id]
             except KeyError:
-                # Item no longer exists in self._items anymore
+                # Item no longer exists in data_dict anymore
                 dead_items.append(w)
 
         # Remove dead *ItemWidget instances
         marked = self._marked
         for w in dead_items:
             walker.remove(w)
             marked.discard(w)  # self._marked may have a reference too
 
         # Any items that haven't been used to update an existing *ItemWidget instance are new
-        if item_dict:
+        if data_dict:
             table = self._table
             cls = self._ListItemClass
-            for tid in item_dict:
-                table.register(tid)
-                itemw = table.get_row(tid)  # itemw = item widget
-                walker.append(cls(item_dict[tid], itemw))
+            for data_id in data_dict:
+                table.register(data_id)
+                item_widget = table.get_row(data_id)
+                walker.append(cls(data_dict[data_id], item_widget))
 
         # Sort items in walker
         if self._sort is not None:
             self._sort.apply(walker,
-                            item_getter=lambda w: w.item,
+                            item_getter=lambda w: w.data,
                             inplace=True)
 
         # Items could be added/removed - re-focus previously focused item if necessary
         if focusedw is not None and self.focused_widget is not None and \
            focusedw.id != self.focused_widget.id:
             focused_id = focusedw.id
             for i,w in enumerate(walker):
@@ -306,19 +313,19 @@
         else:
             self._sort = sort
 
     @property
     def count(self):
         """Number of listed items"""
         # If this method was called before rendering, the contents of the
-        # listbox widget are inaccurate and we have to use self._items.  But if
-        # we're called after rendering, self._items is reset to None and we have
-        # to count items in the listbox.
-        if self._items is not None:
-            return len(self._items)
+        # listbox widget are inaccurate and we have to use self._data_dict.  But
+        # if we're called after rendering, self._data_dict is reset to None and
+        # we have to count items in the listbox.
+        if self._data_dict is not None:
+            return len(self._data_dict)
         else:
             return len(self._listbox.body)
 
     @property
     def title_name(self):
         """The base name of the title"""
         return str(self._title_name or 'No title')
@@ -338,25 +345,29 @@
         parts = [self.title_name]
         sort = self.title_sort_order
         if sort:
             parts.append(sort)
         return ' '.join(parts)
 
 
+    @property
+    def has_marked_column(self):
+        return 'marked' in self._table.columns
+
     def mark(self, toggle=False, all=False):
         """Mark the currently focused item or all items"""
         self._set_mark(True, toggle=toggle, all=all)
 
     def unmark(self, toggle=False, all=False):
         """Unmark the currently focused item or all items"""
         self._set_mark(False, toggle=toggle, all=all)
 
     @property
     def marked(self):
-        """Generator that yields TorrentItemWidgets"""
+        """Generator that yields ItemWidgetBase descendants"""
         yield from self._marked
 
     def _set_mark(self, mark, toggle=False, all=False):
         if toggle and self.focused_widget is not None:
             mark = not self.focused_widget.is_marked
 
         for widget in self._select_items_for_marking(all):
@@ -391,40 +402,24 @@
     def focused_id(self):
         """ID of the currently focused list item or `None`"""
         focused_widget = self._listbox.focus
         if focused_widget is not None:
             return focused_widget.id
 
     @property
-    def focused_torrent_id(self):
-        """ID of the torrent that the currently focused list item belongs to or `None`"""
-        focused_widget = self._listbox.focus
-        if focused_widget is not None:
-            return focused_widget.torrent_id
-
-    @property
     def focus_position(self):
         """Focus position (first item is 0; `None` if list is empty)"""
         return self._listbox.focus_position
 
     @focus_position.setter
     def focus_position(self, focus_position):
         self._listbox.focus_position = min(focus_position, len(self._listbox.body)-1)
 
 
 def stringify_torrent_filter(tfilter, torrents):
     if tfilter is None:
         return 'all'
-    elif isinstance(tfilter, collections.abc.Sequence):
-        # tfilter is a sequence of torrent IDs
-        if len(tfilter) == 1:
-            # Just one specific torrent requested
-            return torrents[0]['name']
-        else:
-            # Multiple specific torrents requested
-            return ','.join(str(tid) for tid in tfilter)
     else:
-        # Should be a TorrentFilter instance
         return str(tfilter)
 
 
 from . import hooks
```

### Comparing `stig-0.8.3a0/stig/tui/views/filelist.py` & `stig-0.9.0a0/stig/tui/views/file_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 log = make_logger(__name__)
 
 import urwid
 import urwidtrees
 from collections import abc
 import builtins
 
-from .flist_columns import TUICOLUMNS
+from .file import TUICOLUMNS
 from . import (ItemWidgetBase, ListWidgetBase, stringify_torrent_filter)
 
 
-from ...views.filelist import (create_directory_data, create_directory_name)
+from ...views.file import (create_directory_data, create_directory_name)
 from urwidtrees.decoration import ArrowTree
 class FileTreeDecorator(ArrowTree):
     """urwidtrees decorator for TorrentFiles and TorrentFileTrees"""
 
     def __init__(self, torrents, keymap, table, ffilter):
         self._filewidgetcls = keymap.wrap(FileItemWidget, context='file')
         self._table = table
@@ -70,16 +70,15 @@
                             fcount += 1
                         else:
                             filtered_count += 1
                     elif v.nodetype == 'parent':
                         dirnode = create_directory_data(name=k, tree=v)
                         tree.append(create_tree(dirnode, v))
 
-                node_id = (node['tid'], node['id'])
-                self._filtered_counts[node_id] = filtered_count
+                self._filtered_counts[node['id']] = filtered_count
                 node['name'] = create_directory_name(node['name'], filtered_count)
                 return (node, tree or None)
 
         fcount = 0
         forest = []  # Multiple trees as siblings
         for t in sorted(torrents, key=lambda t: t['name'].lower()):
             filetree = t['files']
@@ -96,42 +95,41 @@
         # We can use the tree position as table ID
         self._table.register(pos)
         row = self._table.get_row(pos)
 
         # We use parent's decorate() method to give the name column a tree
         # structure.  But we also need the original update() method so we can
         # apply new data to the widget.  This is dirty but it works.
-        update_method = row.name.update
-        decowidget = super().decorate(pos, row.name, is_first=is_first)
-        decowidget.update = update_method
-        row.replace('name', decowidget)
+        if row.exists('name'):
+            update_method = row.name.update
+            decowidget = super().decorate(pos, row.name, is_first=is_first)
+            decowidget.update = update_method
+            row.replace('name', decowidget)
 
         # Wrap the whole row in a FileItemWidget with keymapping.  This also
         # applies all the other values besides the name (size, progress, etc).
         file_widget = self._filewidgetcls(data, row)
-        node_id = (data['tid'], data['id'])
-        self._widgets[node_id] = file_widget
+        self._widgets[data['id']] = file_widget
         return file_widget
 
     def update(self, torrents):
         widgets = self._widgets
         for t in torrents:
             tid = t['id']
 
             # Update file nodes
             for f in t['files'].files:
-                fid = f['id']
-                node_id = (tid, fid)
+                node_id = f['id']
+                # File might be filtered
                 if node_id in widgets:
                     widgets[node_id].update(f)
 
             # Update directory nodes
             for name,content in t['files'].directories:
-                fids = frozenset(f['id'] for f in content.files)
-                node_id = (tid, fids)
+                node_id = content.id
                 if node_id in widgets:
                     filtered_count = self._filtered_counts[node_id]
                     data = create_directory_data(name, tree=content,
                                                  filtered_count=filtered_count)
                     widgets[node_id].update(data)
 
     @property
@@ -145,25 +143,25 @@
     palette_unfocused = 'filelist'
     palette_focused   = 'filelist.focused'
     columns_focus_map = {}
     for col in TUICOLUMNS.values():
         columns_focus_map.update(col.style.focus_map)
 
     @property
-    def torrent_id(self):
-        return self._item['tid']
+    def id(self):
+        return self.data['id']
 
     @property
-    def file_id(self):
-        return self._item['id']
+    def torrent_id(self):
+        return self.data['tid']
 
     @property
     def nodetype(self):
         """'parent' or 'leaf'"""
-        return self._item.nodetype
+        return self.data.nodetype
 
 
 class FileListWidget(ListWidgetBase):
     tuicolumns      = TUICOLUMNS
     ListItemClass   = FileItemWidget
     keymap_context  = 'file'
     palette_name    = 'filelist'
@@ -173,16 +171,15 @@
         super().__init__(srvapi, keymap, columns=columns, title=title)
         self._tfilter = tfilter
         self._ffilter = ffilter
         self._initialized = False
         self._torrents = None
 
         self._poller = self._srvapi.create_poller(
-            self._srvapi.torrent.torrents, tfilter, keys=('files', 'name'),
-            autoconnect=False
+            self._srvapi.torrent.torrents, tfilter, keys=('files', 'name')
         )
         self._poller.on_response(self._handle_files)
 
     def _handle_files(self, response):
         if response is None or not response.torrents:
             self.clear()
         else:
@@ -254,18 +251,28 @@
 
     @property
     def focused_file_ids(self):
         """File IDs of the focused files in a tuple"""
         focused = self.focused_widget
         if focused is not None:
             # The focused widget in the list can be a file or a directory.  If
-            # it's a directory, the 'file_id' property returns the IDs of all
-            # the contained files recursively.
-            fid = focused.file_id
-            return tuple(fid) if isinstance(fid, (abc.Sequence, abc.Set)) else (fid,)
+            # it's a directory, the 'id' property returns the IDs of all the
+            # contained files recursively, otherwise it's just a single ID.  For
+            # consistency, we always return a sequence of IDs.
+            if focused.nodetype == 'leaf':
+                return (focused.id,)
+            else:
+                return focused.id
+
+    @property
+    def focused_torrent_id(self):
+        """Torrent ID of the currently focused file or `None`"""
+        focused_widget = self.focused_widget
+        if focused_widget is not None:
+            return focused_widget.torrent_id
 
 
     def all_children(self, pos):
         """Yield (position, widget) tuples of all sub-nodes (leaves and parents)"""
         ft = self._filetree
         lb = self._listbox
         def recurse(subpos):
```

### Comparing `stig-0.8.3a0/stig/tui/views/flist_columns.py` & `stig-0.9.0a0/stig/tui/views/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,83 +11,79 @@
 
 """Column classes that display information in torrent file lists"""
 
 import urwid
 
 from ..table import ColumnHeaderWidget
 from . import (Style, CellWidgetBase)
-from ...views.filelist import COLUMNS as _COLUMNS
+from ...views.file import COLUMNS as _COLUMNS
 
 
 TUICOLUMNS = {}
 
 
 from .common_columns import MarkedBase
 class Marked(MarkedBase):
     style = Style(prefix='filelist.marked', focusable=True, extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(), style.attrs('header'))
 
 TUICOLUMNS['marked'] = Marked
 
 
+from ...utils.string import normalize_unicode
 class Filename(_COLUMNS['name'], CellWidgetBase):
     width = ('weight', 100)
     style = Style(prefix='filelist.name', focusable=True,
                   extras=('header',), modes=('file', 'folder', 'filtered'))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['name'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        if isinstance(self.data['id'], int):
+        if self.data.nodetype == 'leaf':
             return 'file'
         else:
             return 'folder'
 
+    def get_tui_value(self):
+        return normalize_unicode(super().get_tui_value())
+
 TUICOLUMNS['name'] = Filename
 
 
 class Size(_COLUMNS['size'], CellWidgetBase):
     style = Style(prefix='filelist.size', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['size'].header),
                            style.attrs('header'))
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['size'].header['right']
-
 TUICOLUMNS['size'] = Size
 
 
 class Downloaded(_COLUMNS['downloaded'], CellWidgetBase):
     style = Style(prefix='filelist.downloaded', focusable=True,
                   extras=('header',), modes=('highlighted',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['downloaded'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if self.data['progress'] < 100 else None
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['downloaded'].header['right']
+        return 'highlighted' if self.data['%downloaded'] < 100 else None
 
 TUICOLUMNS['downloaded'] = Downloaded
 
 
-class Progress(_COLUMNS['progress'], CellWidgetBase):
-    style = Style(prefix='filelist.progress', focusable=True,
+class PercentDownloaded(_COLUMNS['%downloaded'], CellWidgetBase):
+    style = Style(prefix='filelist.%downloaded', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['progress'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['%downloaded'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value < 100 else ''
 
-TUICOLUMNS['progress'] = Progress
+TUICOLUMNS['%downloaded'] = PercentDownloaded
 
 
 class Priority(_COLUMNS['priority'], CellWidgetBase):
     style = Style(prefix='filelist.priority', focusable=True,
                   extras=('header',), modes=('off', 'low', 'high'))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['priority'].header),
                            style.attrs('header'))
```

### Comparing `stig-0.8.3a0/stig/tui/views/tlist_columns.py` & `stig-0.9.0a0/stig/tui/views/torrent.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,404 +5,372 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-"""Column classes that display information in torrent lists
-
-Adding a new cell type adds a new optional column to torrent lists.  To do
-this, write a new class that derives from CellWidgetBase and register it in
-the COLUMNS dictionary to make it available.
-"""
-
-from ...logging import make_logger
-log = make_logger(__name__)
-
 import urwid
 
 from ..table import ColumnHeaderWidget
 from . import (Style, CellWidgetBase)
-from ...views.torrentlist import COLUMNS as _COLUMNS
+from ...views.torrent import COLUMNS as _COLUMNS
 from ...client import ttypes
+from ...utils.string import normalize_unicode
 
 
 TUICOLUMNS = {}
 
 
 from .common_columns import MarkedBase
 class Marked(MarkedBase):
     style = Style(prefix='torrentlist.marked', focusable=True, extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(), style.attrs('header'))
 
 TUICOLUMNS['marked'] = Marked
 
 
-class Path(_COLUMNS['path'], CellWidgetBase):
-    width = 20
-    style = Style(prefix='torrentlist.path', focusable=True,
+class Id(_COLUMNS['id'], CellWidgetBase):
+    style = Style(prefix='torrentlist.id', focusable=True,
                   extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['path'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['id'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['path'] = Path
+TUICOLUMNS['id'] = Id
 
 
-class Connections(_COLUMNS['connections'], CellWidgetBase):
-    style = Style(prefix='torrentlist.connections', focusable=True,
-                  extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['connections'].header),
+class Name(_COLUMNS['name'], CellWidgetBase):
+    width = ('weight', 100)
+    style = Style(prefix='torrentlist.name', focusable=True, extras=('header',),
+                  modes=('idle.progress1', 'idle.progress2', 'idle.complete',
+                         'stopped.progress1', 'stopped.progress2', 'stopped.complete',
+                         'isolated.progress1', 'isolated.progress2', 'isolated.complete',
+                         'discovering.progress1', 'discovering.progress2', 'discovering.complete',
+                         'verifying.progress1', 'verifying.progress2', 'verifying.complete',
+                         'downloading.progress1', 'downloading.progress2', 'downloading.complete',
+                         'uploading.progress1', 'uploading.progress2', 'uploading.complete',
+                         'queued.progress1', 'queued.progress2', 'queued.complete',
+                         'connected.progress1', 'connected.progress2', 'connected.complete'))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['name'].header),
                            style.attrs('header'))
+    needed_keys = ('name', 'status', '%downloaded', '%verified', '%metadata',
+                   'rate-up', 'rate-down', 'peers-connected')
 
-    def get_mode(self):
-        return 'highlighted' if self.value > 0 else ''
-
-TUICOLUMNS['connections'] = Connections
+    def __init__(self, *args, **kwargs):
+        self.status = ('', 'idle', 0)
+        super().__init__(*args, **kwargs)
 
+    def update(self, torrent):
+        progress = torrent['%downloaded']
+        Status = type(torrent['status'])
+        if Status.STOPPED in torrent['status']:
+            mode = 'stopped'
+        elif Status.ISOLATED in torrent['status']:
+            mode = 'isolated'
+        elif Status.INIT in torrent['status']:
+            mode = 'discovering'
+            progress = torrent['%metadata']
+        elif Status.VERIFY in torrent['status']:
+            mode = 'verifying'
+            progress = torrent['%verified']
+        elif Status.DOWNLOAD in torrent['status']:
+            mode = 'downloading'
+        elif Status.UPLOAD in torrent['status']:
+            mode = 'uploading'
+        elif Status.QUEUED in torrent['status']:
+            mode = 'queued'
+        elif Status.CONNECTED in torrent['status']:
+            mode = 'connected'
+        else:
+            mode = 'idle'
+        new_status = (torrent['name'], mode, progress)
+        if new_status != self.status:
+            self.status = new_status
+            self._invalidate()
 
-class Seeds(_COLUMNS['seeds'], CellWidgetBase):
-    style = Style(prefix='torrentlist.seeds', focusable=True,
-                  extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['seeds'].header),
-                           style.attrs('header'))
+    def render(self, size, focus=False):
+        (maxcol,) = size
+        name, mode, progress = self.status
+        name = normalize_unicode(name)
+        name = name[:maxcol].ljust(maxcol, ' ')  # Expand/Shrink name to full width
+        if progress == 100:
+            attrs = self.style.attrs(mode+'.complete', focused=focus)
+            self.text.set_text((attrs, name))
+        else:
+            completed_col = int(maxcol * progress / 100)  # Width of first part of progress bar
+            name1 = name[:completed_col]
+            name2 = name[completed_col:]
+            attrs1 = self.style.attrs(mode+'.progress1', focused=focus)
+            attrs2 = self.style.attrs(mode+'.progress2', focused=focus)
+            self.text.set_text([(attrs1, name1),
+                                (attrs2, name2)])
+        return super().render(size, focus)
 
     def get_mode(self):
-        return 'highlighted' if self.value < 5 else ''
+        return self.status[1]
 
-TUICOLUMNS['seeds'] = Seeds
+TUICOLUMNS['name'] = Name
 
 
-class Progress(_COLUMNS['progress'], CellWidgetBase):
-    style = Style(prefix='torrentlist.progress', focusable=True,
-                  extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['progress'].header),
+class Path(_COLUMNS['path'], CellWidgetBase):
+    width = 20
+    style = Style(prefix='torrentlist.path', focusable=True,
+                  extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['path'].header),
                            style.attrs('header'))
 
-    def get_mode(self):
-        return 'highlighted' if self.value < 100 else ''
+TUICOLUMNS['path'] = Path
 
-TUICOLUMNS['progress'] = Progress
 
+class Status(_COLUMNS['status'], CellWidgetBase):
+    style = Style(prefix='torrentlist.status', focusable=True,
+                  extras=('header',),
+                  modes=('idle', 'downloading', 'uploading', 'connected', 'seeding',
+                         'stopped', 'queued', 'isolated', 'verifying', 'discovering'))
 
-class PercentAvailable(_COLUMNS['%available'], CellWidgetBase):
-    style = Style(prefix='torrentlist.%available', focusable=True,
-                  extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['%available'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['status'].header),
                            style.attrs('header'))
 
+    MODE_MAP = {
+        ttypes.Status.IDLE      : 'idle',
+        ttypes.Status.DOWNLOAD  : 'downloading',
+        ttypes.Status.UPLOAD    : 'uploading',
+        ttypes.Status.CONNECTED : 'connected',
+        ttypes.Status.SEED      : 'seeding',
+        ttypes.Status.STOPPED   : 'stopped',
+        ttypes.Status.QUEUED    : 'queued',
+        ttypes.Status.ISOLATED  : 'isolated',
+        ttypes.Status.VERIFY    : 'verifying',
+        ttypes.Status.INIT      : 'discovering',
+    }
     def get_mode(self):
-        return 'highlighted' if self.value < 100 else ''
+        return self.MODE_MAP[self.value]
 
-TUICOLUMNS['%available'] = PercentAvailable
+TUICOLUMNS['status'] = Status
 
 
-class Ratio(_COLUMNS['ratio'], CellWidgetBase):
-    style = Style(prefix='torrentlist.ratio', focusable=True,
-                  extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['ratio'].header),
+class Error(_COLUMNS['error'], CellWidgetBase):
+    style = Style(prefix='torrentlist.error', focusable=True,
+                  extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['error'].header),
                            style.attrs('header'))
 
-    def get_mode(self):
-        if 0 <= self.value < 1:
-            return 'highlighted'
-
-TUICOLUMNS['ratio'] = Ratio
+TUICOLUMNS['error'] = Error
 
 
-class Size(_COLUMNS['size'], CellWidgetBase):
-    style = Style(prefix='torrentlist.size', focusable=True,
-                  extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['size'].header),
+class Uploaded(_COLUMNS['uploaded'], CellWidgetBase):
+    style = Style(prefix='torrentlist.uploaded', focusable=True,
+                  extras=('header',), modes=('highlighted',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['uploaded'].header),
                            style.attrs('header'))
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['size'].header['right']
+    def get_mode(self):
+        if self.data['size-uploaded'] < self.data['size-downloaded']:
+            return 'highlighted'
 
-TUICOLUMNS['size'] = Size
+TUICOLUMNS['uploaded'] = Uploaded
 
 
 class Downloaded(_COLUMNS['downloaded'], CellWidgetBase):
     style = Style(prefix='torrentlist.downloaded', focusable=True,
                   extras=('header',), modes=('highlighted',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['downloaded'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         t = self.data
         if t['%downloaded'] < 100 and 0 < t['size-downloaded'] < t['size-final']:
             return 'highlighted'
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['downloaded'].header['right']
-
 TUICOLUMNS['downloaded'] = Downloaded
 
 
-class Uploaded(_COLUMNS['uploaded'], CellWidgetBase):
-    style = Style(prefix='torrentlist.uploaded', focusable=True,
+class PercentDownloaded(_COLUMNS['%downloaded'], CellWidgetBase):
+    style = Style(prefix='torrentlist.%downloaded', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['uploaded'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['%downloaded'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        if self.data['size-uploaded'] < self.data['size-downloaded']:
-            return 'highlighted'
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['uploaded'].header['right']
+        return 'highlighted' if self.value < 100 else ''
 
-TUICOLUMNS['uploaded'] = Uploaded
+TUICOLUMNS['%downloaded'] = PercentDownloaded
 
 
-class BytesAvailable(_COLUMNS['available'], CellWidgetBase):
+class Available(_COLUMNS['available'], CellWidgetBase):
     style = Style(prefix='torrentlist.available', focusable=True,
                   extras=('header',), modes=('highlighted',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['available'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         if self.value < self.data['size-final']:
             return 'highlighted'
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['available'].header['right']
+TUICOLUMNS['available'] = Available
 
-TUICOLUMNS['available'] = BytesAvailable
 
-
-class RateDown(_COLUMNS['rate-down'], CellWidgetBase):
-    style = Style(prefix='torrentlist.rate-down', focusable=True,
+class PercentAvailable(_COLUMNS['%available'], CellWidgetBase):
+    style = Style(prefix='torrentlist.%available', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-down'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['%available'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if self.value > 0 else ''
+        return 'highlighted' if self.value < 100 else ''
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-down'].header['right']
+TUICOLUMNS['%available'] = PercentAvailable
 
-TUICOLUMNS['rate-down'] = RateDown
 
+class Size(_COLUMNS['size'], CellWidgetBase):
+    style = Style(prefix='torrentlist.size', focusable=True,
+                  extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['size'].header),
+                           style.attrs('header'))
+
+TUICOLUMNS['size'] = Size
 
-class RateUp(_COLUMNS['rate-up'], CellWidgetBase):
-    style = Style(prefix='torrentlist.rate-up', focusable=True,
+
+class Peers(_COLUMNS['peers'], CellWidgetBase):
+    style = Style(prefix='torrentlist.peers', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-up'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['peers'].header),
                            style.attrs('header'))
 
     def get_mode(self):
         return 'highlighted' if self.value > 0 else ''
 
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-up'].header['right']
-
-TUICOLUMNS['rate-up'] = RateUp
-
+TUICOLUMNS['peers'] = Peers
 
 
-class RateLimitDown(_COLUMNS['rate-limit-down'], CellWidgetBase):
-    style = Style(prefix='torrentlist.rate-limit-down', focusable=True,
+class Seeds(_COLUMNS['seeds'], CellWidgetBase):
+    style = Style(prefix='torrentlist.seeds', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-limit-down'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['seeds'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if self.value < float('inf') else ''
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-limit-down'].header['right']
+        return 'highlighted' if self.value < 5 else ''
 
-TUICOLUMNS['rate-limit-down'] = RateLimitDown
+TUICOLUMNS['seeds'] = Seeds
 
 
-class RateLimitUp(_COLUMNS['rate-limit-up'], CellWidgetBase):
-    style = Style(prefix='torrentlist.rate-limit-up', focusable=True,
+class Ratio(_COLUMNS['ratio'], CellWidgetBase):
+    style = Style(prefix='torrentlist.ratio', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-limit-up'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['ratio'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if self.value < float('inf') else ''
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header.original_widget.right = _COLUMNS['rate-limit-up'].header['right']
+        if 0 <= self.value < 1:
+            return 'highlighted'
 
-TUICOLUMNS['rate-limit-up'] = RateLimitUp
+TUICOLUMNS['ratio'] = Ratio
 
 
-class EtaComplete(_COLUMNS['eta'], CellWidgetBase):
-    style = Style(prefix='torrentlist.eta', focusable=True,
+class RateUp(_COLUMNS['rate-up'], CellWidgetBase):
+    style = Style(prefix='torrentlist.rate-up', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['eta'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-up'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if bool(self.value) else ''
+        return 'highlighted' if self.value > 0 else ''
 
-TUICOLUMNS['eta'] = EtaComplete
+TUICOLUMNS['rate-up'] = RateUp
 
 
-class TimeCreated(_COLUMNS['time-created'], CellWidgetBase):
-    style = Style(prefix='torrentlist.created', focusable=True, extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['time-created'].header),
+class RateDown(_COLUMNS['rate-down'], CellWidgetBase):
+    style = Style(prefix='torrentlist.rate-down', focusable=True,
+                  extras=('header',), modes=('highlighted',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['rate-down'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['time-created'] = TimeCreated
+    def get_mode(self):
+        return 'highlighted' if self.value > 0 else ''
 
-class TimeAdded(_COLUMNS['time-added'], CellWidgetBase):
-    style = Style(prefix='torrentlist.added', focusable=True, extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['time-added'].header),
-                           style.attrs('header'))
+TUICOLUMNS['rate-down'] = RateDown
 
-TUICOLUMNS['time-added'] = TimeAdded
 
-class TimeStarted(_COLUMNS['time-started'], CellWidgetBase):
-    style = Style(prefix='torrentlist.started', focusable=True, extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['time-started'].header),
+class LimitRateUp(_COLUMNS['limit-rate-up'], CellWidgetBase):
+    style = Style(prefix='torrentlist.limit-rate-up', focusable=True,
+                  extras=('header',), modes=('highlighted',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['limit-rate-up'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['time-started'] = TimeStarted
+    def get_mode(self):
+        return 'highlighted' if self.value < float('inf') else ''
 
-class TimeActive(_COLUMNS['time-activity'], CellWidgetBase):
-    style = Style(prefix='torrentlist.activity', focusable=True, extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['time-activity'].header),
-                           style.attrs('header'))
+TUICOLUMNS['limit-rate-up'] = LimitRateUp
 
-TUICOLUMNS['time-activity'] = TimeActive
 
-class TimeCompleted(_COLUMNS['time-completed'], CellWidgetBase):
-    style = Style(prefix='torrentlist.completed', focusable=True,
+class LimitRateDown(_COLUMNS['limit-rate-down'], CellWidgetBase):
+    style = Style(prefix='torrentlist.limit-rate-down', focusable=True,
                   extras=('header',), modes=('highlighted',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['time-completed'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['limit-rate-down'].header),
                            style.attrs('header'))
 
     def get_mode(self):
-        return 'highlighted' if self.value.in_future else ''
+        return 'highlighted' if self.value < float('inf') else ''
 
-TUICOLUMNS['time-completed'] = TimeCompleted
+TUICOLUMNS['limit-rate-down'] = LimitRateDown
 
 
 class Tracker(_COLUMNS['tracker'], CellWidgetBase):
     style = Style(prefix='torrentlist.tracker', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['tracker'].header),
                            style.attrs('header'))
 
 TUICOLUMNS['tracker'] = Tracker
 
 
-class Error(_COLUMNS['error'], CellWidgetBase):
-    style = Style(prefix='torrentlist.error', focusable=True,
-                  extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['error'].header),
+class Eta(_COLUMNS['eta'], CellWidgetBase):
+    style = Style(prefix='torrentlist.eta', focusable=True,
+                  extras=('header',), modes=('highlighted',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['eta'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['error'] = Error
+    def get_mode(self):
+        return 'highlighted' if bool(self.value) else ''
 
+TUICOLUMNS['eta'] = Eta
 
-class Status(_COLUMNS['status'], CellWidgetBase):
-    style = Style(prefix='torrentlist.status', focusable=True,
-                  extras=('header',),
-                  modes=('idle', 'downloading', 'uploading', 'connected', 'seeding',
-                         'stopped', 'queued', 'isolated', 'verifying', 'discovering'))
 
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['status'].header),
+class Created(_COLUMNS['created'], CellWidgetBase):
+    style = Style(prefix='torrentlist.created', focusable=True, extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['created'].header),
                            style.attrs('header'))
 
-    MODE_MAP = {
-        ttypes.Status.IDLE      : 'idle',
-        ttypes.Status.DOWNLOAD  : 'downloading',
-        ttypes.Status.UPLOAD    : 'uploading',
-        ttypes.Status.CONNECTED : 'connected',
-        ttypes.Status.SEED      : 'seeding',
-        ttypes.Status.STOPPED   : 'stopped',
-        ttypes.Status.QUEUED    : 'queued',
-        ttypes.Status.ISOLATED  : 'isolated',
-        ttypes.Status.VERIFY    : 'verifying',
-        ttypes.Status.INIT      : 'discovering',
-    }
-    def get_mode(self):
-        return self.MODE_MAP[self.value]
+TUICOLUMNS['created'] = Created
 
-TUICOLUMNS['status'] = Status
+class Added(_COLUMNS['added'], CellWidgetBase):
+    style = Style(prefix='torrentlist.added', focusable=True, extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['added'].header),
+                           style.attrs('header'))
 
+TUICOLUMNS['added'] = Added
 
-class TorrentName(_COLUMNS['name'], CellWidgetBase):
-    width = ('weight', 100)
-    style = Style(prefix='torrentlist.name', focusable=True, extras=('header',),
-                  modes=('idle.progress1', 'idle.progress2', 'idle.complete',
-                         'stopped.progress1', 'stopped.progress2', 'stopped.complete',
-                         'isolated.progress1', 'isolated.progress2', 'isolated.complete',
-                         'discovering.progress1', 'discovering.progress2', 'discovering.complete',
-                         'verifying.progress1', 'verifying.progress2', 'verifying.complete',
-                         'downloading.progress1', 'downloading.progress2', 'downloading.complete',
-                         'uploading.progress1', 'uploading.progress2', 'uploading.complete',
-                         'queued.progress1', 'queued.progress2', 'queued.complete',
-                         'connected.progress1', 'connected.progress2', 'connected.complete'))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['name'].header),
+class Started(_COLUMNS['started'], CellWidgetBase):
+    style = Style(prefix='torrentlist.started', focusable=True, extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['started'].header),
                            style.attrs('header'))
-    needed_keys = ('name', 'status', '%downloaded', '%verified', '%metadata',
-                   'rate-up', 'rate-down', 'peers-connected')
 
-    def __init__(self, *args, **kwargs):
-        self.status = ('', 'idle', 0)
-        super().__init__(*args, **kwargs)
+TUICOLUMNS['started'] = Started
 
-    def update(self, torrent):
-        progress = torrent['%downloaded']
-        Status = type(torrent['status'])
-        if Status.STOPPED in torrent['status']:
-            mode = 'stopped'
-        elif Status.ISOLATED in torrent['status']:
-            mode = 'isolated'
-        elif Status.INIT in torrent['status']:
-            mode = 'discovering'
-            progress = torrent['%metadata']
-        elif Status.VERIFY in torrent['status']:
-            mode = 'verifying'
-            progress = torrent['%verified']
-        elif Status.DOWNLOAD in torrent['status']:
-            mode = 'downloading'
-        elif Status.UPLOAD in torrent['status']:
-            mode = 'uploading'
-        elif Status.QUEUED in torrent['status']:
-            mode = 'queued'
-        elif Status.CONNECTED in torrent['status']:
-            mode = 'connected'
-        else:
-            mode = 'idle'
-        new_status = (torrent['name'], mode, progress)
-        if new_status != self.status:
-            self.status = new_status
-            self._invalidate()
+class Active(_COLUMNS['activity'], CellWidgetBase):
+    style = Style(prefix='torrentlist.activity', focusable=True, extras=('header',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['activity'].header),
+                           style.attrs('header'))
 
-    def render(self, size, focus=False):
-        (maxcol,) = size
-        name, mode, progress = self.status
-        name = name[:maxcol].ljust(maxcol, ' ')  # Expand/Shrink name to full width
-        if progress == 100:
-            attrs = self.style.attrs(mode+'.complete', focused=focus)
-            self.text.set_text((attrs, name))
-        else:
-            completed_col = int(maxcol * progress / 100)  # Width of first part of progress bar
-            name1 = name[:completed_col]
-            name2 = name[completed_col:]
-            attrs1 = self.style.attrs(mode+'.progress1', focused=focus)
-            attrs2 = self.style.attrs(mode+'.progress2', focused=focus)
-            self.text.set_text([(attrs1, name1),
-                                (attrs2, name2)])
-        return super().render(size, focus)
+TUICOLUMNS['activity'] = Active
+
+class Completed(_COLUMNS['completed'], CellWidgetBase):
+    style = Style(prefix='torrentlist.completed', focusable=True,
+                  extras=('header',), modes=('highlighted',))
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['completed'].header),
+                           style.attrs('header'))
 
     def get_mode(self):
-        return self.status[1]
+        return 'highlighted' if self.value.in_future else ''
 
-TUICOLUMNS['name'] = TorrentName
+TUICOLUMNS['completed'] = Completed
```

### Comparing `stig-0.8.3a0/stig/tui/views/torrentlist.py` & `stig-0.9.0a0/stig/tui/views/torrent_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
-import urwid
-
-from ..scroll import ScrollBar
-from .tlist_columns import TUICOLUMNS
+from .torrent import TUICOLUMNS
 from . import (ItemWidgetBase, ListWidgetBase, stringify_torrent_filter)
 
 
 class TorrentItemWidget(ItemWidgetBase):
     palette_unfocused = 'torrentlist'
     palette_focused   = 'torrentlist.focused'
     columns_focus_map = {}
     for col in TUICOLUMNS.values():
         columns_focus_map.update(col.style.focus_map)
 
+    @property
+    def id(self):
+        return self.data['id']
+
+    @property
+    def torrent_id(self):
+        return self.data['id']
+
 
 class TorrentListWidget(ListWidgetBase):
     tuicolumns      = TUICOLUMNS
     ListItemClass   = TorrentItemWidget
     keymap_context  = 'torrent'
     palette_name    = 'torrentlist'
     focusable_items = True
@@ -37,25 +42,25 @@
     def __init__(self, srvapi, keymap, tfilter=None, sort=None, columns=None, title=None):
         super().__init__(srvapi, keymap, columns=columns, sort=sort, title=title)
         self._tfilter = tfilter
         self._register_request()
 
     @property
     def id(self):
-        """Hashable object that is unique among all torrent lists"""
+        """Hashable that is unique among all torrent lists"""
         return id(self)
 
     def _register_request(self):
         # Get keys needed for sort order, tfilter and columns
         keys = ['name']
         if self._sort is not None:
             keys.extend(self._sort.needed_keys)
         if hasattr(self._tfilter, 'needed_keys'):
             keys.extend(self._tfilter.needed_keys)
-        for colname in self._columns:
+        for colname in self.columns:
             keys.extend(self.tuicolumns[colname].needed_keys)
 
         # Register new request in request pool
         log.debug('Registering keys for %r: %s', self, keys)
         self._srvapi.treqpool.register(self.id,
                                        self._handle_torrents,
                                        keys=keys, tfilter=self._tfilter)
@@ -69,27 +74,34 @@
     #     log.debug('Rendered torrent list in %.3fms', (time.time()-start)*1000)
     #     return canvas
 
     def _handle_torrents(self, torrents):
         # Auto-generate title from our filters if not set
         if self._title_name is None:
             self._title_name = stringify_torrent_filter(self._tfilter, torrents)
-        self._items = {t['id']:t for t in torrents}
+        self._data_dict = {t['id']:t for t in torrents}
         self._invalidate()
 
     def clear(self):
         for w in self._listbox.body:
-            w.item.clearcache()
+            w.data.clearcache()
         super().clear()
 
     def refresh(self):
         self._srvapi.treqpool.poll()
 
     @property
     def sort(self):
         return self._sort
 
     @sort.setter
     def sort(self, sort):
         self._srvapi.treqpool.remove(self.id)
         ListWidgetBase.sort.fset(self, sort)
         self._register_request()
+
+    @property
+    def focused_torrent_id(self):
+        """Torrent ID of the currently focused torrent or `None`"""
+        focused_widget = self._listbox.focus
+        if focused_widget is not None:
+            return focused_widget.torrent_id
```

### Comparing `stig-0.8.3a0/stig/tui/views/trklist_columns.py` & `stig-0.9.0a0/stig/tui/views/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 """Column classes that display information in peer lists"""
 
 import urwid
 
 from ..table import ColumnHeaderWidget
 from . import (Style, CellWidgetBase)
-from ...views.trackerlist import COLUMNS as _COLUMNS
+from ...views.tracker import COLUMNS as _COLUMNS
 
 
 TUICOLUMNS = {}
 
-class TorrentName(_COLUMNS['torrent'], CellWidgetBase):
+class Torrent(_COLUMNS['torrent'], CellWidgetBase):
     width = ('weight', 50)
     style = Style(prefix='trackerlist.torrent', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['torrent'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['torrent'] = TorrentName
+TUICOLUMNS['torrent'] = Torrent
 
 
 class Tier(_COLUMNS['tier'], CellWidgetBase):
     style = Style(prefix='trackerlist.tier', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['tier'].header),
                            style.attrs('header'))
@@ -65,21 +65,21 @@
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['url-scrape'].header),
                            style.attrs('header'))
 
 TUICOLUMNS['url-scrape'] = ScrapeURL
 
 
-class State(_COLUMNS['state'], CellWidgetBase):
-    style = Style(prefix='trackerlist.state', focusable=True,
+class Status(_COLUMNS['status'], CellWidgetBase):
+    style = Style(prefix='trackerlist.status', focusable=True,
                   extras=('header',))
-    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['state'].header),
+    header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['status'].header),
                            style.attrs('header'))
 
-TUICOLUMNS['state'] = State
+TUICOLUMNS['status'] = Status
 
 
 class Error(_COLUMNS['error'], CellWidgetBase):
     width = ('weight', 100)
     style = Style(prefix='trackerlist.error', focusable=True,
                   extras=('header',))
     header = urwid.AttrMap(ColumnHeaderWidget(**_COLUMNS['error'].header),
```

### Comparing `stig-0.8.3a0/stig/tui/views/peerlist.py` & `stig-0.9.0a0/stig/tui/views/peer_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-import urwid
-
-from ..scroll import ScrollBar
-from .plist_columns import TUICOLUMNS
+from .peer import TUICOLUMNS
 from . import (ItemWidgetBase, ListWidgetBase, stringify_torrent_filter)
 
 
 class PeerItemWidget(ItemWidgetBase):
     palette_unfocused = 'peerlist'
 
+    @property
+    def id(self):
+        return self.data['id']
+
+    @property
+    def torrent_id(self):
+        return self.data['tid']
+
 
 class PeerListWidget(ListWidgetBase):
     tuicolumns      = TUICOLUMNS
     ListItemClass   = PeerItemWidget
     keymap_context  = 'peer'
     palette_name    = 'peerlist'
     focusable_items = False
@@ -38,16 +43,15 @@
                 yield from pfilter.apply(peers)
         else:
             def filter_peers(peers):
                 yield from peers
         self._maybe_filter_peers = filter_peers
 
         self._poller = self._srvapi.create_poller(
-            self._srvapi.torrent.torrents, tfilter, keys=('peers', 'name', 'id'),
-            autoconnect=False
+            self._srvapi.torrent.torrents, tfilter, keys=('peers', 'name', 'id')
         )
         self._poller.on_response(self._handle_peers)
 
     def _handle_peers(self, response):
         if response is None or not response.torrents:
             self.clear()
         else:
@@ -57,17 +61,22 @@
                 if self._pfilter:
                     self._title_name += ' %s' % self._pfilter
 
             # Create list items our base widget can handle
             def peers_combined(torrents):
                 for t in torrents:
                     yield from self._maybe_filter_peers(t['peers'])
-            self._items = {p['id']:p for p in peers_combined(response.torrents)}
+            self._data_dict = {p['id']:p for p in peers_combined(response.torrents)}
         self._invalidate()
 
+    def clear(self):
+        for w in self._listbox.body:
+            w.data.clearcache()
+        super().clear()
+
     def refresh(self):
         self._poller.poll()
 
     @property
     def sort(self):
         return self._sort
```

### Comparing `stig-0.8.3a0/stig/tui/views/common_columns.py` & `stig-0.9.0a0/stig/tui/views/common_columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 #
 # This program is distributed in the hope that it will be useful
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
-import urwid
-
-from ..table import ColumnHeaderWidget
-from . import (Style, CellWidgetBase)
-from ...views.torrentlist import COLUMNS as _COLUMNS
+from . import CellWidgetBase
+from ...views.torrent import COLUMNS as _COLUMNS
 
 TUICOLUMNS = {}
 
 class MarkedBase(_COLUMNS['marked'], CellWidgetBase):
     width = 1
     needed_keys = ()
     _marked_char = '#'
```

### Comparing `stig-0.8.3a0/stig/tui/theme.py` & `stig-0.9.0a0/stig/tui/theme.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/tui/logger.py` & `stig-0.9.0a0/stig/tui/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
     @property
     def height(self):
         return self._height
 
     @height.setter
     def height(self, rows):
-        self._height = rows
+        self._height = int(rows)
         self._invalidate_rows()
         self._invalidate()
 
     def selectable(self):
         return False
```

### Comparing `stig-0.8.3a0/stig/tui/table.py` & `stig-0.9.0a0/stig/tui/table.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/commands/base/tracker.py` & `stig-0.9.0a0/stig/commands/base/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     aliases = ('trkls', 'lstrk')
     provides = set()
     category = 'tracker'
     description = 'List tracker(s) of torrent(s)'
     usage = ('trackerlist [<OPTIONS>]',
              'trackerlist [<OPTIONS>] <TORRENT FILTER>',
              'trackerlist [<OPTIONS>] <TORRENT FILTER> <TRACKER FILTER>')
-    examples = ()  # TODO
+    examples = ("trackerlist 'name~debian'",
+                "trackerlist tracker=my.tracker.local error")
     argspecs = (
         make_X_FILTER_spec('TORRENT', or_focused=True, nargs='?'),
         make_X_FILTER_spec('TRACKER', or_focused=True, nargs='?'),
 
         { 'names': ('--sort', '-s'),
           'default_description': "current value of 'sort.trackers' setting",
           'description': ('Comma-separated list of sort orders '
@@ -44,28 +45,28 @@
         { 'names': ('--columns', '-c'),
           'default_description': "current value of 'columns.trackers' setting",
           'description': ('Comma-separated list of column names '
                           "(see COLUMNS section)") },
     )
     cfg = ExpectedResource
 
-    from ...views.trackerlist import COLUMNS
-    from ...client.sorters.trksorter import TorrentTrackerSorter
+    from ...views.tracker import COLUMNS
+    from ...client.sorters.tracker import TorrentTrackerSorter
     more_sections = {
         'COLUMNS': make_COLUMNS_doc(COLUMNS, '--columns', 'columns.trackers', append=(
             '',
             'The "torrent" column is added automatically if multiple '
             'torrents could be listed potentially.')),
         'SORT ORDERS': make_SORT_ORDERS_doc(TorrentTrackerSorter, '--sort', 'sort.trackers'),
         'SCRIPTING': make_SCRIPTING_doc(name),
     }
 
     async def run(self, TORRENT_FILTER, TRACKER_FILTER, sort, columns):
-        columns = self.cfg['columns.trackers'].value if columns is None else columns
-        sort = self.cfg['sort.trackers'].value if sort is None else sort
+        columns = self.cfg['columns.trackers'] if columns is None else columns
+        sort = self.cfg['sort.trackers'] if sort is None else sort
         try:
             torfilter = self.select_torrents(TORRENT_FILTER,
                                              allow_no_filter=True,
                                              discover_torrent=True)
             trkfilter = self.get_tracker_filter(TRACKER_FILTER)
             sort      = self.get_tracker_sorter(sort)
             columns   = self.get_tracker_columns(columns)
@@ -73,22 +74,22 @@
             log.error(e)
             return False
 
         # Unless we're listing trackers of exactly one torrent, specified by its
         # ID, automatically add the 'torrent' column.
         if 'torrent' not in columns and \
            (not isinstance(torfilter, abc.Sequence) or len(torfilter) != 1):
-            columns.append('torrent')
+            columns += ('torrent',)
 
         log.debug('Listing %s trackers of %s torrents', trkfilter, torfilter)
 
-        if asyncio.iscoroutinefunction(self.make_trklist):
-            return await self.make_trklist(torfilter, trkfilter, sort, columns)
+        if asyncio.iscoroutinefunction(self.make_tracker_list):
+            return await self.make_tracker_list(torfilter, trkfilter, sort, columns)
         else:
-            return self.make_trklist(torfilter, trkfilter, sort, columns)
+            return self.make_tracker_list(torfilter, trkfilter, sort, columns)
 
 
 class AnnounceCmdbase(metaclass=InitCommand):
     name = 'announce'
     aliases = ('an',)
     provides = set()
     category = 'tracker'
```

### Comparing `stig-0.8.3a0/stig/commands/base/peer.py` & `stig-0.9.0a0/stig/commands/base/peer.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 
         { 'names': ('--columns', '-c'),
           'default_description': "current value of 'columns.peers' setting",
           'description': ('Comma-separated list of column names '
                           "(see COLUMNS section)") },
     )
 
-    from ...views.peerlist import COLUMNS
-    from ...client.sorters.psorter import TorrentPeerSorter
+    from ...views.peer import COLUMNS
+    from ...client.sorters.peer import TorrentPeerSorter
     more_sections = {
         'COLUMNS': make_COLUMNS_doc(COLUMNS, '--columns', 'columns.peers', append=(
             '',
             'The "torrent" column is added automatically if multiple '
             'torrents could be listed potentially.')),
         'SORT ORDERS': make_SORT_ORDERS_doc(TorrentPeerSorter, '--sort', 'sort.peers'),
         'SCRIPTING': make_SCRIPTING_doc(name),
     }
 
     cfg = ExpectedResource
 
     async def run(self, TORRENT_FILTER, PEER_FILTER, sort, columns):
-        columns = self.cfg['columns.peers'].value if columns is None else columns
-        sort = self.cfg['sort.peers'].value if sort is None else sort
+        columns = self.cfg['columns.peers'] if columns is None else columns
+        sort = self.cfg['sort.peers'] if sort is None else sort
         try:
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=True,
                                            discover_torrent=True)
             pfilter = self.get_peer_filter(PEER_FILTER)
             sort    = self.get_peer_sorter(sort)
             columns = self.get_peer_columns(columns)
@@ -76,15 +76,15 @@
             log.error(e)
             return False
 
         # Unless we're listing peers of exactly one torrent, specified by its
         # ID, automatically add the 'torrent' column.
         if 'torrent' not in columns and \
            (not isinstance(tfilter, abc.Sequence) or len(tfilter) != 1):
-            columns.append('torrent')
+            columns += ('torrent',)
 
         log.debug('Listing %s peers of %s torrents', pfilter, tfilter)
 
-        if asyncio.iscoroutinefunction(self.make_plist):
-            return await self.make_plist(tfilter, pfilter, sort, columns)
+        if asyncio.iscoroutinefunction(self.make_peer_list):
+            return await self.make_peer_list(tfilter, pfilter, sort, columns)
         else:
-            return self.make_plist(tfilter, pfilter, sort, columns)
+            return self.make_peer_list(tfilter, pfilter, sort, columns)
```

### Comparing `stig-0.8.3a0/stig/commands/base/_mixin.py` & `stig-0.9.0a0/stig/commands/base/_mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,155 +7,168 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """Mixin classes that are common between TUI and CLI commands"""
 
-from ...logging import make_logger
-log = make_logger(__name__)
-
-
 from .. import utils
 
 
-def _get_columns(columns, setting, interface, COLSPECS, cfg):
-    # Resolve aliases and complain about invalid values
-    columns = cfg[setting].convert(columns)
-    cfg[setting].validate(columns)
-
-    # Make sure `columns` is a list
-    columns = utils.listify_args(columns)
-
-    # Remove columns that aren't supported by the active interface
-    for col in tuple(columns):
-        if interface is not None and interface not in COLUMNS[col].interfaces:
-            log.debug('Removing column %r because it does not support %r', col, interface)
-            columns.remove(col)
-    return columns
-
-
-class get_torrent():
-    async def get_torrent(self, tfilter, keys=()):
-        """Get a single torrent that matches TorrentFilter `tfilter`
+class get_single_torrent():
+    async def get_single_torrent(self, tfilter, keys=()):
+        """
+        Get a single torrent that matches TorrentFilter `tfilter`
 
         If there are multple matches, they are sorted by name and the first
         match is returned.
 
         Return None if no match is found.
         """
-        request = self.srvapi.torrent.torrents(tfilter, keys=keys)
+        request = self.srvapi.torrent.torrents(tfilter, keys=tuple(keys) + ('name',))
         response = await self.make_request(request, polling_frenzy=False, quiet=True)
         if response.success:
             from ...client import TorrentSorter
             torrents = TorrentSorter(('name',)).apply(response.torrents)
             return torrents[0]
 
 class get_torrent_sorter():
     def get_torrent_sorter(self, args):
-        """Return TorrentSorter instance or None
+        """
+        Return TorrentSorter instance or None
 
         If `args` evaluates to True, it is passed to TorrentSorter and the
         result is returned.
 
         If `args` evaluates to False, None is returned.
         """
         if args:
             from ...client import TorrentSorter
-            return TorrentSorter(utils.listify_args(args))
+            return TorrentSorter(self.cfg.validate('sort.torrents', args))
 
 class get_torrent_columns():
-    def get_torrent_columns(self, columns, interface=None):
-        """Check if each item in iterable `columns` is a valid torrent list column name
-
-        If `interface` is not None, also remove all columns that don't have
-        `interface` in their `interfaces` attribute.
+    def get_torrent_columns(self, columns):
+        """
+        Check if each item in iterable `columns` is a valid torrent list column name
 
         Raise ValueError or return a new list of `columns`.
         """
-        from ...views.torrentlist import COLUMNS
-        return _get_columns(columns, 'columns.torrents', interface, COLUMNS, self.cfg)
+        return self.cfg.validate('columns.torrents', columns)
 
 
 
 class get_file_columns():
-    def get_file_columns(self, columns, interface=None):
-        """Check if each item in iterable `columns` is a valid file list column name
+    def get_file_columns(self, columns):
+        """
+        Check if each item in iterable `columns` is a valid file list column name
 
         Raise ValueError or return a new list of `columns`.
         """
-        from ...views.filelist import COLUMNS
-        return _get_columns(columns, 'columns.files', interface, COLUMNS, self.cfg)
+        return self.cfg.validate('columns.files', columns)
 
 
 
 class get_peer_sorter():
     def get_peer_sorter(self, args):
-        """Return TorrentPeerSorter instance or None
+        """
+        Return TorrentPeerSorter instance or None
 
         If `args` evaluates to True, it is passed to TorrentPeerSorter and the
         result is returned.
 
         If `args` evaluates to False, None is returned.
         """
         if args:
             from ...client import TorrentPeerSorter
-            return TorrentPeerSorter(utils.listify_args(args))
+            return TorrentPeerSorter(self.cfg.validate('sort.peers', args))
 
 class get_peer_filter():
     def get_peer_filter(self, FILTER):
-        """Return TorrentPeerFilter instance or None
+        """
+        Return TorrentPeerFilter instance or None
 
-        If `FILTER` evaluates to True, it is passed to TorrentPeerFilter and
-        the resulting object is returned.
+        If `FILTER` evaluates to True, it is passed to TorrentPeerFilter and the
+        resulting object is returned.
 
         If `FILTER` evaluates to False, None is returned.
         """
         if FILTER:
             from ...client import TorrentPeerFilter
             return TorrentPeerFilter(FILTER)
 
 class get_peer_columns():
-    def get_peer_columns(self, columns, interface=None):
-        """Check if each item in iterable `columns` is a valid peer list column name
+    def get_peer_columns(self, columns):
+        """
+        Check if each item in iterable `columns` is a valid peer list column name
 
         Raise ValueError or return a new list of `columns`.
         """
-        from ...views.peerlist import COLUMNS
-        return _get_columns(columns, 'columns.peers', interface, COLUMNS, self.cfg)
+        cols = self.cfg.validate('columns.peers', columns)
+        if 'country' in cols:
+            from ...main import localcfg
+            if not localcfg['geoip']:
+                cols = cols.copy(*(col for col in cols if col != 'country'))
+        return cols
 
 
 
 class get_tracker_sorter():
     def get_tracker_sorter(self, args):
-        """Return TorrentTrackerSorter instance or None
+        """
+        Return TorrentTrackerSorter instance or None
 
         If `args` evaluates to True, it is passed to TorrentTrackerSorter and
         the result is returned.
 
         If `args` evaluates to False, None is returned.
         """
         if args:
             from ...client import TorrentTrackerSorter
-            return TorrentTrackerSorter(utils.listify_args(args))
+            return TorrentTrackerSorter(self.cfg.validate('sort.trackers', args))
 
 class get_tracker_filter():
     def get_tracker_filter(self, FILTER):
-        """Return TorrentTrackerFilter instance or None
+        """
+        Return TorrentTrackerFilter instance or None
 
         If `FILTER` evaluates to True, it is passed to TorrentTrackerFilter and
         the resulting object is returned.
 
         If `FILTER` evaluates to False, None is returned.
         """
         if FILTER:
             from ...client import TorrentTrackerFilter
             return TorrentTrackerFilter(FILTER)
 
 class get_tracker_columns():
-    def get_tracker_columns(self, columns, interface=None):
-        """Check if each item in iterable `columns` is a valid tracker list column name
+    def get_tracker_columns(self, columns):
+        """
+        Check if each item in iterable `columns` is a valid tracker list column name
+
+        Raise ValueError or return a new list of `columns`.
+        """
+        return self.cfg.validate('columns.trackers', columns)
+
+
+
+class get_setting_sorter():
+    def get_setting_sorter(self, args):
+        """
+        Return SettingSorter instance or None
+
+        If `args` evaluates to True, it is passed to SettingSorter and the
+        result is returned.
+
+        If `args` evaluates to False, None is returned.
+        """
+        if args:
+            from ...client import SettingSorter
+            return SettingSorter(self.cfg.validate('sort.settings', args))
+
+class get_setting_columns():
+    def get_setting_columns(self, columns):
+        """
+        Check if each item in iterable `columns` is a valid setting list column name
 
         Raise ValueError or return a new list of `columns`.
         """
-        from ...views.trackerlist import COLUMNS
-        return _get_columns(columns, 'columns.trackers', interface, COLUMNS, self.cfg)
+        return self.cfg.validate('columns.settings', columns)
```

### Comparing `stig-0.8.3a0/stig/commands/base/__init__.py` & `stig-0.9.0a0/stig/commands/base/__init__.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/commands/base/misc.py` & `stig-0.9.0a0/stig/commands/base/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """Base classes for documentation commands"""
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
 from .. import (InitCommand, ExpectedResource)
-from ... import (APPNAME, __version__)
+from ... import (__appname__, __version__)
 
 
 class HelpCmdbase(metaclass=InitCommand):
     name = 'help'
     aliases = ('man',)
     category = 'miscellaneous'
     provides = set()
@@ -58,28 +58,28 @@
 
             if lines:
                 # Remove last TOPIC_DELIMITER
                 for _ in range(len(self.TOPIC_DELIMITER)):
                     lines.pop(-1)
 
         if not existing_topics:
-            existing_topics.append(APPNAME)
+            existing_topics.append(__appname__)
 
         self.display_help(existing_topics, lines)
         return success
 
 
 class VersionCmdbase(metaclass=InitCommand):
     name = 'version'
     category = 'miscellaneous'
     provides = set()
-    description = 'Show {} version'.format(APPNAME)
+    description = 'Show {} version'.format(__appname__)
 
     def run(self):
-        log.info('{} version {}'.format(APPNAME, __version__))
+        log.info('{} version {}'.format(__appname__, __version__))
         return True
 
 
 class LogCmdbase(metaclass=InitCommand):
     name = 'log'
     provides = set()
     category = 'miscellaneous'
@@ -97,16 +97,15 @@
 
     more_sections = { 'clear': ('Remove all previously logged messages in the TUI.  '
                                 'This action ignores all PARAMETERs.',),
                       'scroll': ('Scroll the log messages up or down in the TUI.  '
                                  'Valid PARAMETERs are "up", "down", "page up", "page down", '
                                  '"top" and "bottom".',),
                       'info': ('Join all PARAMETERs and display them as a normal message.',),
-                      'error': ('Join all PARAMETERs and display them as an error message.',),
-    }
+                      'error': ('Join all PARAMETERs and display them as an error message.',) }
 
     def run(self, ACTION):
         if len(ACTION) < 1:
             log.error('%s: Missing arguments', self.name)
             return False
         elif ACTION[0] == 'clear':
             return self._do('clear', *ACTION[1:])
```

### Comparing `stig-0.8.3a0/stig/commands/base/_common.py` & `stig-0.9.0a0/stig/commands/base/_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
               "the output is optimized for scripting.  Numbers are "
               "unformatted, columns are separated by a horizontal tab "
               "character ('\\t') and headers are not printed."),
              "",
              ("To enforce human-readable, formatted output, set the environment "
               "variables COLUMNS and LINES."),
              "",
-             "\t$ \tCOLUMNS=80 LINES=24 {{APPNAME}} {CMDNAME} | less -R".format(CMDNAME=cmdname) )
+             "\t$ \tCOLUMNS=80 LINES=24 {{__appname__}} {CMDNAME} | less -R".format(CMDNAME=cmdname) )
 
 
 def make_SORT_ORDERS_doc(sortercls, option, setting, append=()):
     doc = [('The following sort orders can be specified with the {option} option '
             'or the "{setting}" setting:').format(option=option, setting=setting),
             '']
 
@@ -57,9 +57,8 @@
 
 def make_COLUMNS_doc(columnspecs, option, setting, append=()):
     return (('The following columns can be specified with the {option} option '
              'or the "{setting}" setting:').format(option=option, setting=setting),
             '',
             '\t%s' % ', '.join(sorted(columnspecs)),
             '',
-            'Columns are separated with "," without spaces.') \
-            + append
+            'Columns are separated with "," without spaces.') + append
```

### Comparing `stig-0.8.3a0/stig/commands/base/file.py` & `stig-0.9.0a0/stig/commands/base/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,42 +36,42 @@
         make_X_FILTER_spec('FILE', or_focused=False, nargs='?'),
         { 'names': ('--columns', '-c'),
           'default_description': "current value of 'columns.files' setting",
           'description': ('Comma-separated list of column names '
                           "(see COLUMNS section)") },
     )
 
-    from ...views.filelist import COLUMNS
+    from ...views.file import COLUMNS
     more_sections = {
         'COLUMNS': make_COLUMNS_doc(COLUMNS, '--columns', 'columns.files'),
         'SCRIPTING': make_SCRIPTING_doc(name),
     }
 
     cfg = ExpectedResource
 
     async def run(self, TORRENT_FILTER, FILE_FILTER, columns):
-        columns = self.cfg['columns.files'].value if columns is None else columns
+        columns = self.cfg['columns.files'] if columns is None else columns
         try:
             columns = self.get_file_columns(columns)
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=False,
                                            discover_torrent=True)
             ffilter = self.select_files(FILE_FILTER,
                                         allow_no_filter=True,
                                         discover_file=False)
         except ValueError as e:
             log.error(e)
             return False
 
         log.debug('Listing %s files of %s torrents', ffilter, tfilter)
 
-        if asyncio.iscoroutinefunction(self.make_flist):
-            return await self.make_flist(tfilter, ffilter, columns)
+        if asyncio.iscoroutinefunction(self.make_file_list):
+            return await self.make_file_list(tfilter, ffilter, columns)
         else:
-            return self.make_flist(tfilter, ffilter, columns)
+            return self.make_file_list(tfilter, ffilter, columns)
 
 
 class PriorityCmdbase(metaclass=InitCommand):
     name = 'priority'
     aliases = ('prio',)
     provides = set()
     category = 'file'
@@ -103,49 +103,40 @@
             if PRIORITY in names:
                 priority = p
                 break
         if priority is None:
             log.error('Invalid priority: {!r}'.format(PRIORITY))
             return False
 
+        # Whether the user manually typed a filter
+        utilize_tui = not bool(TORRENT_FILTER)
+
         try:
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=False,
                                            discover_torrent=True)
+
+            # If the user specified a filter instead of selecting via the TUI,
+            # ignore focused/marked files.
+            log.debug('%sdiscovering file(s)', '' if utilize_tui else 'Not ')
             ffilter = self.select_files(FILE_FILTER,
                                         allow_no_filter=True,
-                                        discover_file=True)
+                                        discover_file=utilize_tui)
         except ValueError as e:
             log.error(e)
             return False
 
-        if not isinstance(tfilter, tuple):
-            # tfilter must be TorrentFilter instance, which means the user
-            # specified a filter and will be informed about the matches.
-            if isinstance(ffilter, tuple):
-                # The user did specify a torrent filter but not a file filter,
-                # so select_files() may have returned a focused file.  But we
-                # assume that the user meant all files of the matching
-                # torrents, otherwise they wouldn't have given a torrent
-                # filter.
-                ffilter = None
-
-            msg = 'New download priority of %s files in %s torrents: %s' % (
-                'all' if ffilter is None else ffilter, tfilter, priority)
-            log.info(msg)
+        if not utilize_tui:
+            log.info('New download priority of %s files in %s torrents: %s',
+                     'all' if ffilter is None else ffilter, tfilter, priority)
             quiet = False
         else:
-            # We're operating on the focused file and success is indiciated by
-            # the updated file list, so no info message necessary.
+            # We're operating on focused/marked file and changes are indiciated
+            # by the updated file list, so no info messages necessary.
             quiet = True
 
-        # If ffilter is a tuple, it is a tuple of (torrent_id, file_id) tuples.
-        # In that case, we overload tfilter with the torrent_ids from ffilter.
-        if isinstance(ffilter, tuple):
-            tfilter = tuple(set(ids[0] for ids in ffilter))
         log.debug('Setting file download priority to %s for %s files of %s torrents',
                   priority, ffilter, tfilter)
-
         response = await self.make_request(
             self.srvapi.torrent.file_priority(tfilter, ffilter, priority),
             polling_frenzy=True, quiet=quiet)
         return response.success
```

### Comparing `stig-0.8.3a0/stig/commands/base/torrent.py` & `stig-0.9.0a0/stig/commands/base/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,60 +30,59 @@
     usage = ('list [<OPTIONS>]',
              'list [<OPTIONS>] <TORRENT FILTER> <TORRENT FILTER> ...')
     examples = ('ls active',
                 'ls !active',
                 'ls seeds<10',
                 'ls active&tracker~example.org',
                 'ls active|idle&tracker~example')
-
     argspecs = (
         make_X_FILTER_spec('TORRENT', or_focused=False, nargs='*'),
 
         { 'names': ('--sort', '-s'),
           'default_description': "current value of 'sort.torrents' setting",
           'description': ('Comma-separated list of sort orders '
                           "(see SORT ORDERS section)") },
 
         { 'names': ('--columns', '-c'),
           'default_description': "current value of 'columns.torrents' setting",
           'description': ('Comma-separated list of column names '
                           "(see COLUMNS section)") },
     )
 
-    from ...views.trackerlist import COLUMNS
-    from ...client.sorters.tsorter import TorrentSorter
+    from ...views.torrent import COLUMNS
+    from ...client.sorters.torrent import TorrentSorter
     more_sections = {
         'COLUMNS': make_COLUMNS_doc(COLUMNS, '--columns', 'columns.torrents'),
         'SORT ORDERS': make_SORT_ORDERS_doc(TorrentSorter, '--sort', 'sort.torrents'),
         'SCRIPTING': make_SCRIPTING_doc(name),
     }
 
     cfg = ExpectedResource
 
     async def run(self, TORRENT_FILTER, sort, columns):
-        sort = self.cfg['sort.torrents'].value if sort is None else sort
-        columns = self.cfg['columns.torrents'].value if columns is None else columns
+        sort = self.cfg['sort.torrents'] if sort is None else sort
+        columns = self.cfg['columns.torrents'] if columns is None else columns
         try:
             columns = self.get_torrent_columns(columns)
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=True,
                                            discover_torrent=False)
             sort = self.get_torrent_sorter(sort)
         except ValueError as e:
             log.error(e)
             return False
         else:
             log.debug('Listing %s torrents sorted by %s', tfilter, sort)
-            if asyncio.iscoroutinefunction(self.make_tlist):
-                return await self.make_tlist(tfilter, sort, columns)
+            if asyncio.iscoroutinefunction(self.make_torrent_list):
+                return await self.make_torrent_list(tfilter, sort, columns)
             else:
-                return self.make_tlist(tfilter, sort, columns)
+                return self.make_torrent_list(tfilter, sort, columns)
 
 
-class TorrentSummaryCmdbase(mixin.get_torrent, metaclass=InitCommand):
+class TorrentSummaryCmdbase(mixin.get_single_torrent, metaclass=InitCommand):
     name = 'summary'
     aliases = ('info', 'details')
     provides = set()
     category = 'torrent'
     description = 'Display detailed torrent information'
     usage = ('summary',
              'summary <TORRENT FILTER>')
@@ -93,38 +92,43 @@
     )
     srvapi = ExpectedResource
 
     async def run(self, TORRENT_FILTER):
         try:
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=False,
-                                           discover_torrent=True)
+                                           discover_torrent=True,
+                                           prefer_focused=True)
         except ValueError as e:
             log.error(e)
             return False
         else:
-            log.debug('Showing summary of torrent: %r', tfilter)
-            if asyncio.iscoroutinefunction(self.display_summary):
-                return await self.display_summary(tfilter)
+            torrent = await self.get_single_torrent(tfilter, keys=('id', 'name'))
+            if not torrent:
+                return False
             else:
-                return self.display_summary(tfilter)
+                log.debug('Showing summary of torrent %r: %r', tfilter, torrent)
+                if asyncio.iscoroutinefunction(self.display_summary):
+                    return await self.display_summary(torrent['id'])
+                else:
+                    return self.display_summary(torrent['id'])
 
 
 class AddTorrentsCmdbase(metaclass=InitCommand):
     name = 'add'
     aliases = ('download','get')
     provides = set()
     category = 'torrent'
     description = 'Download torrents'
     usage = ('add [<OPTIONS>] <TORRENT> <TORRENT> <TORRENT> ...',)
     examples = ('add 72d7a3179da3de7a76b98f3782c31843e3f818ee',
                 'add --stopped http://example.org/something.torrent')
     argspecs = (
         { 'names': ('TORRENT',), 'nargs': '+',
-          'description': 'Link or path to torrent file, magnet link or hash' },
+          'description': 'Link or path to torrent file, magnet link or info hash' },
 
         { 'names': ('--stopped','-s'), 'action': 'store_true',
           'description': 'Do not start downloading the added torrent(s)' },
 
         { 'names': ('--path','-p'),
           'description': 'Custom download directory for added torrent(s)' },
     )
@@ -148,22 +152,22 @@
     name = 'move'
     aliases = ('mv',)
     provides = set()
     category = 'torrent'
     description = "Change torrents' location"
     usage = ('move <PATH>',
              'move <TORRENT FILTER> <PATH>')
-    examples = ('move new/path',
-                'move size>50g path/to/lots/of/storage')
+    examples = ('move ./new/path',
+                'move size>50G /path/to/lots/of/storage')
     argspecs = (
         make_X_FILTER_spec('TORRENT', or_focused=True, nargs='?'),
         {'names': ('PATH',),
-         'description': ('New location of the specified torrent(s).  If PATH is relative '
-                         '(does not start with "/"), it is relative to the value of the '
-                         'setting "srv.path.complete".')},
+         'description': ('Move the specified torrent(s) to this directory.  If PATH is relative '
+                         '(i.e. does not start with "/"), it is relative to the value of the '
+                         'setting "srv.path.complete".  That means "." is the download path.')},
     )
     srvapi = ExpectedResource
 
     async def run(self, TORRENT_FILTER, PATH):
         try:
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=False,
@@ -192,16 +196,14 @@
         make_X_FILTER_spec('TORRENT', or_focused=True, nargs='*'),
         { 'names': ('--delete-files','-d'), 'action': 'store_true',
           'description': 'Delete any downloaded files' },
     )
     srvapi = ExpectedResource
     cfg = ExpectedResource
 
-    CONFIRMATION_TAB_TITLE = "Removal Confirmation"
-
     async def run(self, TORRENT_FILTER, delete_files):
         try:
             tfilter = self.select_torrents(TORRENT_FILTER,
                                            allow_no_filter=False,
                                            discover_torrent=True)
         except ValueError as e:
             log.error(e)
@@ -211,18 +213,21 @@
                 response = await self.make_request(
                     self.srvapi.torrent.remove(tfilter, delete=delete_files),
                     polling_frenzy=True)
                 return response.success
 
             response = await self.srvapi.torrent.torrents(tfilter, keys=('id',))
             hits = len(response.torrents)
-            if hits > self.cfg['remove.max-hits'].value:
+            if hits > self.cfg['remove.max-hits']:
                 await self.show_list_of_hits(tfilter)
-                question = 'Are you sure you want to remove %d torrent%s?' % (
+                question = 'Are you sure you want to remove %d torrent%s' % (
                     hits, '' if hits == 1 else 's')
+                if delete_files:
+                    question += ' and their files'
+                question += '?'
                 return await self.ask_yes_no(question, yes=do_remove,
                                              after=self.remove_list_of_hits)
             else:
                 return await do_remove()
 
 
 # Argument definitions that are shared between commands
```

### Comparing `stig-0.8.3a0/stig/commands/__init__.py` & `stig-0.9.0a0/stig/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,14 @@
 class CommandManager():
     def __init__(self, loop=None, pre_run_hook=None):
         self.loop = loop if loop is not None else asyncio.get_event_loop()
         self.pre_run_hook = pre_run_hook
         self._cmds = {}
         self._active_interface = None
         self._resources = CallbackDict(callback=self._update_resources)
-        from . import utils
         self._resources.update(cmdmgr=self)
 
     def load_cmds_from_module(self, *modules):
         """Import modules and look for command classes
 
         Command classes must have set metaclass=InitCommand.
         """
@@ -597,15 +596,14 @@
         """Return task that runs `run_async`"""
         log.debug('Creating command chain task: %r', commands)
         return self.loop.create_task(self.run_async(
             commands, on_success, on_error, **kwargs))
 
     def _yield_from_cmdchain(self, cmdchain, **kwargs):
         prev_process_success = True
-        prev_process_exc = None
         for i,cmdline in enumerate(cmdchain):
             if cmdline in OPS_AND and not prev_process_success:
                 log.debug('Previous command failed (%r) - aborting', prev_process_success)
                 break
             elif cmdline in OPS_OR and prev_process_success:
                 log.debug('Previous command succeeded (%r) - aborting', prev_process_success)
                 break
```

### Comparing `stig-0.8.3a0/stig/commands/cli/tracker.py` & `stig-0.9.0a0/stig/commands/cli/tracker.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
 from ..base import tracker as base
 from . import _mixin as mixin
 from .. import ExpectedResource
-from ._table import (print_table, TERMSIZE)
+from ._table import print_table
 
 
 class ListTrackersCmd(base.ListTrackersCmdbase,
                       mixin.make_request, mixin.select_torrents):
     provides = {'cli'}
     srvapi = ExpectedResource
 
-    async def make_trklist(self, torfilter, trkfilter, sort, columns):
+    async def make_tracker_list(self, torfilter, trkfilter, sort, columns):
         response = await self.make_request(
             self.srvapi.torrent.torrents(torfilter, keys=('name', 'trackers')),
             quiet=True)
         torrents = response.torrents
 
         if len(torrents) < 1:
             return False
@@ -40,15 +40,15 @@
         trklist = []
         for torrent in sorted(torrents, key=lambda t: t['name'].lower()):
             trklist.extend(filter_trackers(torrent['trackers']))
 
         sort.apply(trklist, inplace=True)
 
         if trklist:
-            from ...views.trackerlist import COLUMNS as TRACKER_COLUMNS
+            from ...views.tracker import COLUMNS as TRACKER_COLUMNS
             print_table(trklist, columns, TRACKER_COLUMNS)
             return True
         else:
             filter_is_relevant = lambda f: f and str(f) != 'all'
 
             if filter_is_relevant(trkfilter):
                 errmsg = 'No matching trackers'
```

### Comparing `stig-0.8.3a0/stig/commands/cli/_table.py` & `stig-0.9.0a0/stig/commands/cli/_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,41 +8,69 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
-from ...utils import (strwidth, crop_and_align)
+from ...utils.string import (strwidth, stralign, crop_and_align, normalize_unicode)
 
+import re
+import textwrap
 from types import SimpleNamespace
 from shutil import get_terminal_size
 TERMSIZE = get_terminal_size(fallback=(None, None))
 
 
-def _get_cell_string(cell):
+_whitespace_regex = re.compile(r'^\s*$')
+def _wrapped(line, width):
+    # Prevent textwrap.wrap() from filtering out empty lines
+    if _whitespace_regex.match(line):
+        yield line
+    else:
+        yield from textwrap.wrap(line, width=width, break_on_hyphens=False)
+
+def _get_cell_lines(cell):
     # Return string of single cell correctly cropped/padded and aligned
-    value = cell.get_value()
+    line = normalize_unicode(str(cell.get_cli_value()))
     width = cell.width
     if isinstance(width, int):
-        return crop_and_align(str(value), width, cell.align,
-                              has_wide_chars=cell.may_have_wide_chars)
+        if cell.wrap == 'clip':
+            return (crop_and_align(line, width, cell.align,
+                                   has_wide_chars=cell.may_have_wide_chars),)
+        else:
+            return tuple(stralign(line, width=width)
+                         for line in _wrapped(line, width))
     else:
-        return str(value)
+        return (line,)
 
-def _assemble_line(table, line_index, pretty=True):
+def _assemble_row(table, line_index, pretty=True):
     # Concatenate all cells in a row with delimiters
-    row = table.rows[line_index]
-    line = []
-    for cell in row:
+    # Return a list of lines (cells may have multiple lines)
+    row = []
+    for cell in table.rows[line_index]:
         if pretty:
-            line.append(_get_cell_string(cell))
+            row.append(_get_cell_lines(cell))
         else:
-            line.append(str(cell.get_raw()))
-    return table.delimiter.join(line)
+            row.append((str(cell.get_raw_value()),))
+
+    lines_count = max(len(cell) for cell in row)
+    lines = []
+    delimiter = table.delimiter
+    for i in range(lines_count):
+        # `row` is a list of cells; each `cell` is a list of lines in an
+        # individual cell.
+        line = []
+        for cell in row:
+            cell_lines = len(cell)
+            empty_space = ' ' * len(cell[0])
+            line.append(cell[i] if i < cell_lines else empty_space)
+        line = table.delimiter.join(line)
+        lines.append(line)
+    return lines
 
 def _assemble_headers(table):
     # Concatenate all column headers with delimiters
     # This must be called after shrink_and_expand_to_fit() so we can
     # grab the final column widths from the first row.
     headers = []
     for colname in table.colorder:
@@ -58,21 +86,17 @@
 def _get_header_width(table, colname):
     header = table.colspecs[colname].header
     return strwidth(' '.join((header.get('left', ''),
                               header.get('right', ''))).strip())
 
 def _get_colwidth(table, colindex):
     # Return width of widest cell in column
-    return max(strwidth(str(row[colindex].get_value()))
-               for row in table.rows)
-
-def _get_min_colwidth(table, colindex):
-    # Return minimum column width according to column specs (column becomes
-    # useless if narrower)
-    return table.rows[0][colindex].min_width
+    rows = (normalize_unicode(str(row[colindex].get_cli_value()))
+            for row in table.rows)
+    return max(strwidth(row) for row in rows)
 
 def _column_has_variable_width(table, colname):
     # Whether column has fixed or variable width
     return not isinstance(table.colspecs[colname].width, int)
 
 def _column_could_use_more_width(table, colname):
     # Whether any cell in a column is cropped
@@ -93,15 +117,16 @@
     # Set maximum width a column can make use of (no cell needs more horizontal
     # space than `maxwidth`)
     colname = table.colorder[colindex]
     table.maxcolwidths[colname] = maxwidth
 
 def _get_excess_width(table):
     # Return width by which table must be narrowed to fit in max_width
-    return strwidth(_assemble_line(table, 0)) - table.max_width
+    first_line = _assemble_row(table, 0)[0]
+    return strwidth(first_line) - table.max_width
 
 def _remove_column(table, colindex):
     # Delete column from internal structures
     del table.colwidths[table.colorder[colindex]]
     del table.colorder[colindex]
     for row in table.rows:
         del row[colindex]
@@ -153,15 +178,15 @@
     freed_width = -_get_excess_width(table)
     if freed_width > 0:
         while freed_width > 0:
             freed_width -= 1
             # Find non-fixed-width columns that could use more width
             candidates = [(colname,table.colwidths[colname])
                           for colname in table.colorder
-                          if _column_has_variable_width(table, colname) and \
+                          if _column_has_variable_width(table, colname) and
                              _column_could_use_more_width(table, colname)]
             if not candidates:
                 # We have space left, but no column wants it
                 break
             candidates_sorted = sorted(candidates, key=lambda col: col[1])
             colname = candidates_sorted[0][0]
             new_width = table.colwidths[candidates_sorted[0][0]] + 1
@@ -178,15 +203,16 @@
         _set_colwidth(table, colindex, colwidth)
 
     _shrink_to_widest_value(table)
     _shrink_variable_width_columns(table)
     _shrink_by_removing_columns(table)
 
 def print_table(items, order, column_specs):
-    """Print table from a two-dimensional array of column objects
+    """
+    Print table from a two-dimensional array of column objects
 
     `column_specs` maps column IDs to ColumnBase classes.  A column ID is any
     hashable object, but you probably want strings like 'name', 'id', 'date',
     etc.
 
     `order` is a sequence of column IDs.
 
@@ -218,9 +244,9 @@
         else:
             log.debug('Could not detect TTY size - assuming stdout is no TTY')
 
         for line_index in range(len(table.rows)):
             # Print column headers after every screen full
             if pretty_output and line_index % (TERMSIZE.lines-2) == 0:
                 log.info(headerstr)
-            log.info(_assemble_line(table, line_index, pretty=pretty_output))
-
+            for row in _assemble_row(table, line_index, pretty=pretty_output):
+                log.info(row)
```

### Comparing `stig-0.8.3a0/stig/commands/cli/peer.py` & `stig-0.9.0a0/stig/commands/cli/peer.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class ListPeersCmd(base.ListPeersCmdbase,
                    mixin.make_request, mixin.select_torrents):
     provides = {'cli'}
     srvapi = ExpectedResource
 
-    async def make_plist(self, tfilter, pfilter, sort, columns):
+    async def make_peer_list(self, tfilter, pfilter, sort, columns):
         response = await self.make_request(
             self.srvapi.torrent.torrents(tfilter, keys=('name', 'peers')),
             quiet=True)
         torrents = response.torrents
 
         if len(torrents) < 1:
             return False
@@ -37,18 +37,24 @@
         else:
             filter_peers = lambda peers: pfilter.apply(peers)
 
         peerlist = []
         for torrent in sorted(torrents, key=lambda t: t['name'].lower()):
             peerlist.extend(filter_peers(torrent['peers']))
 
+        # Pre-lookup peers' IPs
+        from ...main import localcfg
+        if 'ip' in columns and localcfg['reverse-dns']:
+            from ...client import rdns
+            rdns.query(*(p['ip'] for p in peerlist))
+
         sort.apply(peerlist, inplace=True)
 
         if peerlist:
-            from ...views.peerlist import COLUMNS as PEER_COLUMNS
+            from ...views.peer import COLUMNS as PEER_COLUMNS
             print_table(peerlist, columns, PEER_COLUMNS)
             return True
         else:
             filter_is_relevant = lambda f: f and str(f) != 'all'
 
             if filter_is_relevant(pfilter):
                 errmsg = 'No matching peers'
```

### Comparing `stig-0.8.3a0/stig/commands/cli/_mixin.py` & `stig-0.9.0a0/stig/commands/cli/_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,61 +12,66 @@
 """Mixin classes for CLI commands"""
 
 from ...logging import make_logger
 log = make_logger(__name__)
 
 from .. import ExpectedResource
 from .. import utils
+from ._common import clear_line
 
 
 class make_request():
     async def make_request(self, request_coro, polling_frenzy=False, quiet=False):
         """Awaits request coroutine and logs messages; returns response"""
         response = await request_coro
         utils.log_msgs(log, response.msgs, quiet)
         return response
 
 
-class user_confirmation():
+class ask_yes_no():
     aioloop = ExpectedResource
 
     ANSWERS = {'y': True, 'n': False,
-               'Y': True, 'N': False}
+               'Y': True, 'N': False,
+               '\x03': False,  # ctrl-c
+               '\x07': False,  # ctrl-g
+               '\x1b': False}  # escape
 
     async def ask_yes_no(self, question, yes=None, no=None, after=None):
-        """Ask user a yes/no question
+        """
+        Ask user a yes/no question and return True/False
 
         The `yes` and `no` arguments are callbacks (or None) that are called
         depending on the user's answer. `after` is called after the user
         answered and after `yes` or `no` has been called.
 
         Callbacks may be normal functions, coroutine functions or
         coroutines. They don't get any arguments and their return value is
         ignored.
         """
         import sys, tty, termios
         async def aiogetch(loop):
             # Disable printing of typed characters
             old_settings = termios.tcgetattr(sys.stdin.fileno())
-            tty.setcbreak(sys.stdin.fileno())
+            tty.setraw(sys.stdin.fileno())
 
             # Read exactly one character
             key = await loop.run_in_executor(None, sys.stdin.read, 1)
 
-            # Restore terminal settings and remove question
+            # Restore terminal settings
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old_settings)
-            print('\r\033[2K', end='', flush=True)
 
             return key
 
         # Get an answer from user
-        print(question, end=' [y|n] ', flush=True)
         answer = None
         while answer is None:
+            print(question, end=' [y|n] ', flush=True)
             key = await aiogetch(self.aioloop)
+            clear_line()
             answer = self.ANSWERS.get(key, None)
 
         # Run yes, no and after callbacks
         import asyncio
         async def run_func_or_coro(func_or_coro):
             if asyncio.iscoroutinefunction(func_or_coro):
                 await func_or_coro()
@@ -80,42 +85,44 @@
         else:
             await run_func_or_coro(no)
         await run_func_or_coro(after)
         return answer
 
 
 class select_torrents():
-    def select_torrents(self, FILTER, allow_no_filter=True, discover_torrent=None):
-        """Get TorrentFilter instance or None
+    def select_torrents(self, FILTER, allow_no_filter=True, discover_torrent=None, prefer_focused=None):
+        """
+        Get TorrentFilter instance or None
 
         If `FILTER` evaluates to True, it is passed to TorrentFilter and the
         resulting object is returned.
 
         If `FILTER` evaluates to False, None is returned if allow_no_filter
         evaluates to True, otherwise a ValueError is raised.
 
-        `discover_torrent` is ignored and only used in the TUI version of this
-        method (see ..tui.mixin.select_torrent).
+        `discover_torrent` and `prefer_focused` are ignored and only used in the
+        TUI version of this method.
         """
         if FILTER:
             from ...client import TorrentFilter
             return TorrentFilter(FILTER)
         else:
             if allow_no_filter:
                 return None
             else:
                 raise ValueError('No torrent specified')
 
 
 class select_files():
     def select_files(self, FILTER, allow_no_filter=True, discover_file=None):
-        """Get TorrentFileFilter instance or None
+        """
+        Get TorrentFileFilter instance or None
 
-        If `FILTER` evaluates to True, it is passed to TorrentFileFilter and
-        the resulting object is returned.
+        If `FILTER` evaluates to True, it is passed to TorrentFileFilter and the
+        resulting object is returned.
 
         If `FILTER` evaluates to False, None is returned if allow_no_filter
         evaluates to True, otherwise a ValueError is raised.
 
         `discover_file` is ignored and only used in the TUI version of this
         method (see ..tui.mixin.select_file).
         """
```

### Comparing `stig-0.8.3a0/stig/commands/cli/__init__.py` & `stig-0.9.0a0/stig/commands/tui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 
 from .config import *
 from .misc import *
 from .torrent import *
 from .file import *
 from .peer import *
 from .tracker import *
+from .tui import *
```

### Comparing `stig-0.8.3a0/stig/commands/cli/misc.py` & `stig-0.9.0a0/stig/commands/cli/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 
     cfg = ExpectedResource
     srvapi = ExpectedResource
 
     async def run(self, TOPIC):
         # If TOPIC is a setting and it is managed by the server, we must fetch
         # config values from the server so we can display its current value.
-        from ...settings import is_srv_setting
         for topic in TOPIC:
-            if is_srv_setting(topic, self.cfg):
+            if topic.startswith('srv.'):
                 try:
                     await self.srvapi.settings.update()
                 except self.srvapi.ClientError as e:
                     log.error(str(e))
                 finally:
                     break
```

### Comparing `stig-0.8.3a0/stig/commands/cli/file.py` & `stig-0.9.0a0/stig/commands/cli/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 
 class ListFilesCmd(base.ListFilesCmdbase,
                    mixin.make_request, mixin.select_torrents, mixin.select_files,
                    mixin.only_supported_columns):
     provides = {'cli'}
     srvapi = ExpectedResource
 
-    async def make_flist(self, tfilter, ffilter, columns):
+    async def make_file_list(self, tfilter, ffilter, columns):
         response = await self.make_request(
             self.srvapi.torrent.torrents(tfilter, keys=('name', 'files')),
             quiet=True)
         torrents = response.torrents
 
         if len(torrents) < 1:
             return False
 
         filelist = []
         for torrent in sorted(torrents, key=lambda t: t['name'].lower()):
             files, filtered_count = self._flatten_tree(torrent['files'], ffilter)
             filelist.extend(files)
 
         if filelist:
-            from ...views.filelist import COLUMNS as FILE_COLUMNS
+            from ...views.file import COLUMNS as FILE_COLUMNS
             # Remove columns that aren't supported by CLI interface (e.g. 'marked')
             columns = self.only_supported_columns(columns, FILE_COLUMNS)
             print_table(filelist, columns, FILE_COLUMNS)
             return True
         else:
             if str(tfilter) != 'all':
                 log.error('No matching files in {} torrents: {}'.format(tfilter, ffilter))
@@ -57,42 +57,45 @@
         """Return list of rows for `print_table`
 
         `files` must be a nested mapping tree (i.e. TorrentFileTree).
         `ffilter` must be a TorrentFileFilter instance or None.
         """
         if TERMSIZE.columns is None:
             def indent_file_name(node):
-                node['name'] = os.path.join(node['path'], node['name'])
+                path = node['path']
+                if path != '.':
+                    node['name'] = os.path.join(path, node['name'])
+                node['name'] = os.path.join(node['location'], node['name'])
 
             def indent_directory_name(node):
                 node['name'] = node['path']
         else:
             def indent_file_name(node):
                 node['name'] = '%s%s' % ('  '*(_indent_level), node['name'])
             indent_directory_name = indent_file_name
 
-        from ...views.filelist import create_directory_data
+        from ...views.file import create_directory_data
         flist = []
         filtered_count = 0
         for key,value in sorted(files.items(), key=lambda pair: pair[0].lower()):
             if value.nodetype == 'leaf':
                 if ffilter is None or ffilter.match(value):
                     filenode = dict(value)  # Copy original TorrentFile
                     indent_file_name(filenode)
                     flist.append(filenode)
                 else:
                     filtered_count += 1
 
             elif value.nodetype == 'parent':
                 sub_flist, sub_filtered_count = self._flatten_tree(value, ffilter, _indent_level+1)
-                dirnode = create_directory_data(key, value, sub_filtered_count)
-                indent_directory_name(dirnode)
-                flist.append(dirnode)
+                if TERMSIZE.columns is not None:
+                    dirnode = create_directory_data(key, value, sub_filtered_count)
+                    indent_directory_name(dirnode)
+                    flist.append(dirnode)
                 flist.extend(sub_flist)
 
         return flist, filtered_count
 
 
 class PriorityCmd(base.PriorityCmdbase,
                   mixin.make_request, mixin.select_torrents, mixin.select_files):
     provides = {'cli'}
-
```

### Comparing `stig-0.8.3a0/stig/commands/cli/torrent.py` & `stig-0.9.0a0/stig/commands/cli/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 class ListTorrentsCmd(base.ListTorrentsCmdbase,
                       mixin.make_request, mixin.select_torrents,
                       mixin.only_supported_columns):
     provides = {'cli'}
     srvapi = ExpectedResource  # TUI version of 'list' doesn't need srvapi
 
-    async def make_tlist(self, tfilter, sort, columns):
-        from ...views.torrentlist import COLUMNS as TORRENT_COLUMNS
+    async def make_torrent_list(self, tfilter, sort, columns):
+        from ...views.torrent import COLUMNS as TORRENT_COLUMNS
 
         # Remove columns that aren't supported by CLI interface (e.g. 'marked')
         columns = self.only_supported_columns(columns, TORRENT_COLUMNS)
 
         # Get wanted torrents and sort them
         if tfilter is None:
             keys = set(sort.needed_keys)
@@ -47,28 +47,23 @@
         return len(torrents) > 0
 
 
 class TorrentsSummaryCmd(base.TorrentSummaryCmdbase,
                          mixin.make_request, mixin.select_torrents):
     provides = {'cli'}
 
-    async def display_summary(self, tfilter):
-        torrent = await self.get_torrent(tfilter, keys=('id',))
-        if torrent is None:
-            return False
-        tid = torrent['id']
-
+    async def display_summary(self, torrent_id):
         from ...views.summary import SECTIONS
         needed_keys = set(('name',))
         for _section in SECTIONS:
             for _item in _section['items']:
                 needed_keys.update(_item.needed_keys)
 
         response = await self.make_request(
-            self.srvapi.torrent.torrents((tid,), keys=needed_keys),
+            self.srvapi.torrent.torrents((torrent_id,), keys=needed_keys),
             quiet=True)
         if len(response.torrents) < 1:
             return False
         else:
             torrent = response.torrents[0]
 
         # Whether to print for a human or for a machine to read our output
@@ -105,15 +100,15 @@
 
 class MoveTorrentsCmd(base.MoveTorrentsCmdbase,
                       mixin.make_request, mixin.select_torrents):
     provides = {'cli'}
 
 
 class RemoveTorrentsCmd(base.RemoveTorrentsCmdbase,
-                        mixin.make_request, mixin.select_torrents, mixin.user_confirmation):
+                        mixin.make_request, mixin.select_torrents, mixin.ask_yes_no):
     provides = {'cli'}
     cmdmgr = ExpectedResource
 
     async def show_list_of_hits(self, tfilter):
         cmd = 'ls --sort name %s' % tfilter
         await self.cmdmgr.run_async(cmd)
```

### Comparing `stig-0.8.3a0/stig/commands/tui/tracker.py` & `stig-0.9.0a0/stig/commands/tui/tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..base import tracker as base
 from . import _mixin as mixin
-from .. import (ExpectedResource, InitCommand)
 
 
 class ListTrackersCmd(base.ListTrackersCmdbase,
                       mixin.make_request,
                       mixin.select_torrents,
                       mixin.create_list_widget):
     provides = {'tui'}
 
-    def make_trklist(self, torfilter, trkfilter, sort, columns):
-        from ...tui.views.trackerlist import TrackerListWidget
+    def make_tracker_list(self, torfilter, trkfilter, sort, columns):
+        from ...tui.views.tracker_list import TrackerListWidget
         self.create_list_widget(TrackerListWidget, theme_name='trackerlist',
                                 torfilter=torfilter, trkfilter=trkfilter,
                                 sort=sort, columns=columns,
                                 markable_items=False)
         return True
```

### Comparing `stig-0.8.3a0/stig/commands/tui/tui.py` & `stig-0.9.0a0/stig/commands/tui/tui.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 log = make_logger(__name__)
 
 from .. import (InitCommand, ExpectedResource)
 from . import _mixin as mixin
 from ._common import make_tab_title_widget
 
 import shlex
+from functools import partial
 
 
 # Import tui.main module only on demand
-def _get_KEYMAP_CONTEXTS():
-    from ...tui.main import KEYMAP_CONTEXTS
-    return sorted(KEYMAP_CONTEXTS)
+def _get_keymap_contexts():
+    from ...tui.main import keymap
+    return tuple(keymap.contexts)
 
 
 class BindCmd(metaclass=InitCommand):
     name = 'bind'
     provides = {'tui'}
     category = 'tui'
     description = 'Bind keys to commands or other keys'
@@ -54,16 +55,16 @@
     def __create_CONTEXTS_section():
         lines = [
             ('Keys are mapped in contexts.  With no context given, the default '
              'context is used.  The default context only gets the key if no '
              'other context wants it.  The same key can be mapped to different '
              'actions in different contexts.'),
             '',
-            'Available contexts are: ' + \
-              ', '.join('%s' % context for context in _get_KEYMAP_CONTEXTS()),
+            'Available contexts are: ' +
+              ', '.join('%s' % context for context in _get_keymap_contexts()),
             '',
             'EXAMPLE',
             '\tbind --context torrent ctrl-t start',
             '\tbind --context tabs ctrl-t tab',
             '\tbind ctrl-t <left>',
             '',
             ('\tWhen focusing a torrent, <ctrl-t> starts the focused torrent.  '
@@ -98,17 +99,16 @@
         if len(ACTION) == 1 and ACTION[0][0] == '<' and ACTION[0][-1] == '>':
             # ACTION is another key (e.g. 'j' -> 'down')
             action = keymap.mkkey(ACTION[0])
         else:
             action = ' '.join(shlex.quote(x) for x in ACTION)
 
         if context is None:
-            from ...tui.keymap import DEFAULT_CONTEXT
-            context = DEFAULT_CONTEXT
-        elif context not in _get_KEYMAP_CONTEXTS():
+            context = keymap.DEFAULT_CONTEXT
+        elif context not in _get_keymap_contexts():
             log.error('Invalid context: {!r}'.format(context))
             return False
 
         try:
             keymap.bind(key, action, context=context)
         except ValueError as e:
             log.error(e)
@@ -139,17 +139,16 @@
     def run(self, context, all, KEY):
         keymap = self.tui.keymap
 
         if all:
             keymap.clear()
 
         if context is None:
-            from ...tui.keymap import DEFAULT_CONTEXT
-            context = DEFAULT_CONTEXT
-        elif context not in _get_KEYMAP_CONTEXTS():
+            context = keymap.DEFAULT_CONTEXT
+        elif context not in _get_keymap_contexts():
             log.error('Invalid context: {!r}'.format(context))
             return False
 
         success = True
         for key in KEY:
             try:
                 keymap.unbind(key, context=context)
@@ -183,15 +182,15 @@
                    'specified by the settings "tui.marked.on" and "tui.marked.off".')),
     }
 
     tui = ExpectedResource
 
     def run(self, focus_next, toggle, all):
         widget = self.tui.tabs.focus
-        if not hasattr(widget, 'mark'):
+        if not widget.has_marked_column:
             log.error('Nothing to mark here.')
             return False
         else:
             widget.mark(toggle=toggle, all=all)
             if focus_next:
                 widget.focus_position += 1
             return True
@@ -213,15 +212,15 @@
     )
     more_sections = MarkCmd.more_sections
 
     tui = ExpectedResource
 
     def run(self, focus_next, toggle, all):
         widget = self.tui.tabs.focus
-        if not hasattr(widget, 'unmark'):
+        if not widget.has_marked_column:
             log.error('Nothing to unmark here.')
             return False
         else:
             widget.unmark(toggle=toggle, all=all)
             if focus_next:
                 widget.focus_position += 1
             return True
@@ -234,14 +233,94 @@
     description = 'Terminate the TUI'
 
     def run(self):
         import urwid
         raise urwid.ExitMainLoop()
 
 
+class SortCmd(metaclass=InitCommand):
+    name = 'sort'
+    aliases = ()
+    provides = {'tui'}
+    category = 'tui'
+    description = "Sort lists of torrents/peers/trackers/etc"
+    usage = ('sort [<OPTIONS>] [<ORDER> <ORDER> <ORDER> ...]',)
+    examples = ('sort tracker status !rate-down',
+                'sort --add eta')
+    argspecs = (
+        {'names': ('ORDER',), 'nargs': '*',
+         'description': 'How to sort list items (see SORT ORDERS section)'},
+
+        {'names': ('--add', '-a'), 'action': 'store_true',
+         'description': 'Append ORDERs to current list of sort orders instead of replacing it'},
+
+        {'names': ('--reset', '-r'), 'action': 'store_true',
+         'description': 'Go back to sort order that was used when list was created'},
+
+        {'names': ('--none', '-n'), 'action': 'store_true',
+         'description': 'Remove all sort orders from the list'},
+    )
+
+    def _list_sort_orders(title, sortercls):
+        return (title,) + \
+            tuple('\t{}\t - \t{}'.format(', '.join((sname,) + s.aliases), s.description)
+                  for sname,s in sorted(sortercls.SORTSPECS.items()))
+
+    from ...client import (TorrentSorter, TorrentPeerSorter,
+                           TorrentTrackerSorter, SettingSorter)
+    more_sections = {
+        'SORT ORDERS': _list_sort_orders('TORRENT LISTS', TorrentSorter) +
+                       ('',) +
+                       _list_sort_orders('PEER LISTS', TorrentPeerSorter) +
+                       ('',) +
+                       _list_sort_orders('TRACKER LISTS', TorrentTrackerSorter)
+    }
+
+    tui = ExpectedResource
+
+    async def run(self, add, reset, none, ORDER):
+        current_tab = self.tui.tabs.focus
+
+        if reset:
+            current_tab.sort = 'RESET'
+
+        if none:
+            current_tab.sort = None
+
+        if ORDER:
+            # Find appropriate sorter class for focused list
+            from ...tui.views.torrent_list import TorrentListWidget
+            from ...tui.views.peer_list import PeerListWidget
+            from ...tui.views.tracker_list import TrackerListWidget
+            from ...tui.views.setting_list import SettingListWidget
+            if isinstance(current_tab, TorrentListWidget):
+                sortcls = self.TorrentSorter
+            elif isinstance(current_tab, PeerListWidget):
+                sortcls = self.TorrentPeerSorter
+            elif isinstance(current_tab, TrackerListWidget):
+                sortcls = self.TorrentTrackerSorter
+            elif isinstance(current_tab, SettingListWidget):
+                sortcls = self.SettingSorter
+            else:
+                log.error('Current tab is not sortable.')
+                return False
+
+            try:
+                new_sort = sortcls(ORDER)
+            except ValueError as e:
+                log.error(e)
+                return False
+
+            if add and current_tab.sort is not None:
+                current_tab.sort += new_sort
+            else:
+                current_tab.sort = new_sort
+            return True
+
+
 class TabCmd(mixin.select_torrents, metaclass=InitCommand):
     name = 'tab'
     provides = {'tui'}
     category = 'tui'
     description = 'Open, close and focus tabs'
     usage = ('tab [<OPTIONS>]',
              'tab [<OPTIONS>] <COMMAND>')
@@ -430,15 +509,15 @@
                           'see ELEMENT NAMES section for a list') },
     )
 
     # Lazily load the element names from tui (HelpManager supports sequences
     # of lines or a callable that returns them)
     def __create_element_names():
         from ...tui.main import widgets
-        return ('Available TUI element names are: ' + \
+        return ('Available TUI element names are: ' +
                 ', '.join(str(e) for e in sorted(widgets.names_recursive)),)
     more_sections = { 'ELEMENT NAMES': __create_element_names }
 
     tui = ExpectedResource
 
     def run(self, ACTION, ELEMENT):
         widgets = self.tui.widgets
@@ -455,92 +534,18 @@
                     current_path.append(widgetname)
                     widget = getattr(widget, widgetname)
             except AttributeError as e:
                 log.error('Unknown TUI element: %r', '.'.join(current_path))
 
             if widget is not None:
                 action = getattr(widget, ACTION)
+                if any(ACTION == x for x in ('hide', 'toggle')):
+                    action = partial(action, free_space=False)
+                log.debug(action)
+
                 log.debug('%sing %s in %s', ACTION.capitalize(), target_name, widget)
                 try:
                     action(target_name)
                     success = True
                 except ValueError as e:
                     log.error(e)
         return success
-
-
-class SortCmd(metaclass=InitCommand):
-    name = 'sort'
-    aliases = ()
-    provides = {'tui'}
-    category = 'tui'
-    description = "Sort lists of torrents/peers/trackers/etc"
-    usage = ('sort [<OPTIONS>] [<ORDER> <ORDER> <ORDER> ...]',)
-    examples = ('sort tracker status !rate-down',
-                'sort --add eta')
-    argspecs = (
-        {'names': ('ORDER',), 'nargs': '*',
-         'description': 'How to sort list items (see SORT ORDERS section)'},
-
-        {'names': ('--add', '-a'), 'action': 'store_true',
-         'description': 'Append ORDERs to current list of sort orders instead of replacing it'},
-
-        {'names': ('--reset', '-r'), 'action': 'store_true',
-         'description': 'Go back to sort order that was used when list was created'},
-
-        {'names': ('--none', '-n'), 'action': 'store_true',
-         'description': 'Remove all sort orders from the list'},
-    )
-
-    def _list_sort_orders(title, sortercls):
-        return (title,) + \
-            tuple('\t{}\t - \t{}'.format(', '.join((sname,) + s.aliases), s.description)
-                  for sname,s in sorted(sortercls.SORTSPECS.items()))
-
-    from ...client.sorters.tsorter import TorrentSorter
-    from ...client.sorters.psorter import TorrentPeerSorter
-    from ...client.sorters.trksorter import TorrentTrackerSorter
-    more_sections = {
-        'SORT ORDERS': _list_sort_orders('TORRENT LISTS', TorrentSorter) + \
-                       ('',) + \
-                       _list_sort_orders('PEER LISTS', TorrentPeerSorter) + \
-                       ('',) + \
-                       _list_sort_orders('TRACKER LISTS', TorrentTrackerSorter)
-    }
-
-    tui = ExpectedResource
-
-    async def run(self, add, reset, none, ORDER):
-        current_tab = self.tui.tabs.focus
-
-        if reset:
-            current_tab.sort = 'RESET'
-
-        if none:
-            current_tab.sort = None
-
-        if ORDER:
-            # Find appropriate sorter class for focused list
-            from ...tui.views.torrentlist import TorrentListWidget
-            from ...tui.views.peerlist import PeerListWidget
-            from ...tui.views.trackerlist import TrackerListWidget
-            if isinstance(current_tab, TorrentListWidget):
-                sortcls = self.TorrentSorter
-            elif isinstance(current_tab, PeerListWidget):
-                sortcls = self.TorrentPeerSorter
-            elif isinstance(current_tab, TrackerListWidget):
-                sortcls = self.TorrentTrackerSorter
-            else:
-                log.error('Current tab does not contain a torrent, peer or tracker list.')
-                return False
-
-            try:
-                new_sort = sortcls(ORDER)
-            except ValueError as e:
-                log.error(e)
-                return False
-
-            if add and current_tab.sort is not None:
-                current_tab.sort += new_sort
-            else:
-                current_tab.sort = new_sort
-            return True
```

### Comparing `stig-0.8.3a0/stig/commands/tui/peer.py` & `stig-0.9.0a0/stig/commands/tui/peer.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..base import peer as base
 from . import _mixin as mixin
-from .. import (ExpectedResource, InitCommand)
 
 
 class ListPeersCmd(base.ListPeersCmdbase,
                    mixin.make_request,
                    mixin.select_torrents,
                    mixin.create_list_widget):
     provides = {'tui'}
 
-    def make_plist(self, tfilter, pfilter, sort, columns):
-        from ...tui.views.peerlist import PeerListWidget
+    def make_peer_list(self, tfilter, pfilter, sort, columns):
+        from ...tui.views.peer_list import PeerListWidget
         self.create_list_widget(PeerListWidget, theme_name='peerlist',
                                 tfilter=tfilter, pfilter=pfilter,
                                 sort=sort, columns=columns,
                                 markable_items=False)
         return True
```

### Comparing `stig-0.8.3a0/stig/commands/tui/_mixin.py` & `stig-0.9.0a0/stig/commands/tui/_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,24 @@
         response = await request_coro
         utils.log_msgs(log, response.msgs, quiet)
         if response.success and polling_frenzy:
             self.polling_frenzy()
         return response
 
 
-class user_confirmation():
+class ask_yes_no():
     tui     = ExpectedResource
     aioloop = ExpectedResource
 
     ANSWERS = {'y': True, 'n': False,
                'Y': True, 'N': False}
 
     async def ask_yes_no(self, question, yes=None, no=None, after=None):
-        """Ask user a yes/no question
+        """
+        Ask user a yes/no question
 
         The `yes` and `no` arguments are callbacks (or None) that are called
         depending on the user's answer. `after` is called after the user
         answered and after `yes` or `no` has been called.
 
         Callbacks may be normal functions, coroutine functions or
         coroutines. They don't get any arguments and their return value is
@@ -79,68 +80,86 @@
         tui.widgets.add(widget=widget, name='yesnoprompt', removable=True,
                         options='pack', position=pos)
 
 
 class select_torrents():
     tui = ExpectedResource
 
-    def select_torrents(self, FILTER, allow_no_filter=True, discover_torrent=True):
-        """Get TorrentFilter instance or focused/marked torrent IDs
+    def select_torrents(self, FILTER, allow_no_filter=True, discover_torrent=True, prefer_focused=False):
+        """
+        Get TorrentFilter instance or None
 
         If `FILTER` evaluates to True, it is passed to TorrentFilter and the
         resulting object is returned.
 
         If `FILTER` evaluates to False, the result of `discover_torrent_ids` is
-        returned if `discover_torrent` evaluates to True. Otherwise, None is
-        returned if `allow_no_filter` evaluates to True, else a ValueError is
-        raised.
+        returned if `discover_torrent` evaluates to True.  `prefer_focused` is
+        forwarded to `discover_torrent_ids`.  If `discover_torrent` evaluates to
+        False, None is returned if `allow_no_filter` evaluates to True,
+        otherwise a ValueError is raised.
         """
         if FILTER:
             from ...client import TorrentFilter
             return TorrentFilter(FILTER)
         else:
             if discover_torrent:
-                tids = self.discover_torrent_ids()
+                tids = self.discover_torrent_ids(prefer_focused=prefer_focused)
                 if tids is not None:
-                    return tids
+                    return self.ids2tfilter(tids)
 
             if allow_no_filter:
                 return None
 
             else:
                 raise ValueError('No torrent specified')
 
-    def discover_torrent_ids(self):
-        """Auto-detect which torrents are currently selected by the user
+    def discover_torrent_ids(self, prefer_focused=False):
+        """
+        Auto-detect which torrents are currently selected by the user
 
-        Try `get_marked_torrent_ids` first, then `get_focused_torrent_id`.
+        Torrents are selected by marking them or by focusing them.  If
+        `prefer_focused` evaluates to True, the focused torrent ID is returned,
+        if possible, before looking for marks.  Otherwise, the focused torrent
+        ID is only returned if there are no marked torrents.
 
         If any torrents are found, return a tuple of torrent IDs, otherwise
         None.
         """
-        tids = self.get_marked_torrent_ids()
-        if tids:
-            return tids
-        tid = self.get_focused_torrent_id()
-        if tid:
-            return (tid,)
+        def get_marked():
+            tids = self.get_marked_torrent_ids()
+            if tids:
+                log.debug('Found marked torrents: %r', tids)
+                return tids
+
+        def get_focused():
+            tid = self.get_focused_torrent_id()
+            if tid:
+                log.debug('Found focused torrent: %r', tid)
+                return (tid,)
+
+        if prefer_focused:
+            return get_focused() or get_marked()
+        else:
+            return get_marked() or get_focused()
 
     def get_marked_torrent_ids(self):
-        """Return IDs of marked items in the current or previous tab
+        """
+        Return IDs of marked items in the current or previous tab
 
         This relies on the widget having a `marked` attribute.
         """
         widget = self._get_current_or_previous_tab()
         if hasattr(widget, 'marked'):
-            tids = tuple(twidget.id for twidget in widget.marked)
+            tids = tuple(twidget.torrent_id for twidget in widget.marked)
             if tids:
-                return tids
+                return set(tids)
 
     def get_focused_torrent_id(self):
-        """Return torrent ID of focused item in the current or previous tab
+        """
+        Return torrent ID of focused item in the current or previous tab
 
         This relies on the widget having a `focused_torrent_id` attribute.
         """
         widget = self._get_current_or_previous_tab()
         if hasattr(widget, 'focused_torrent_id'):
             tid = widget.focused_torrent_id
             if tid is not None:
@@ -156,60 +175,73 @@
             try:
                 widget = self.tui.tabs.get_content(self.previous_tab_id)
             except IndexError:
                 pass
             else:
                 return widget
 
+    @staticmethod
+    def ids2tfilter(ids):
+        """Turn an iterable of ids into a TorrentFilter instance"""
+        if all(isinstance(x, int) for x in ids):
+            from ...client import TorrentFilter
+            return TorrentFilter('|'.join(('id=%d' % id for id in ids)))
+        else:
+            raise RuntimeError('Not a list of IDs: %r' % (ids,))
+
 
 class select_files():
     tui = ExpectedResource
 
     def select_files(self, FILTER, allow_no_filter=True, discover_file=True):
-        """Get TorrentFileFilter instance, focused file ID or None
+        """
+        Get TorrentFileFilter instance, focused/marked file IDs or None
 
-        If `FILTER` evaluates to True, it is passed to TorrentFileFilter and
-        the resulting object is returned.
+        If `FILTER` evaluates to True, it is passed to TorrentFileFilter and the
+        resulting object is returned.
 
         If `FILTER` evaluates to False and `discover_file` evaluates to True,
-        the file ID (or IDs) are returned in a tuple if possible. Otherwise,
-        None is returned if `allow_no_filter` evaluates to True, else a
-        ValueError is raised.
+        a tuple of (<torrent ID>, <file ID>) tuples is returned.  If
+        `discover_file` evaluates to False, None is returned if
+        `allow_no_filter` evaluates to True, else a ValueError is raised.
 
-        File are discovered by getting the `focused_file_id` of the focused
+        Files are discovered by getting the `focused_file_ids` of the focused
         tab's widget.
         """
         if FILTER:
             from ...client import TorrentFileFilter
             return TorrentFileFilter(FILTER)
         else:
             if discover_file:
                 fids = self._find_file_ids()
-                if fids is not None:
+                if fids:
+                    log.debug('Found file IDs: %r', fids)
                     return fids
             if allow_no_filter:
                 return None
             else:
                 raise ValueError('No torrent file specified')
 
     def _find_file_ids(self):
         focused_widget = self.tui.tabs.focus
-
+        # Get marked file IDs
         if hasattr(focused_widget, 'marked'):
-            tfids = tuple((fwidget.torrent_id, fwidget.file_id)
-                          for fwidget in focused_widget.marked
-                          if isinstance(fwidget.file_id, int))
-            if tfids:
-                return tfids
-
-        # Get torrent ID from widget in focused tab
-        if hasattr(focused_widget, 'focused_file_ids') and \
-           focused_widget.focused_file_ids is not None:
-            return tuple((focused_widget.focused_torrent_id, fid)
-                         for fid in focused_widget.focused_file_ids)
+            fids = tuple(fwidget.id for fwidget in focused_widget.marked)
+            if fids:
+                log.debug('Found marked files: %r', fids)
+                return fids
+
+        # Get focused file IDs (if directory is focused, include all files in it)
+        if hasattr(focused_widget, 'focused_file_ids'):
+            fids = tuple(focused_widget.focused_file_ids)
+            if fids:
+                log.debug('Found focused files: %r', fids)
+                return fids
+
+        return ()
 
 
 class create_list_widget():
     tui    = ExpectedResource
     srvapi = ExpectedResource
 
     def create_list_widget(self, list_cls, *args, theme_name, markable_items=False, **kwargs):
```

### Comparing `stig-0.8.3a0/stig/commands/tui/misc.py` & `stig-0.9.0a0/stig/commands/tui/misc.py`

 * *Files identical despite different names*

### Comparing `stig-0.8.3a0/stig/commands/tui/_common.py` & `stig-0.9.0a0/stig/commands/tui/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 
 def make_tab_title_widget(text_cropable, text_fixed='', attr_unfocused='', attr_focused=''):
     import urwid
-    from ...utils import strcrop
+    from ...utils.string import strcrop
     from ...tui.main import MAX_TAB_TITLE_WIDTH
     max_width = max(1, MAX_TAB_TITLE_WIDTH-len(text_fixed))
     text_cropped = strcrop(text_cropable, max_width, tail='…')
     return urwid.AttrMap(urwid.Text(''.join((text_cropped, text_fixed))),
                          attr_unfocused, attr_focused)
```

### Comparing `stig-0.8.3a0/stig/commands/tui/file.py` & `stig-0.9.0a0/stig/commands/tui/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..base import file as base
 from . import _mixin as mixin
-from .. import (ExpectedResource, InitCommand)
 
 
 class ListFilesCmd(base.ListFilesCmdbase,
                    mixin.make_request,
                    mixin.select_torrents, mixin.select_files,
                    mixin.create_list_widget):
     provides = {'tui'}
 
-    def make_flist(self, tfilter, ffilter, columns):
-        from ...tui.views.filelist import FileListWidget
+    def make_file_list(self, tfilter, ffilter, columns):
+        from ...tui.views.file_list import FileListWidget
         self.create_list_widget(FileListWidget, theme_name='filelist',
                                 tfilter=tfilter, ffilter=ffilter,
                                 columns=columns,
                                 markable_items=True)
         return True
```

### Comparing `stig-0.8.3a0/stig/commands/tui/torrent.py` & `stig-0.9.0a0/stig/commands/tui/torrent.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,56 +7,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..base import torrent as base
 from . import _mixin as mixin
-from .. import (ExpectedResource, InitCommand)
+from .. import ExpectedResource
 from ._common import make_tab_title_widget
 
 from functools import partial
 
 
 class ListTorrentsCmd(base.ListTorrentsCmdbase,
                       mixin.select_torrents,
                       mixin.create_list_widget):
     provides = {'tui'}
 
-    def make_tlist(self, tfilter, sort, columns):
-        from ...tui.views.torrentlist import TorrentListWidget
+    def make_torrent_list(self, tfilter, sort, columns):
+        from ...tui.views.torrent_list import TorrentListWidget
         self.create_list_widget(TorrentListWidget, theme_name='torrentlist',
                                 tfilter=tfilter, sort=sort, columns=columns,
                                 markable_items=True)
         return True
 
 
 class TorrentSummaryCmd(base.TorrentSummaryCmdbase,
                         mixin.select_torrents, mixin.make_request):
     provides = {'tui'}
     tui = ExpectedResource
 
-    async def display_summary(self, tfilter):
-        from collections import abc
-        if isinstance(tfilter, abc.Sequence):
-            # If tfilter is a bunch of IDs, the user probably has torrents
-            # marked.  But we can't display details of multiple torrents, so we
-            # have to pick one.  The most logical solution is to ignore the
-            # marked torrents and pick the focused one.
-            torrent_id = self.get_focused_torrent_id()
-
-        else:
-            # If an actual filter is specified (e.g. 'summary foo|bar'), use the
-            # first matching torrent (in alphabetical order).
-            torrent = await self.get_torrent(tfilter, keys=('id',))
-            if torrent is None:
-                return False
-            else:
-                torrent_id = torrent['id']
-
+    async def display_summary(self, torrent_id):
         make_titlew = partial(make_tab_title_widget,
                               attr_unfocused='tabs.torrentsummary.unfocused',
                               attr_focused='tabs.torrentsummary.focused')
 
         from ...tui.views.summary import TorrentSummaryWidget
         TorrentSummaryWidget_keymapped = self.tui.keymap.wrap(TorrentSummaryWidget,
                                                               context='torrent')
@@ -85,17 +68,18 @@
 class MoveTorrentsCmd(base.MoveTorrentsCmdbase,
                       mixin.polling_frenzy, mixin.make_request, mixin.select_torrents):
     provides = {'tui'}
 
 
 class RemoveTorrentsCmd(base.RemoveTorrentsCmdbase,
                         mixin.polling_frenzy, mixin.make_request, mixin.select_torrents,
-                        mixin.user_confirmation):
+                        mixin.ask_yes_no):
     provides = {'tui'}
     cmdmgr = ExpectedResource
+    CONFIRMATION_TAB_TITLE = "Removal Confirmation"
 
     async def show_list_of_hits(self, tfilter):
         cmd = 'tab --title %r ls --sort name %s' % (self.CONFIRMATION_TAB_TITLE, tfilter)
         await self.cmdmgr.run_async(cmd)
 
     async def remove_list_of_hits(self):
         cmd = 'tab --close %r --focus left' % self.CONFIRMATION_TAB_TITLE
```

### Comparing `stig-0.8.3a0/stig/commands/utils.py` & `stig-0.9.0a0/stig/commands/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     __delitem__ = _wrap(dict.__delitem__)
     __setitem__ = _wrap(dict.__setitem__)
     clear = _wrap(dict.clear)
     pop = _wrap(dict.pop)
     popitem = _wrap(dict.popitem)
     setdefault = _wrap(dict.setdefault)
-    update =  _wrap(dict.update)
+    update = _wrap(dict.update)
 
 
 from collections import abc
 def listify_args(args):
     """Make list from `args`
 
     Ensure `args` is a string and use split(',') to turn it into a list.  If
```

### Comparing `stig-0.8.3a0/stig/commands/guess_ui.py` & `stig-0.9.0a0/stig/commands/guess_ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
-from ..settings import is_srv_setting
-from ..commands import is_op as is_cmd_op
+from . import is_op as is_cmd_op
+from . import CmdError
 
 
 class UIGuessError(Exception):
     pass
 
-def guess_ui(clicmds, cmdmgr, cfg):
+def guess_ui(clicmds, cmdmgr):
     """Guess desired user interface based on CLI commands
 
     Return 'tui' or 'cli'
     """
     if not clicmds:
         return 'tui'
 
@@ -62,20 +62,32 @@
             debugmsg += 'torrent command - guessing CLI'
             guess = 'cli'
 
         # Some 'set' commands should enforce the tui or cli, other 'set'
         # commands shouldn't care.
         elif cmdline[0] == 'set' and len(cmdline) >= 2 or \
              cmdline[0] == 'reset' and len(cmdline) >= 2:
-            setting = cmdline[1]
-            if setting.startswith('tui.'):
+
+            # Get name of setting
+            i = 1
+            args = list(cmdline[1:])
+            while i < len(args):
+                if args[0][0] == '-':
+                    args.pop(0) ; args.pop(0)
+                i += 1
+            setting = args[0] if args else None
+
+            if setting is None:
+                debugmsg += 'no setting means print list of settings - guessing CLI'
+                guess = 'cli'
+            elif setting.startswith('tui.'):
                 debugmsg += 'TUI setting: %r - guessing TUI' % setting
                 guess = 'tui'
-            elif is_srv_setting(setting, cfg):
-                debugmsg += 'server setting: %r - guessing CLI' % setting
+            elif setting.startswith('srv.'):
+                debugmsg += 'remote setting: %r - guessing CLI' % setting
                 guess = 'cli'
             else:
                 debugmsg += 'other setting: %r - guessing TUI' % setting
                 guess = 'tui'
 
         elif clicmd is not None:
             debugmsg += 'CLI supported - guessing CLI'
```

### Comparing `stig-0.8.3a0/stig/views/trackerlist.py` & `stig-0.9.0a0/stig/views/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,38 +14,41 @@
 from ..logging import make_logger
 log = make_logger(__name__)
 
 from . import ColumnBase
 
 
 COLUMNS = {}
-ALIASES = { 'host'   : 'domain',
-            'u-an'   : 'url-announce',
-            'u-sc'   : 'url-scrape',
-            'e-an'   : 'error-announce',
-            'e-sc'   : 'error-scrape',
-            'l-an'   : 'last-announce',
-            'n-an'   : 'next-announce',
-            'l-sc'   : 'last-scrape',
-            'n-sc'   : 'next-scrape',
-            'dns'    : 'downloads',
-            'status' : 'state' }
+ALIASES = { 'dom'   : 'domain',
+            'an'    : 'url-announce',
+            'sc'    : 'url-scrape',
+            'st'    : 'status',
+            'err'   : 'err',
+            'erran' : 'error-announce',
+            'errsc' : 'error-scrape',
+            'dns'   : 'downloads',
+            'lcs'   : 'leeches',
+            'sds'   : 'seeds',
+            'lan'   : 'last-announce',
+            'nan'   : 'next-announce',
+            'lsc'   : 'last-scrape',
+            'nsc'   : 'next-scrape' }
 
 
-class TorrentName(ColumnBase):
+class Torrent(ColumnBase):
     header = {'left': 'Torrent'}
     align = 'left'
     width = None
     min_width = 7
     may_have_wide_chars = True
 
     def get_value(self):
         return self.data['tname']
 
-COLUMNS['torrent'] = TorrentName
+COLUMNS['torrent'] = Torrent
 
 
 class Tier(ColumnBase):
     header = {'left': 'Tier'}
     align = 'right'
     width = 4
     min_width = 4
@@ -88,24 +91,24 @@
 
     def get_value(self):
         return self.data['url-scrape']
 
 COLUMNS['url-scrape'] = ScrapeURL
 
 
-class State(ColumnBase):
-    header = {'left': 'State'}
+class Status(ColumnBase):
+    header = {'left': 'Status'}
     align = 'right'
     width = 10
     min_width = 5
 
     def get_value(self):
-        return self.data['state']
+        return self.data['status']
 
-COLUMNS['state'] = State
+COLUMNS['status'] = Status
 
 
 class Error(ColumnBase):
     header = {'left': 'Error'}
     align = 'left'
     width = None
     min_width = 20
@@ -145,47 +148,38 @@
     align = 'right'
     width = 9
     min_width = 5
 
     def get_value(self):
         return self.data['count-downloads']
 
-    def get_raw(self):
-        return int(self.get_value())
-
 COLUMNS['downloads'] = Downloads
 
 
 class Leeches(ColumnBase):
     header = {'left': 'Leeches'}
     align = 'right'
     width = 7
     min_width = 5
 
     def get_value(self):
         return self.data['count-leeches']
 
-    def get_raw(self):
-        return int(self.get_value())
-
 COLUMNS['leeches'] = Leeches
 
 
 class Seeds(ColumnBase):
     header = {'left': 'Seeds'}
     align = 'right'
     width = 5
     min_width = 5
 
     def get_value(self):
         return self.data['count-seeds']
 
-    def get_raw(self):
-        return int(self.get_value())
-
 COLUMNS['seeds'] = Seeds
 
 
 class LastAnnounce(ColumnBase):
     header = {'left': 'Last Announce'}
     align = 'right'
     width = 13
```

### Comparing `stig-0.8.3a0/stig/views/summary.py` & `stig-0.9.0a0/stig/views/summary.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,20 +23,19 @@
     else:
         return '%s (%s wanted)' % (t['size-total'].with_unit, t['size-final'].with_unit)
 
 def _size_mr(t):
     return '%d\t%d' % (t['size-total'], t['size-final'])
 
 
-def _rate_limit_hr(direction, t):
-    limit = t['rate-limit-' + direction]
-    return limit.with_unit if hasattr(limit, 'with_unit') else str(limit)
+def _limit_rate_hr(direction, t):
+    return str(t['limit-rate-' + direction])
 
-def _rate_limit_mr(direction, t):
-    limit = t['rate-limit-' + direction]
+def _limit_rate_mr(direction, t):
+    limit = t['limit-rate-' + direction]
     return int(limit) if limit < float('inf') else str(limit)
 
 
 def _file_counts(t):
     files = tuple(t['files'].files)
     all_files = len(files)
     wanted_files = sum(1 for f in files if f['is-wanted'])
@@ -61,18 +60,18 @@
             if t['private'] else
             'no (decentralized peer discovery allowed if enabled globally)')
 
 def _private_mr(t):
     return 'yes' if t['private'] else 'no'
 
 
-def _state_hr(t):
+def _status_hr(t):
     return ', '.join(t['status'])
 
-def _state_mr(t):
+def _status_mr(t):
     return ','.join(t['status'])
 
 
 def _uploaded_hr(t):
     return '%s (%.2f %%)' % (t['size-uploaded'].with_unit, t['%uploaded'])
 
 def _uploaded_mr(t):
@@ -97,15 +96,15 @@
 def _ratio_hr(t):
     ratio = t['ratio']
     if ratio == ratio.INFINITE:
         return 'infinite'
     elif ratio == ratio.NOT_APPLICABLE:
         return 'not applicable'
     else:
-        return '%.4f' % ratio
+        return '%g' % ratio
 _ratio_mr = _ratio_hr
 
 
 def _available_hr(t):
     return '%s (%.2f %%)' % (t['size-available'].with_unit, t['%available'])
 
 def _available_mr(t):
@@ -160,54 +159,120 @@
             self.machine_readable = self.human_readable
         else:
             self.machine_readable = machine_readable
 
 
 SECTIONS = (
     {'title': 'Torrent', 'width': 60, 'items': (
-        Item('Name',       ('name',)),
-        Item('ID',         ('id',)),
-        Item('Hash',       ('hash',)),
-        Item('Size',       ('size-total', 'size-final'), _size_hr, _size_mr),
-        Item('Files',      ('files',), _files_hr, _files_mr),
-        Item('Pieces',     ('count-pieces', 'size-piece'), _pieces_hr, _pieces_mr),
-        Item('Private',    ('private',), _private_hr, _private_mr),
-        Item('Comment',    ('comment',)),
-        Item('Creator',    ('creator',)),
+        Item('Name',
+             needed_keys=('name',)),
+        Item('ID',
+             needed_keys=('id',)),
+        Item('Hash',
+             needed_keys=('hash',)),
+        Item('Size',
+             needed_keys=('size-total', 'size-final'),
+             human_readable=_size_hr,
+             machine_readable=_size_mr),
+        Item('Files',
+             needed_keys=('files',),
+             human_readable=_files_hr,
+             machine_readable=_files_mr),
+        Item('Pieces',
+             needed_keys=('count-pieces', 'size-piece'),
+             human_readable=_pieces_hr,
+             machine_readable=_pieces_mr),
+        Item('Private',
+             needed_keys=('private',),
+             human_readable=_private_hr,
+             machine_readable=_private_mr),
+        Item('Comment',
+             needed_keys=('comment',)),
+        Item('Creator',
+             needed_keys=('creator',)),
     )},
 
     {'title': 'Status', 'width': 51, 'items': (
-        Item('State',      ('status',), _state_hr, _state_mr),
-        Item('Location',   ('path',),),
-        Item('Available',  ('%available', 'size-available'), _available_hr, _available_mr),
-        Item('Downloaded', ('size-downloaded', 'size-left', '%downloaded', 'timespan-eta'), _downloaded_hr, _downloaded_mr),
-        Item('Uploaded',   ('size-uploaded', 'size-total', '%uploaded'), _uploaded_hr, _uploaded_mr),
-        Item('Ratio',      ('ratio',), _ratio_hr, _ratio_mr),
-        Item('Isolated',   ('status',), _isolated_hr, _isolated_mr),
-        Item('Error',      ('error',)),
+        Item('State',
+             needed_keys=('status',),
+             human_readable=_status_hr,
+             machine_readable=_status_mr),
+        Item('Location',
+             needed_keys=('path',),),
+        Item('Available',
+             needed_keys=('%available', 'size-available'),
+             human_readable=_available_hr,
+             machine_readable=_available_mr),
+        Item('Downloaded',
+             needed_keys=('size-downloaded', 'size-left', '%downloaded', 'timespan-eta'),
+             human_readable=_downloaded_hr,
+             machine_readable=_downloaded_mr),
+        Item('Uploaded',
+             needed_keys=('size-uploaded', 'size-total', '%uploaded'),
+             human_readable=_uploaded_hr,
+             machine_readable=_uploaded_mr),
+        Item('Ratio',
+             needed_keys=('ratio',),
+             human_readable=_ratio_hr,
+             machine_readable=_ratio_mr),
+        Item('Isolated',
+             needed_keys=('status',),
+             human_readable=_isolated_hr,
+             machine_readable=_isolated_mr),
+        Item('Error',
+             needed_keys=('error',)),
     )},
 
     {'title': 'Limits', 'width': 24, 'items': (
-        Item('Upload rate',   ('rate-limit-up',), partial(_rate_limit_hr, 'up'), partial(_rate_limit_mr, 'up')),
-        Item('Download rate',   ('rate-limit-down',), partial(_rate_limit_hr, 'down'), partial(_rate_limit_mr, 'down')),
+        Item('Upload rate',
+             needed_keys=('limit-rate-up',),
+             human_readable=partial(_limit_rate_hr, 'up'),
+             machine_readable=partial(_limit_rate_mr, 'up')),
+        Item('Download rate',
+             needed_keys=('limit-rate-down',),
+             human_readable=partial(_limit_rate_hr, 'down'),
+             machine_readable=partial(_limit_rate_mr, 'down')),
     )},
 
     {'title': 'Peers', 'width': 18, 'items': (
-        Item('Seeding',     ('peers-seeding',)),
-        Item('Connected',   ('peers-connected',)),
-        Item('Uploading',   ('peers-uploading',)),
-        Item('Downloading', ('peers-downloading',)),
+        Item('Seeding',
+             needed_keys=('peers-seeding',)),
+        Item('Connected',
+             needed_keys=('peers-connected',)),
+        Item('Uploading',
+             needed_keys=('peers-uploading',)),
+        Item('Downloading',
+             needed_keys=('peers-downloading',)),
     )},
 
     {'title': 'Dates and Times', 'width': 41, 'items': (
-        Item('Created',    ('time-created',),   partial(_date_hr, 'time-created'),   partial(_date_mr, 'time-created')),
-        Item('Added',      ('time-added',),     partial(_date_hr, 'time-added'),     partial(_date_mr, 'time-added')),
-        Item('Started',    ('time-started',),   partial(_date_hr, 'time-started'),   partial(_date_mr, 'time-started')),
-        Item('Completed',  ('time-completed',), partial(_date_hr, 'time-completed'), partial(_date_mr, 'time-completed')),
-        Item('Active',     ('time-activity',),  partial(_date_hr, 'time-activity'),  partial(_date_mr, 'time-activity')),
-
-        Item('Seeding', ('timespan-seeding',),
-             partial(_timespan_hr, 'timespan-seeding'),  partial(_timespan_mr, 'timespan-seeding')),
-        Item('Downloading', ('timespan-downloading',),
-             partial(_timespan_hr, 'timespan-downloading'),  partial(_timespan_mr, 'timespan-downloading')),
+        Item('Created',
+             needed_keys=('time-created',),
+             human_readable=partial(_date_hr, 'time-created'),
+             machine_readable=partial(_date_mr, 'time-created')),
+        Item('Added',
+             needed_keys=('time-added',),
+             human_readable=partial(_date_hr, 'time-added'),
+             machine_readable=partial(_date_mr, 'time-added')),
+        Item('Started',
+             needed_keys=('time-started',),
+             human_readable=partial(_date_hr, 'time-started'),
+             machine_readable=partial(_date_mr, 'time-started')),
+        Item('Completed',
+             needed_keys=('time-completed',),
+             human_readable=partial(_date_hr, 'time-completed'),
+             machine_readable=partial(_date_mr, 'time-completed')),
+        Item('Active',
+             needed_keys=('time-activity',),
+             human_readable=partial(_date_hr, 'time-activity'),
+             machine_readable=partial(_date_mr, 'time-activity')),
+
+        Item('Seeding',
+             needed_keys=('timespan-seeding',),
+             human_readable=partial(_timespan_hr, 'timespan-seeding'),
+             machine_readable=partial(_timespan_mr, 'timespan-seeding')),
+        Item('Downloading',
+             needed_keys=('timespan-downloading',),
+             human_readable=partial(_timespan_hr, 'timespan-downloading'),
+             machine_readable=partial(_timespan_mr, 'timespan-downloading')),
     )},
 )
```

### Comparing `stig-0.8.3a0/stig/views/__init__.py` & `stig-0.9.0a0/stig/views/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 class ColumnBase():
     header = {'left': '', 'right': ''}
     width = None
     min_width = 1
     align = 'right'
+    wrap = 'clip'
     interfaces = ('cli', 'tui')
     may_have_wide_chars = False
 
     def __init__(self, data=None):
         self.data = data if data is not None else {}
         super().__init__()
 
@@ -72,27 +73,35 @@
                 # for citem in items_with_hits:
                 #     log.debug('  %5d hits, last hit: %s: %s',
                 #               citem['hits'],
                 #               strftime('%H:%M:%S', localtime(citem['last_hit'])),
                 #               citem['value'])
         return value
 
+    @classmethod
+    def clearcache(cls):
+        cls._cache.clear()
+
     def get_value(self):
         raise NotImplementedError()
 
-    def get_raw(self):
+    def get_cli_value(self):
+        return self.get_value()
+
+    def get_tui_value(self):
         return self.get_value()
 
+    def get_raw_value(self):
+        value = self.get_value()
+        if isinstance(value, (int, float)) and value < float('inf'):
+            return repr(value)
+        else:
+            return value
+
     def __repr__(self):
-        if self.data:
+        if getattr(self, 'data', None):
             return '<{} {}>'.format(type(self).__name__, self.get_value())
         else:
             return '<{} <UNINITIALIZED>>'.format(type(self).__name__)
 
-
-def _ensure_string_without_unit(value):
-    # We don't want to display the unit (e.g. 'B' or 'b' for file size or
-    # transfer rate) in each cell; it's already displayed in the column header.
-    if hasattr(value, 'str_includes_unit'):
-        return type(value)(value, str_includes_unit=False)
-    else:
-        return value
+def _ensure_hide_unit(value):
+    return type(value)(value, hide_unit=True)
```

### Comparing `stig-0.8.3a0/stig/views/filelist.py` & `stig-0.9.0a0/stig/views/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """TUI and CLI specs for file list columns"""
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
-from . import (ColumnBase, _ensure_string_without_unit)
+from . import (ColumnBase, _ensure_hide_unit)
 
 
 COLUMNS = {}
-ALIASES = { 'dn'   : 'downloaded',
-            'mark' : 'marked',
-            'file' : 'name',
+ALIASES = { 'n'    : 'name',
+            'sz'   : 'size',
+            'dn'   : 'downloaded',
+            '%dn'  : '%downloaded',
             'prio' : 'priority',
-            '%'    : 'progress' }
+            'mark' : 'marked' }
 
 
 class Filename(ColumnBase):
     header = {'left': 'Filename'}
     align = 'left'
     width = None
     min_width = 10
@@ -40,69 +41,60 @@
 
 class Size(ColumnBase):
     header = {'left': 'Size', 'right': '?'}
     width = 6
     min_width = 6
 
     def get_value(self):
-        return _ensure_string_without_unit(self.data['size-total'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return _ensure_hide_unit(self.data['size-total'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = unit
 
 COLUMNS['size'] = Size
 
 
 class Downloaded(ColumnBase):
     header = {'left': 'Dn', 'right': '?'}
     width = 6
     min_width = 6
 
     def get_value(self):
-        return _ensure_string_without_unit(self.data['size-downloaded'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return _ensure_hide_unit(self.data['size-downloaded'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = unit
 
 COLUMNS['downloaded'] = Downloaded
 
 
-class Progress(ColumnBase):
+class PercentDownloaded(ColumnBase):
     header = {'right': '%'}
     width = 4
     min_width = 4
 
     def get_value(self):
-        return _ensure_string_without_unit(self.data['progress'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return _ensure_hide_unit(self.data['%downloaded'])
 
-COLUMNS['progress'] = Progress
+COLUMNS['%downloaded'] = PercentDownloaded
 
 
 class Priority(ColumnBase):
     header = {'left': 'Priority'}
     width = 4
     min_width = 4
     align = 'left'
 
     def get_value(self):
-        val = self.get_raw()
+        val = self.get_raw_value()
         return '' if val == 'normal' else val
 
-    def get_raw(self):
+    def get_raw_value(self):
         return 'off' if self.data['is-wanted'] is False else self.data['priority']
 
 COLUMNS['priority'] = Priority
 
 
 class Marked(ColumnBase):
     interfaces = ('tui',)
@@ -125,15 +117,15 @@
     # Each value recursively summarizes the values of all the TorrentFiles
     # in `tree`.
 
     tfiles = tuple(tree.files)
 
     def sum_size(tfiles, key):
         sizes = tuple(tfile[key] for tfile in tfiles)
-        # Preserve the original type (NumberFloat)
+        # Preserve the original type (Float)
         first_size = sizes[0]
         start_value = type(first_size)(0, unit=first_size.unit, prefix=first_size.prefix)
         return sum(sizes, start_value)
 
     def sum_priority(tfiles):
         if len(set(tfile['priority'] for tfile in tfiles)) == 1:
             return tfiles[0]['priority']
@@ -143,22 +135,22 @@
     data = {'size-downloaded': sum_size(tfiles, 'size-downloaded'),
             'size-total': sum_size(tfiles, 'size-total'),
             'priority': sum_priority(tfiles),
             'is-wanted': True}
 
     data['name'] = create_directory_name(name, filtered_count)
 
-    progress_cls = type(tfiles[0]['progress'])
+    pdownloaded_cls = type(tfiles[0]['%downloaded'])
     try:
-        data['progress'] = progress_cls(data['size-downloaded'] / data['size-total'] * 100)
+        data['%downloaded'] = pdownloaded_cls(data['size-downloaded'] / data['size-total'] * 100)
     except ZeroDivisionError:
-        data['progress'] = progress_cls(0)
+        data['%downloaded'] = pdownloaded_cls(0)
     data['tid'] = tfiles[0]['tid']
+    data['id'] = tuple(tf['id'] for tf in tfiles)
     data['path'] = tree.path
-    data['id'] = frozenset(tf['id'] for tf in tfiles)
     return TorrentFileDirectory(data)
 
 def create_directory_name(name, filtered_count):
     if filtered_count > 0:
         return '%s (%d file%s filtered)' % (name, filtered_count,
                                             '' if filtered_count == 1 else 's')
     else:
```

### Comparing `stig-0.8.3a0/stig/views/torrentlist.py` & `stig-0.9.0a0/stig/views/torrent.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,37 +10,73 @@
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """TUI and CLI specs for torrent list columns"""
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
-from . import (ColumnBase, _ensure_string_without_unit)
+from . import (ColumnBase, _ensure_hide_unit)
 
 COLUMNS = {}
-ALIASES = { '%avail'   : '%available',
-            'avail'    : 'available',
-            'dn'       : 'downloaded',
-            'up'       : 'uploaded',
-            'con'      : 'connections',
-            'mark'     : 'marked',
-            'torrent'  : 'name',
-            '%'        : 'progress',
+ALIASES = { 'mark'     : 'marked',
+            'n'        : 'name',
             'dir'      : 'path',
-            'rdn'      : 'rate-down',
+            'st'       : 'status',
+            'err'      : 'error',
+            'up'       : 'uploaded',
+            'dn'       : 'downloaded',
+            '%dn'      : '%downloaded',
+            'av'       : 'available',
+            '%av'      : '%available',
+            'sz'       : 'size',
+            'prs'      : 'peers',
+            'sds'      : 'seeds',
+            'rto'      : 'ratio',
             'rup'      : 'rate-up',
-            'rldn'     : 'rate-limit-down',
-            'rlup'     : 'rate-limit-up',
-            'state'    : 'status',
+            'rdn'      : 'rate-down',
+            'lrup'     : 'limit-rate-up',
+            'lrdn'     : 'limit-rate-down',
             'trk'      : 'tracker',
-            't-create' : 'time-created',
-            't-add'    : 'time-added',
-            't-start'  : 'time-started',
-            't-active' : 'time-activity',
-            't-comp'   : 'time-completed' }
+            'tcrt'     : 'created',
+            'tadd'     : 'added',
+            'tsta'     : 'started',
+            'tact'     : 'activity',
+            'tcmp'     : 'completed' }
+
+
+class Marked(ColumnBase):
+    interfaces = ('tui',)
+
+COLUMNS['marked'] = Marked
+
+
+class Id(ColumnBase):
+    header = {'left': 'ID'}
+    width = 4
+    needed_keys = ('id',)
+    align = 'right'
+
+    def get_value(self):
+        return self.data['id']
+
+COLUMNS['id'] = Id
+
+
+class Name(ColumnBase):
+    header = {'left': 'Name'}
+    width = None
+    min_width = 5
+    needed_keys = ('name',)
+    align = 'left'
+    may_have_wide_chars = True
+
+    def get_value(self):
+        return self.data['name']
+
+COLUMNS['name'] = Name
 
 
 import os
 PATHSEP = os.sep
 class Path(ColumnBase):
     header = {'left': 'Path'}
     width = None
@@ -97,308 +133,264 @@
         return self._from_cache(self._shorten_path,
                                 self.data['path'].rstrip(PATHSEP),
                                 self.width)
 
 COLUMNS['path'] = Path
 
 
-class Connections(ColumnBase):
-    header = {'left': 'Conn'}
-    width = 5
-    min_width = 5
-    needed_keys = ('peers-connected',)
+class Status(ColumnBase):
+    header = {'left': 'Status'}
+    width = 11
+    min_width = 11
+    needed_keys = ('status',)
 
     def get_value(self):
-        return self.data['peers-connected']
+        return self.data['status'][0]
+
+COLUMNS['status'] = Status
+
+
+class Error(ColumnBase):
+    header = {'left': 'Error'}
+    width = ('weight', 300)
+    min_width = 10
+    needed_keys = ('error',)
+    align = 'left'
 
-    def get_raw(self):
-        return int(self.get_value())
+    def get_value(self):
+        return self.data['error']
 
-COLUMNS['connections'] = Connections
+COLUMNS['error'] = Error
 
 
-class Seeds(ColumnBase):
-    header = {'left': 'Seeds'}
-    width = 5
-    min_width = 5
-    needed_keys = ('peers-seeding',)
+class Uploaded(ColumnBase):
+    header = {'left': 'Up', 'right': '?'}
+    width = 6
+    min_width = 6
+    needed_keys = ('size-uploaded', 'size-downloaded')
 
     def get_value(self):
-        return self.data['peers-seeding']
+        return self._from_cache(_ensure_hide_unit, self.data['size-uploaded'])
 
-    def get_raw(self):
-        return int(self.get_value())
+    @classmethod
+    def set_unit(cls, unit):
+        cls.header['right'] = unit
 
-COLUMNS['seeds'] = Seeds
+COLUMNS['uploaded'] = Uploaded
 
 
-class Progress(ColumnBase):
+class Downloaded(ColumnBase):
+    header = {'left': 'Dn', 'right': '?'}
+    width = 6
+    min_width = 6
+    needed_keys = ('size-downloaded', 'size-final')
+
+    def get_value(self):
+        return self._from_cache(_ensure_hide_unit, self.data['size-downloaded'])
+
+    @classmethod
+    def set_unit(cls, unit):
+        cls.header['right'] = unit
+
+COLUMNS['downloaded'] = Downloaded
+
+
+class PercentDownloaded(ColumnBase):
     header = {'right': '%'}
     width = 4
     min_width = 4
     needed_keys = ('%verified', '%downloaded', '%metadata')
 
     @staticmethod
     def _get_value(verified, downloaded, metadata):
         if 0 < verified < 100:
             value = verified
         elif 0 < metadata < 100:
             value = metadata
         else:
             value = downloaded
-        return _ensure_string_without_unit(value)
+        return _ensure_hide_unit(value)
 
     def get_value(self):
         t = self.data
         return self._from_cache(self._get_value, t['%verified'], t['%downloaded'], t['%metadata'])
 
-    def get_raw(self):
-        return float(self.get_value()) / 100
+COLUMNS['%downloaded'] = PercentDownloaded
 
-COLUMNS['progress'] = Progress
+
+class Available(ColumnBase):
+    header = {'left': 'Avail', 'right': '?'}
+    width = 7
+    min_width = 7
+    needed_keys = ('size-available', 'size-final', 'peers-seeding')
+
+    @staticmethod
+    def _get_value(size_final, size_available, peers_seeding):
+        if peers_seeding > 0:
+            return _ensure_hide_unit(size_final)
+        else:
+            return _ensure_hide_unit(size_available)
+
+    def get_value(self):
+        t = self.data
+        return self._from_cache(self._get_value, t['size-final'], t['size-available'], t['peers-seeding'])
+
+    @classmethod
+    def set_unit(cls, unit):
+        cls.header['right'] = unit
+
+COLUMNS['available'] = Available
 
 
 class PercentAvailable(ColumnBase):
     header = {'left': 'Avail', 'right': '%'}
     width = 7
     min_width = 7
     needed_keys = ('%available', 'peers-seeding')
 
     @staticmethod
     def _get_value(perc_available, peers_seeding):
         if peers_seeding > 0:
-            NumberFloat = type(perc_available)
-            return NumberFloat(100, str_includes_unit=False)
+            return type(perc_available)(100, unit='%', hide_unit=True)
         else:
-            return _ensure_string_without_unit(perc_available)
+            return _ensure_hide_unit(perc_available)
 
     def get_value(self):
         t = self.data
         return self._from_cache(self._get_value, t['%available'], t['peers-seeding'])
 
-    def get_raw(self):
-        return float(self.get_value()) / 100
-
 COLUMNS['%available'] = PercentAvailable
 
 
-class Ratio(ColumnBase):
-    header = {'left': 'Ratio'}
-    width = 5
-    min_width = 5
-    needed_keys = ('ratio',)
-
-    def get_value(self):
-        return self.data['ratio']
-
-    def get_raw(self):
-        return float(self.get_value())
-
-COLUMNS['ratio'] = Ratio
-
-
 class Size(ColumnBase):
     header = {'left': 'Size', 'right': '?'}
     width = 6
     min_width = 6
     needed_keys = ('size-final',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['size-final'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['size-final'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = unit
 
 COLUMNS['size'] = Size
 
 
-class Downloaded(ColumnBase):
-    header = {'left': 'Dn', 'right': '?'}
-    width = 6
-    min_width = 6
-    needed_keys = ('size-downloaded', 'size-final')
+class Peers(ColumnBase):
+    header = {'left': 'Peers'}
+    width = 5
+    min_width = 5
+    needed_keys = ('peers-connected',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['size-downloaded'])
-
-    def get_raw(self):
-        return int(self.get_value())
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header['right'] = unit
+        return self.data['peers-connected']
 
-COLUMNS['downloaded'] = Downloaded
+COLUMNS['peers'] = Peers
 
 
-class Uploaded(ColumnBase):
-    header = {'left': 'Up', 'right': '?'}
-    width = 6
-    min_width = 6
-    needed_keys = ('size-uploaded', 'size-downloaded')
+class Seeds(ColumnBase):
+    header = {'left': 'Seeds'}
+    width = 5
+    min_width = 5
+    needed_keys = ('peers-seeding',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['size-uploaded'])
-
-    def get_raw(self):
-        return int(self.get_value())
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header['right'] = unit
+        return self.data['peers-seeding']
 
-COLUMNS['uploaded'] = Uploaded
+COLUMNS['seeds'] = Seeds
 
 
-class BytesAvailable(ColumnBase):
-    header = {'left': 'Avail', 'right': '?'}
-    width = 7
-    min_width = 7
-    needed_keys = ('size-available', 'size-final', 'peers-seeding')
-
-    @staticmethod
-    def _get_value(size_final, size_available, peers_seeding):
-        if peers_seeding > 0:
-            return _ensure_string_without_unit(size_final)
-        else:
-            return _ensure_string_without_unit(size_available)
+class Ratio(ColumnBase):
+    header = {'left': 'Ratio'}
+    width = 5
+    min_width = 5
+    needed_keys = ('ratio',)
 
     def get_value(self):
-        t = self.data
-        return self._from_cache(self._get_value, t['size-final'], t['size-available'], t['peers-seeding'])
-
-    def get_raw(self):
-        return int(self.get_value())
-
-    @classmethod
-    def set_unit(cls, unit):
-        cls.header['right'] = unit
+        return self.data['ratio']
 
-COLUMNS['available'] = BytesAvailable
+COLUMNS['ratio'] = Ratio
 
 
-class RateDown(ColumnBase):
-    header = {'left': 'Dn', 'right': '?/s'}
+class RateUp(ColumnBase):
+    header = {'left': 'Up', 'right': '?/s'}
     width = 6
     min_width = 6
-    needed_keys = ('rate-down',)
+    needed_keys = ('rate-up',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-down'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['rate-up'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-down'] = RateDown
+COLUMNS['rate-up'] = RateUp
 
 
-class RateUp(ColumnBase):
-    header = {'left': 'Up', 'right': '?/s'}
+class RateDown(ColumnBase):
+    header = {'left': 'Dn', 'right': '?/s'}
     width = 6
     min_width = 6
-    needed_keys = ('rate-up',)
+    needed_keys = ('rate-down',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-up'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['rate-down'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-up'] = RateUp
+COLUMNS['rate-down'] = RateDown
 
 
-class RateLimitDown(ColumnBase):
-    header = {'left': 'LmtDn', 'right': '?/s'}
+class LimitRateUp(ColumnBase):
+    header = {'left': 'LmtUp', 'right': '?/s'}
     width = 9
     min_width = 9
-    needed_keys = ('rate-limit-down',)
+    needed_keys = ('limit-rate-up',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-limit-down'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['limit-rate-up'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-limit-down'] = RateLimitDown
+COLUMNS['limit-rate-up'] = LimitRateUp
 
 
-class RateLimitUp(ColumnBase):
-    header = {'left': 'LmtUp', 'right': '?/s'}
+class LimitRateDown(ColumnBase):
+    header = {'left': 'LmtDn', 'right': '?/s'}
     width = 9
     min_width = 9
-    needed_keys = ('rate-limit-up',)
+    needed_keys = ('limit-rate-down',)
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-limit-up'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['limit-rate-down'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-limit-up'] = RateLimitUp
+COLUMNS['limit-rate-down'] = LimitRateDown
 
 
-class EtaComplete(ColumnBase):
+class Eta(ColumnBase):
     header = {'left': 'ETA'}
     width = 5
     min_width = 9
     needed_keys = ('timespan-eta',)
 
     def get_value(self):
         return self.data['timespan-eta']
 
-    def get_raw(self):
-        return int(self.get_value())
-
-COLUMNS['eta'] = EtaComplete
-
-
-class TorrentName(ColumnBase):
-    header = {'left': 'Name'}
-    width = None
-    min_width = 5
-    needed_keys = ('name',)
-    align = 'left'
-    may_have_wide_chars = True
-
-    def get_value(self):
-        return self.data['name']
-
-COLUMNS['name'] = TorrentName
-
-
-class Status(ColumnBase):
-    header = {'left': 'Status'}
-    width = 11
-    min_width = 11
-    needed_keys = ('status',)
-
-    def get_value(self):
-        return self.data['status'][0]
-
-COLUMNS['status'] = Status
+COLUMNS['eta'] = Eta
 
 
 class Tracker(ColumnBase):
     header = {'left': 'Tracker'}
     width = 10
     min_width = 5
     needed_keys = ('trackers',)
@@ -409,77 +401,55 @@
             return self.data['trackers'][0]['url-announce'].domain
         else:
             return ''
 
 COLUMNS['tracker'] = Tracker
 
 
-class Error(ColumnBase):
-    header = {'left': 'Error'}
-    width = ('weight', 300)
-    min_width = 10
-    needed_keys = ('error',)
-    align = 'left'
-
-    def get_value(self):
-        return self.data['error']
-
-COLUMNS['error'] = Error
-
-
-class Marked(ColumnBase):
-    interfaces = ('tui',)
-
-COLUMNS['marked'] = Marked
-
-
-class TimeBase(ColumnBase):
+class _TimeBase(ColumnBase):
     width = 10
     min_width = 10
 
-    def get_raw(self):
-        return int(self.get_value())
-
-class TimeCreated(TimeBase):
+class Created(_TimeBase):
     header = {'left': 'Created'}
     needed_keys = ('time-created',)
 
     def get_value(self):
         return self.data['time-created']
 
-COLUMNS['time-created'] = TimeCreated
+COLUMNS['created'] = Created
 
-class TimeAdded(TimeBase):
+class Added(_TimeBase):
     header = {'left': 'Added'}
     needed_keys = ('time-added',)
 
     def get_value(self):
         return self.data['time-added']
 
-COLUMNS['time-added'] = TimeAdded
+COLUMNS['added'] = Added
 
-class TimeStarted(TimeBase):
+class Started(_TimeBase):
     header = {'left': 'Started'}
     needed_keys = ('time-started',)
 
     def get_value(self):
         return self.data['time-started']
 
-COLUMNS['time-started'] = TimeStarted
+COLUMNS['started'] = Started
 
-class TimeActivity(TimeBase):
+class Activity(_TimeBase):
     header = {'left': 'Activity'}
     needed_keys = ('time-activity',)
 
     def get_value(self):
         return self.data['time-activity']
 
-COLUMNS['time-activity'] = TimeActivity
+COLUMNS['activity'] = Activity
 
-class TimeCompleted(TimeBase):
+class Completed(_TimeBase):
     header = {'left': 'Completed'}
     needed_keys = ('time-completed',)
 
     def get_value(self):
         return self.data['time-completed']
 
-COLUMNS['time-completed'] = TimeCompleted
+COLUMNS['completed'] = Completed
```

### Comparing `stig-0.8.3a0/stig/views/peerlist.py` & `stig-0.9.0a0/stig/views/peer.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 # http://www.gnu.org/licenses/gpl-3.0.txt
 
 """TUI and CLI specs for peer list columns"""
 
 from ..logging import make_logger
 log = make_logger(__name__)
 
-from . import (ColumnBase, _ensure_string_without_unit)
+from . import (ColumnBase, _ensure_hide_unit)
 
 
 COLUMNS = {}
-ALIASES = { '%'    : 'progress',
-            'rdn'  : 'rate-down',
+ALIASES = { 'cl'   : 'client',
+            'cn'   : 'country',
+            '%dn'  : '%downloaded',
             'rup'  : 'rate-up',
-            'rest' : 'rate-est',
-            'name' : 'torrent' }
+            'rdn'  : 'rate-down',
+            're'   : 'rate-est' }
 
 
-class TorrentName(ColumnBase):
+class Torrent(ColumnBase):
     header = {'left': 'Torrent'}
     align = 'left'
     width = None
     min_width = 7
     may_have_wide_chars = True
 
     def get_value(self):
         return self.data['tname']
 
-COLUMNS['torrent'] = TorrentName
+COLUMNS['torrent'] = Torrent
 
 
 class Client(ColumnBase):
     header = {'left': 'Client'}
     align = 'left'
     width = None
     min_width = 6
@@ -58,108 +59,103 @@
 
     def get_value(self):
         return self.data['country']
 
 COLUMNS['country'] = Country
 
 
-class IPAddress(ColumnBase):
+class IP(ColumnBase):
     header = {'left': 'IP'}
     align = 'right'
-    width = 15
-    min_width = 15
+    width = None
+    min_width = 2
 
     def get_value(self):
         return self.data['ip']
 
-COLUMNS['ip'] = IPAddress
+    def get_cli_value(self):
+        from ..main import localcfg
+        if localcfg['reverse-dns']:
+            from ..client import rdns
+            return rdns.gethostbyaddr(self.data['ip'])
+        return self.data['ip']
+
+COLUMNS['ip'] = IP
 
 
 class Port(ColumnBase):
     header = {'left': 'Port'}
     align = 'right'
     width = 5
     min_width = 5
 
     def get_value(self):
         return self.data['port']
 
 COLUMNS['port'] = Port
 
 
-class Progress(ColumnBase):
+class PercentDownloaded(ColumnBase):
     header = {'right': '%'}
     width = 4
     min_width = 4
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['progress'])
+        return self._from_cache(_ensure_hide_unit, self.data['%downloaded'])
 
-COLUMNS['progress'] = Progress
+COLUMNS['%downloaded'] = PercentDownloaded
 
 
-class RateDown(ColumnBase):
-    header = {'left': 'Dn', 'right': '?/s'}
+class RateUp(ColumnBase):
+    header = {'left': 'Up', 'right': '?/s'}
     width = 6
     min_width = 6
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-down'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['rate-up'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-down'] = RateDown
+COLUMNS['rate-up'] = RateUp
 
 
-class RateUp(ColumnBase):
-    header = {'left': 'Up', 'right': '?/s'}
+class RateDown(ColumnBase):
+    header = {'left': 'Dn', 'right': '?/s'}
     width = 6
     min_width = 6
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-up'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['rate-down'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-up'] = RateUp
+COLUMNS['rate-down'] = RateDown
 
 
 class ETA(ColumnBase):
     header = {'left': 'ETA'}
     width = 5
     min_width = 3
 
     def get_value(self):
         return self.data['eta']
 
-    def get_raw(self):
-        return int(self.get_value())
-
 COLUMNS['eta'] = ETA
 
 
-class EstimatedPeerRate(ColumnBase):
+class RateEst(ColumnBase):
     header = {'left': 'Est', 'right': '?/s'}
     width = 7
     min_width = 7
 
     def get_value(self):
-        return self._from_cache(_ensure_string_without_unit, self.data['rate-est'])
-
-    def get_raw(self):
-        return int(self.get_value())
+        return self._from_cache(_ensure_hide_unit, self.data['rate-est'])
 
     @classmethod
     def set_unit(cls, unit):
         cls.header['right'] = '%s/s' % unit
 
-COLUMNS['rate-est'] = EstimatedPeerRate
+COLUMNS['rate-est'] = RateEst
```

### Comparing `stig-0.8.3a0/stig/helpmgr.py` & `stig-0.9.0a0/stig/helpmgr.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,123 +11,136 @@
 
 """Anything related to the help system that is common between interfaces"""
 
 from .logging import make_logger
 log = make_logger(__name__)
 
 from collections import abc
-from . import (APPNAME, __version__)
-from .utils import (striplines, expandtabs)
+import re
 
-from .cliopts import DESCRIPTIONS
+from . import (__appname__, __version__)
+from .utils import expandtabs
+from .utils.string import striplines
+from .cliopts import DESCRIPTIONS as CLI_DESCRIPTIONS
 
 MAIN_TOPICS = ('commands', 'settings', 'keymap', 'filter', 'rcfile')
 
 ALIASES = {
     'command': 'commands', 'cmds': 'commands', 'cmd': 'commands',
     'setting': 'settings', 'config': 'settings', 'cfg': 'settings',
     'keys': 'keymap', 'keybindings': 'keymap',
     'filters': 'filter', 'filtering': 'filter',
 }
 
 
 def finalize_lines(lines):
     return tuple(
-        striplines(line.format(APPNAME=APPNAME)
+        striplines(line.format(__appname__=__appname__)
                    for line in expandtabs.expand(lines, indent=2))
     )
 
 
 class HelpManager():
     """Provide help texts for CommandManager, Settings and KeyMap objects"""
-    def __init__(self):
-        self._cmdmgr = None
-        self._settings = None
-        self._keymap = None
-
     def find(self, topic=None):
         """Find help topic and return lines"""
         if topic in ALIASES:
             topic = ALIASES[topic]
 
         if topic is None:
             return self.overview
         elif topic in MAIN_TOPICS:
             return getattr(self, topic)
-        elif topic in self._cmdmgr:
+        elif topic in self.cmdmgr:
             return self.command(topic)
-        elif topic in self._settings:
+        elif topic in self.localcfg or topic[4:] in self.remotecfg:
             return self.setting(topic)
-        else:
-            raise ValueError('Unknown help topic: {!r}'.format(topic))
+
+        raise ValueError('Unknown help topic: %r' % topic)
 
     @property
     def overview(self):
         lines = [
-            '{} {}'.format(APPNAME, __version__),
+            '{} {}'.format(__appname__, __version__),
             '',
             'SYNTAX',
-            '\t{APPNAME} [<OPTIONS>] [<COMMAND> ; <COMMAND> ; <COMMAND>...]',
+            '\t{__appname__} [<OPTIONS>] [<COMMAND> ; <COMMAND> ; <COMMAND>...]',
             '',
         ]
 
-        for section,opts in DESCRIPTIONS.items():
+        for section,opts in CLI_DESCRIPTIONS.items():
             lines.append('%s' % section.upper())
             for opts,desc in opts.items():
                 lines.append('\t%s  \t%s' % (opts, desc))
             lines.append('')
 
         lines.append('For more information run:')
         for topic in MAIN_TOPICS:
             lines.append('\thelp %s' % topic)
         return finalize_lines(lines)
 
     @property
     def settings(self):
-        """Must be set to a Settings object; provides a help text"""
-        cfg = self._settings
+        """Return help text for all settings"""
+        localcfg = self.localcfg
+        remotecfg = self.remotecfg
 
         lines = [
             'SETTINGS',
             "\tSettings can be changed with the commands 'set' and 'reset'.",
             '',
             "\tUse an rc file (see 'help rcfile') to specify your custom defaults.",
             '',
         ]
 
-        if cfg is None:
-            lines.append('\tSettings have not been loaded.')
-        else:
-            lines.append('\tAVAILABLE SETTINGS')
-            for name in sorted(cfg.names):
-                lines.append('\t\t' + name + '  \t' + cfg[name].description)
+        lines.append('\tLOCAL SETTINGS')
+        for name in sorted(localcfg):
+            lines.append('\t\t' + name + '  \t' + localcfg.description(name))
+
+        lines += ['']
+
+        lines.append('\tREMOTE SETTINGS')
+        for name in sorted(remotecfg):
+            lines.append('\t\tsrv.' + name + '  \t' + remotecfg.description(name))
         return finalize_lines(lines)
 
-    @settings.setter
-    def settings(self, settings):
-        self._settings = settings
-
     def setting(self, name):
         """Return help text for setting"""
-        v = self._settings[name]
-        lines = ['%s - \t%s' % (v.name, v.description),
-                 '\tValue: \t' + v.string(default=False),
-                 '\tType: \t' + v.typename,
-                 '\tDefault: \t' + v.string(default=True)]
-        if hasattr(v, 'options'):
+        if name in self.localcfg:
+            cfg = self.localcfg
+            key = name
+        elif name[4:] in self.remotecfg:
+            cfg = self.remotecfg
+            key = name[4:]
+        else:
+            raise ValueError('Unknown help topic: %r' % name)
+        value = cfg[key]
+
+        def maybe_quote(value):
+            if isinstance(value, str) and re.match(r'^\s+$', value):
+                return repr(value)
+            else:
+                return str(value)
+
+        lines = ['%s - \t%s' % (name, cfg.description(key)),
+                 '\tValue: \t' + maybe_quote(cfg[key]),
+                 '\tDefault: \t' + maybe_quote(cfg.default(key))]
+
+        if hasattr(value, 'options'):
             opt_strs = []
-            for opt in sorted(v.options):
+            for opt in sorted(value.options):
                 opt_strs.append(str(opt))
-                aliases = [alias for alias,option in v.aliases.items()
+                aliases = [alias for alias,option in value.aliases.items()
                            if option == opt]
                 if aliases:
                     opt_strs[-1] += ' (%s)' % (', '.join(aliases))
             lines.append('\tOptions: \t' + ', '.join(opt_strs))
-        if hasattr(v, 'valuesyntax'):
-            lines.append('\tSyntax: \t{}'.format(v.valuesyntax))
+
+        lines.append('\tSyntax: \t' + cfg.syntax(key))
+
         return finalize_lines(lines)
 
     @property
     def commands(self):
         """Must be set to a CommandManager object; provides a help text"""
         lines = [
             'COMMANDS',
@@ -137,75 +150,69 @@
             "\t\t- \tby binding them to keys (see 'help bind'),",
             ("\t\t- \tby listing them in an rc file (see 'help rcfile') "
              "and loading it with the '--rcfile' option or the 'rc' command."),
             '',
             '\tCHAINING COMMANDS',
             ("\t\tCombining commands with operators makes it possible to run "
              "a command based on the previous command's success."),
-             "",
-             "\t\tAvailable command operators are: ",
-             "\t\t\t&/and \t- \tRun the next command if the previous command succeeded.",
-             "\t\t\t|/or \t- \tRun the next command if the previous command failed.",
-             "\t\t\t;/also \t- \tRun the next command in any case.",
-             "",
-             "\t\tCommand operators must be enclosed by spaces.",
-             "",
+            "",
+            "\t\tAvailable command operators are: ",
+            "\t\t\t&/and \t- \tRun the next command if the previous command succeeded.",
+            "\t\t\t|/or \t- \tRun the next command if the previous command failed.",
+            "\t\t\t;/also \t- \tRun the next command in any case.",
+            "",
+            "\t\tCommand operators must be enclosed by spaces.",
+            "",
             ("\t\tFor example, 'ls foo & ls bar' would list all 'foo' torrents and, "
              "if any where found, continue to list all 'bar' torrents.  "
              "However, 'ls foo | ls bar' would list 'bar' torrents only if there "
              "are no 'foo' torrents."),
             '',
             '\tGUESSING THE USER INTERFACE (CLI/TUI)',
             ("\t\tIf commands are given as command line arguments and neither "
-             "'--tui' nor '--notui' are provided, {APPNAME} tries to guess "
+             "'--tui' nor '--notui' are provided, {__appname__} tries to guess "
              "whether it makes sense to start the TUI or just run the commands "
-             "and exit.  For example, if you run '{APPNAME} stop foo', "
+             "and exit.  For example, if you run '{__appname__} stop foo', "
              "it is reasonable to assume that you want to run 'stop foo' and "
-             "get your shell prompt back.  But if you run '{APPNAME} set srv.url foo.bar', "
+             "get your shell prompt back.  But if you run "
+             "'{__appname__} set connect.host foo.bar', "
              "you probably expect the TUI to pop up."),
-             '',
-             "\t\tThis is how this works basically:",
-             ("\t\t\t- \tWithout CLI commands, the TUI is loaded."),
-             ("\t\t\t- \tCommands in the TORRENT category (see below) prevent the TUI."),
-             ("\t\t\t- \tChanging TUI settings ('(re)set tui.*') enforces the TUI."),
-             ("\t\t\t- \tChanging server settings ('(re)set srv.*') prevents the TUI."),
-             ("\t\t\t- \tCommands that are exclusive to TUI or CLI "
-              "(e.g. 'tab') enforce their interface.  Providing both TUI- "
-              "and CLI-only commands produces an error."),
+            '',
+            "\t\tThis is how this works basically:",
+            ("\t\t\t- \tWithout CLI commands, the TUI is loaded."),
+            ("\t\t\t- \tCommands in the TORRENT category (see below) prevent the TUI."),
+            ("\t\t\t- \tChanging TUI settings ('(re)set tui.*') enforces the TUI."),
+            ("\t\t\t- \tChanging remote settings ('set srv.*') prevents the TUI."),
+            ("\t\t\t- \tCommands that are exclusive to TUI or CLI "
+             "(e.g. 'tab') enforce their interface.  Providing both TUI- "
+             "and CLI-only commands produces an error."),
             '',
         ]
 
-        cmdmgr = self._cmdmgr
-        if cmdmgr is None:
-            lines.append('\tCommands have not been loaded.')
-        else:
-            for category in cmdmgr.categories:
-                lines.append('\t{} COMMANDS'.format(category.upper()))
-
-                # To deduplicate commands with the same name that provide
-                # different interfaces (but should have the same docs), map
-                # command names to commands.
-                cmds = {}
-                for cmd in cmdmgr.all_commands:
-                    if category == cmd.category:
-                        cmds[cmd.name] = cmd
-
-                for cmdname,cmd in sorted(cmds.items()):
-                    lines.append('\t\t{}  \t{}'.format(', '.join((cmd.name,)+cmd.aliases),
-                                                       cmd.description))
-                lines.append('')
+        cmdmgr = self.cmdmgr
+        for category in cmdmgr.categories:
+            lines.append('\t{} COMMANDS'.format(category.upper()))
+
+            # To deduplicate commands with the same name that provide
+            # different interfaces (but should have the same docs), map
+            # command names to commands.
+            cmds = {}
+            for cmd in cmdmgr.all_commands:
+                if category == cmd.category:
+                    cmds[cmd.name] = cmd
+
+            for cmdname,cmd in sorted(cmds.items()):
+                lines.append('\t\t{}  \t{}'.format(', '.join((cmd.name,)+cmd.aliases),
+                                                   cmd.description))
+            lines.append('')
         return finalize_lines(lines)
 
-    @commands.setter
-    def commands(self, cmdmgr):
-        self._cmdmgr = cmdmgr
-
     def command(self, name):
         """Return help text for command"""
-        cmd = self._cmdmgr[name]
+        cmd = self.cmdmgr[name]
 
         def takes_value(argspec):
             if argspec.get('action') in ('store_true', 'store_false', 'store_const'):
                 return False  # Boolean option
             if 'nargs' not in argspec:
                 return True
             nargs = argspec['nargs']
@@ -292,95 +299,91 @@
 
         return finalize_lines(lines)
 
     @property
     def keymap(self):
         """Must be set to a KeyMap object; provides a help text"""
 
-        # Make sure the TUI (and ergo the keymap) is loaded
-        from .tui import main
-
-        km = self._keymap
+        from .tui import main as tui
+        km = tui.keymap
         lines = []
 
-        if km is None:
-            lines.append('Keybindings have not been loaded.')
-        else:
-            def stringify(s):
-                return ' '.join(s) if not isinstance(s, str) else s
+        def stringify(s):
+            return ' '.join(s) if not isinstance(s, str) else s
 
-            for context in sorted(km.contexts, key=lambda c: '' if c is None else c):
-                if context is None:
-                    lines.append('GENERAL KEYBINDINGS')
-                else:
-                    lines.append('{} KEYBINDINGS'.format(context.upper()))
-
-                keymap = ((key, stringify(action)) for key,action in km.map(context))
-
-                # Sort by command
-                from natsort import (natsort_keygen, natsorted, ns)
-                get_cmd = natsort_keygen(key=lambda pair: pair[1], alg=ns.IGNORECASE)
-                for key, action in natsorted(keymap, key=get_cmd):
-                    lines.append('\t{}  \t{}'.format(key, action))
-                lines.append('')
-        return finalize_lines(lines)
+        for context in sorted(km.contexts, key=lambda c: '' if c is None else c):
+            if context is None:
+                lines.append('GENERAL KEYBINDINGS')
+            else:
+                lines.append('{} KEYBINDINGS'.format(context.upper()))
 
-    @keymap.setter
-    def keymap(self, keymap):
-        self._keymap = keymap
+            keymap = ((key, stringify(action)) for key,action in km.map(context))
+
+            # Sort by command
+            from natsort import (natsort_keygen, natsorted, ns)
+            get_cmd = natsort_keygen(key=lambda pair: pair[1], alg=ns.IGNORECASE)
+            for key,action in natsorted(keymap, key=get_cmd):
+                lines.append('\t%s  \t%s' % (key, action))
+            lines.append('')
+        return finalize_lines(lines)
 
     @property
     def filter(self):
         """Provide help text for arguments to TorrentFilter"""
         lines = [
-            'FILTERING TORRENTS, FILES AND PEERS',
-            ('\tCommands that accept FILTER arguments for torrents, files or peers '
-             'are applied to torrents, files or peers that match these arguments.'),
+            'FILTERING TORRENTS, FILES, PEERS, ETC',
+            ('\tCommands that accept FILTER arguments are applied to items '
+             'that match these filters.'),
             '',
             '\tThere are two kinds of filters:',
-            "\t\t- \tBoolean filters stand on their own (e.g. 'downloading')",
-            "\t\t- \tComparative filters match against values (e.g. 'seeds>20').",
+            '\t\t- \tBoolean filters stand on their own (e.g. "downloading")',
+            '\t\t- \tComparative filters need a value (e.g. "seeds>20")',
             '',
-            '\tThe syntax of comparative filters is: [[<FILTER NAME>] <OPERATOR>] <VALUE>',
+            '\tThe syntax of comparative filters is: [[<FILTER NAME>]<OPERATOR>]<VALUE>',
             '',
-            ("\tBesides the standard operators (=, !=, >, <, >=, <=), '~' matches "
-             "if the torrent's value contains VALUE."),
-            "\tExample: 'name~foo' matches all torrents with 'foo' in their name.",
-            '',
-            ("\tIf FILTER NAME is omitted, it defaults to 'name'.  If OPERATOR is "
-             "omitted, it defaults to '~'."),
-            "\tExample: 'foo' is the same as '~foo' is the same as 'name~foo'.",
+            ('\tBesides the usual operators (=, !=, >, <, >=, <=), "~" matches '
+             'if the item\'s value contains VALUE.'),
+            '\tExample: "name~foo" matches all torrents with "foo" in their name.',
+            '',
+            ('\tIf FILTER NAME is omitted, it defaults to "name" for torrents and '
+             'files and "domain" for trackers. Peers don\'t have a default filter.  '
+             'If OPERATOR is omitted, it defaults to "~".'),
+            '\tExample: "foo" is the same as "~foo" is the same as "name~foo".',
             '',
             ('\tSpaces before the filter name are ignored.  If there is a space '
              'between the filter name and the operator, all spaces at the '
              'start and end of VALUE are removed, otherwise they are preserved.  '),
-            "\tExample: 'name = foo  ' matches 'foo'; 'name= foo  ' matches ' foo  '.",
+            '\tExample: "name = foo  " matches "foo"; "name= foo  " matches " foo  ".',
             '',
-            "\tAll filters can be inverted by prepending '!'.",
-            ("\tExample: 'name!=foo' is the same as '!name=foo'; "
-             "'!name!=foo' is the same as 'name=foo'."),
+            '\tAll filters can be inverted by prepending "!" to the filter name.',
+            ('\tExample: "name!=foo" is the same as "!name=foo"; '
+             '"!name!=foo" is the same as "name=foo".'),
             '',
             ('\tWhen matching strings, matches are case-sensitive if VALUE includes '
              'upper-case characters, otherwise it is case-insensitive.'),
             '',
-            ("\tWhen matching numbers, the unit prefixes 'k', 'M', 'G', 'T' and "
-             "their binary counterparts 'Ki', 'Mi', 'Gi', 'Ti' are supported.  "
-             "The case of unit prefixes is ignored."),
-            ("\tExample: 'size>1mi' is the same as 'size>1048576' (1 Mebibyte); "
-             "'size>1m' is the same as 'size>1000000' (1 Megabyte)"),
-            '',
-            ("\tFilters can be combined with the operators '&' (logical AND) "
-             "and '|' (logical OR).  Multiple FILTER arguments are combined with '|'."),
-            "\tExample: 'name=foo paused' is the same as 'name=foo|paused'.",
+            ('\tWhen matching numbers, the unit prefixes "k", "M", "G", "T" and '
+             'their binary counterparts "Ki", "Mi", "Gi", "Ti" are supported.  '
+             'The case of unit prefixes is ignored.'),
+            ('\tExample: "size>1mi" is the same as "size>1048576" (1 Mebibyte); '
+             '"size>1m" is the same as "size>1000000" (1 Megabyte)'),
+            '',
+            ('\tFilters can be combined with the operators "&" (logical AND) '
+             'and "|" (logical OR).  Multiple FILTER arguments are implicitly '
+             'combined with "|".'),
+            '\tExample: "name=foo paused" is the same as "name=foo|paused".',
+            '',
+            ('\tOperators can be escaped with a preceding "\\" to remove their meaning.'),
+            '\tExample: "name=foo\&bar" matches torrents with the name "foo & bar".',
         ]
 
-        from .client.filters.tfilter import SingleTorrentFilter
-        from .client.filters.ffilter import SingleTorrentFileFilter
-        from .client.filters.pfilter import SingleTorrentPeerFilter
-        from .client.filters.trkfilter import SingleTrackerFilter
+        from .client.filters.torrent import SingleTorrentFilter
+        from .client.filters.file import SingleTorrentFileFilter
+        from .client.filters.peer import SingleTorrentPeerFilter
+        from .client.filters.tracker import SingleTrackerFilter
 
         for caption,filt in (('TORRENT FILTERS', SingleTorrentFilter),
                              ('FILE FILTERS', SingleTorrentFileFilter),
                              ('PEER FILTERS', SingleTorrentPeerFilter),
                              ('TRACKER FILTERS', SingleTrackerFilter)):
             lines += ['', '\t%s' % caption]
             lines.append('\t\tBOOLEAN FILTERS')
@@ -393,33 +396,34 @@
         return finalize_lines(lines)
 
     @property
     def rcfile(self):
         """Provide help text for rc file"""
         lines = [
             'RC FILES',
-            ("\tAn rc file contains a list of arbitrary commands, one per line.  "
-             "Lines starting with '#' (more precisely: '\s*#') are ignored."),
-            '',
-            ("\tThe default rc file path is '$XDG_CONFIG_HOME/{APPNAME}/rc', "
-             "where XDG_CONFIG_HOME defaults to '~/.config' if it is not set."),
-            '',
-            ("\tA different path can be provided with the '--rcfile' option.  "
-             "An existing rc file at the default path can be ignored with the "
-             "'--norcfile' option."),
+            ('\tAn rc file is a script that contains a list of arbitrary commands.  '
+             'Commands can span multiple lines by escaping linebreaks with "\\".  '
+             'Lines starting with "#" (more precisely: "\s*#") are ignored.'),
+            '',
+            ('\tThe default rc file path is "$XDG_CONFIG_HOME/{__appname__}/rc", '
+             'where XDG_CONFIG_HOME defaults to "~/.config" if it is not set.'),
+            '',
+            ('\tA different path can be provided with the "--rcfile" option.  '
+             'An existing rc file at the default path can be ignored with the '
+             '"--norcfile" option.'),
             '',
             '\tTo permanently change the default config file, create an alias:',
             '',
             '\t\t$ alias stig="command stig --rcfile ~/.stigrc"',
             '',
-            ("\tTo load an additional rc file after the default one, use the "
-             "'rc' command.  (Note that this will prevent the TUI from being "
-             "loaded unless you provide the '--tui' option.  See the GUESSING "
-             "THE USER INTERFACE section in the 'commands' help for more information.)"),
+            ('\tTo load an additional rc file after the default one, use the '
+             '"rc" command.  (Note that this will prevent the TUI from being '
+             'loaded unless you provide the "--tui" option.  See the GUESSING '
+             'THE USER INTERFACE section in the "commands" help for more information.)'),
             '',
             ('\tCommands in an rc file are called during startup before the '
              'commands given on the command line.'),
             '',
-            ("\tTUI commands (e.g. 'tab' or 'bind') in an rc file are ignored "
-             "in CLI mode."),
+            ('\tTUI commands (e.g. "tab" or "bind") in an rc file are ignored '
+             'in CLI mode.'),
         ]
         return finalize_lines(lines)
```

### Comparing `stig-0.8.3a0/stig/logging.py` & `stig-0.9.0a0/stig/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     # Add new handler that only logs the specified level
     lvlhandler = logging.StreamHandler(stream)
     lvlhandler.addFilter(lambda record: record.levelname == level)
     root_logger.addHandler(lvlhandler)
 
 
 def start_profiling(func, filepath, statistical=True):
-    import pprofile, signal
+    import pprofile
     if statistical:
         prof = pprofile.StatisticalProfile()
     else:
         prof = pprofile.Profile()
 
     def stop_profiling(prof, filepath):
         print('Writing profiling data: %s' % filepath, file=sys.stderr)
```

