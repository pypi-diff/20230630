# Comparing `tmp/reus-1.1.2.tar.gz` & `tmp/reus-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reus-1.1.2.tar", last modified: Fri Jun  2 19:53:16 2023, max compression
+gzip compressed data, was "reus-1.1.3.tar", last modified: Fri Jun 30 20:05:10 2023, max compression
```

## Comparing `reus-1.1.2.tar` & `reus-1.1.3.tar`

### file list

```diff
@@ -1,83 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.213519 reus-1.1.2/
--rw-rw-rw-   0        0        0     1090 2023-06-02 19:45:44.000000 reus-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      616 2023-06-02 19:53:16.212519 reus-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2502 2023-06-02 19:44:43.000000 reus-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.144521 reus-1.1.2/reus/
--rw-rw-rw-   0        0        0      178 2023-06-02 18:52:15.000000 reus-1.1.2/reus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.190519 reus-1.1.2/reus/fbref/
--rw-rw-rw-   0        0        0     1866 2023-06-02 18:51:51.000000 reus-1.1.2/reus/fbref/__init__.py
--rw-rw-rw-   0        0        0     3075 2023-05-10 20:47:21.000000 reus-1.1.2/reus/fbref/fb_league_table.py
--rw-rw-rw-   0        0        0     4728 2023-05-12 15:42:41.000000 reus-1.1.2/reus/fbref/fb_match_data.py
--rw-rw-rw-   0        0        0     5262 2023-05-11 14:36:50.000000 reus-1.1.2/reus/fbref/fb_match_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     6747 2023-05-11 14:36:55.000000 reus-1.1.2/reus/fbref/fb_match_keeper_stats.py
--rw-rw-rw-   0        0        0     2215 2023-05-11 14:38:13.000000 reus-1.1.2/reus/fbref/fb_match_lineups.py
--rw-rw-rw-   0        0        0     8210 2023-05-10 17:45:31.000000 reus-1.1.2/reus/fbref/fb_match_metadata.py
--rw-rw-rw-   0        0        0     4753 2023-05-11 14:41:39.000000 reus-1.1.2/reus/fbref/fb_match_misc_stats.py
--rw-rw-rw-   0        0        0     6569 2023-05-11 14:43:26.000000 reus-1.1.2/reus/fbref/fb_match_passing_stats.py
--rw-rw-rw-   0        0        0     4564 2023-05-11 14:43:49.000000 reus-1.1.2/reus/fbref/fb_match_passing_type_stats.py
--rw-rw-rw-   0        0        0     6370 2023-05-11 14:44:03.000000 reus-1.1.2/reus/fbref/fb_match_possession_stats.py
--rw-rw-rw-   0        0        0     3793 2023-05-10 17:59:04.000000 reus-1.1.2/reus/fbref/fb_match_shots.py
--rw-rw-rw-   0        0        0     3262 2023-05-06 14:21:55.000000 reus-1.1.2/reus/fbref/fb_match_summary.py
--rw-rw-rw-   0        0        0     6007 2023-05-11 14:46:36.000000 reus-1.1.2/reus/fbref/fb_match_summary_stats.py
--rw-rw-rw-   0        0        0     9203 2023-05-10 18:01:05.000000 reus-1.1.2/reus/fbref/fb_match_team_stats.py
--rw-rw-rw-   0        0        0      869 2022-09-09 21:55:47.000000 reus-1.1.2/reus/fbref/fb_match_urls.py
--rw-rw-rw-   0        0        0     3945 2023-06-02 18:46:50.000000 reus-1.1.2/reus/fbref/fb_season_fixture_urls.py
--rw-rw-rw-   0        0        0     3930 2023-06-02 18:46:25.000000 reus-1.1.2/reus/fbref/fb_season_urls.py
--rw-rw-rw-   0        0        0     6142 2023-05-11 14:56:35.000000 reus-1.1.2/reus/fbref/fb_team_advanced_keeper_stats.py
--rw-rw-rw-   0        0        0     4206 2023-05-11 15:22:22.000000 reus-1.1.2/reus/fbref/fb_team_data.py
--rw-rw-rw-   0        0        0     4591 2023-05-11 14:56:06.000000 reus-1.1.2/reus/fbref/fb_team_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     4227 2023-05-11 15:11:09.000000 reus-1.1.2/reus/fbref/fb_team_goal_sca_stats.py
--rw-rw-rw-   0        0        0     4272 2023-05-11 15:11:12.000000 reus-1.1.2/reus/fbref/fb_team_keeper_stats.py
--rw-rw-rw-   0        0        0     4048 2023-05-11 15:11:14.000000 reus-1.1.2/reus/fbref/fb_team_misc_stats.py
--rw-rw-rw-   0        0        0     6112 2023-05-11 15:11:17.000000 reus-1.1.2/reus/fbref/fb_team_passing_stats.py
--rw-rw-rw-   0        0        0     3870 2023-05-11 15:11:20.000000 reus-1.1.2/reus/fbref/fb_team_passing_type_stats.py
--rw-rw-rw-   0        0        0     5794 2023-05-10 20:37:39.000000 reus-1.1.2/reus/fbref/fb_team_player_advanced_keeper_stats.py
--rw-rw-rw-   0        0        0     3149 2023-05-11 15:22:18.000000 reus-1.1.2/reus/fbref/fb_team_player_data.py
--rw-rw-rw-   0        0        0     4366 2023-05-10 19:09:34.000000 reus-1.1.2/reus/fbref/fb_team_player_defensive_actions_stats.py
--rw-rw-rw-   0        0        0     4156 2023-05-10 19:15:49.000000 reus-1.1.2/reus/fbref/fb_team_player_goal_sca_stats.py
--rw-rw-rw-   0        0        0     4123 2023-05-10 19:26:43.000000 reus-1.1.2/reus/fbref/fb_team_player_keeper_stats.py
--rw-rw-rw-   0        0        0     3930 2023-05-10 19:41:13.000000 reus-1.1.2/reus/fbref/fb_team_player_misc_stats.py
--rw-rw-rw-   0        0        0     5823 2023-05-10 19:53:16.000000 reus-1.1.2/reus/fbref/fb_team_player_passing_stats.py
--rw-rw-rw-   0        0        0     3807 2023-05-10 19:57:40.000000 reus-1.1.2/reus/fbref/fb_team_player_passing_type_stats.py
--rw-rw-rw-   0        0        0     4870 2023-05-10 20:06:02.000000 reus-1.1.2/reus/fbref/fb_team_player_playing_time_stats.py
--rw-rw-rw-   0        0        0     5548 2023-05-10 20:08:44.000000 reus-1.1.2/reus/fbref/fb_team_player_possession_stats.py
--rw-rw-rw-   0        0        0     4208 2023-05-10 20:14:01.000000 reus-1.1.2/reus/fbref/fb_team_player_shooting_stats.py
--rw-rw-rw-   0        0        0     5299 2023-05-10 20:28:25.000000 reus-1.1.2/reus/fbref/fb_team_player_summary_stats.py
--rw-rw-rw-   0        0        0     4221 2023-05-10 22:30:19.000000 reus-1.1.2/reus/fbref/fb_team_playing_time_stats.py
--rw-rw-rw-   0        0        0     5696 2023-05-11 15:11:25.000000 reus-1.1.2/reus/fbref/fb_team_possession_stats.py
--rw-rw-rw-   0        0        0     4397 2023-05-11 15:11:27.000000 reus-1.1.2/reus/fbref/fb_team_shooting_stats.py
--rw-rw-rw-   0        0        0     5217 2023-05-11 15:11:28.000000 reus-1.1.2/reus/fbref/fb_team_summary_stats.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.199519 reus-1.1.2/reus/fotmob/
--rw-rw-rw-   0        0        0      557 2023-06-02 18:52:01.000000 reus-1.1.2/reus/fotmob/__init__.py
--rw-rw-rw-   0        0        0     2462 2023-06-02 18:47:27.000000 reus-1.1.2/reus/fotmob/fm_league_ids.py
--rw-rw-rw-   0        0        0     1304 2023-05-15 20:41:21.000000 reus-1.1.2/reus/fotmob/fm_league_matches.py
--rw-rw-rw-   0        0        0     1452 2023-06-02 19:20:19.000000 reus-1.1.2/reus/fotmob/fm_league_table.py
--rw-rw-rw-   0        0        0     2496 2023-06-02 18:43:54.000000 reus-1.1.2/reus/fotmob/fm_league_urls.py
--rw-rw-rw-   0        0        0     1466 2023-05-11 15:29:50.000000 reus-1.1.2/reus/fotmob/fm_leagues.py
--rw-rw-rw-   0        0        0    14981 2023-05-26 15:31:04.000000 reus-1.1.2/reus/fotmob/fm_match_data.py
--rw-rw-rw-   0        0        0     1340 2022-10-16 18:56:44.000000 reus-1.1.2/reus/fotmob/fm_match_ids.py
--rw-rw-rw-   0        0        0     1689 2023-06-02 18:20:03.000000 reus-1.1.2/reus/fotmob/fm_season_stat_leaders.py
--rw-rw-rw-   0        0        0     1738 2023-06-02 18:23:50.000000 reus-1.1.2/reus/fotmob/fm_season_stats.py
--rw-rw-rw-   0        0        0     3768 2023-04-22 23:43:18.000000 reus-1.1.2/reus/fotmob/util.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.209520 reus-1.1.2/reus/transfermarkt/
--rw-rw-rw-   0        0        0      387 2023-06-02 18:52:23.000000 reus-1.1.2/reus/transfermarkt/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-05-12 15:42:49.000000 reus-1.1.2/reus/transfermarkt/tm_player_data.py
--rw-rw-rw-   0        0        0     1660 2023-05-12 16:18:21.000000 reus-1.1.2/reus/transfermarkt/tm_player_injury.py
--rw-rw-rw-   0        0        0     1843 2023-05-12 16:09:28.000000 reus-1.1.2/reus/transfermarkt/tm_player_market_value.py
--rw-rw-rw-   0        0        0     8087 2023-05-12 16:18:15.000000 reus-1.1.2/reus/transfermarkt/tm_player_metadata.py
--rw-rw-rw-   0        0        0     3460 2023-05-12 16:18:09.000000 reus-1.1.2/reus/transfermarkt/tm_player_transfers.py
--rw-rw-rw-   0        0        0     5796 2023-05-12 16:06:28.000000 reus-1.1.2/reus/transfermarkt/tm_team_player_data.py
--rw-rw-rw-   0        0        0     9782 2023-05-12 16:04:59.000000 reus-1.1.2/reus/transfermarkt/tm_team_transfers.py
--rw-rw-rw-   0        0        0     2092 2023-05-12 16:07:09.000000 reus-1.1.2/reus/transfermarkt/util.py
--rw-rw-rw-   0        0        0     1052 2023-06-02 18:48:58.000000 reus-1.1.2/reus/util.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.211520 reus-1.1.2/reus/utils/
--rw-rw-rw-   0        0        0       91 2023-06-02 18:52:20.000000 reus-1.1.2/reus/utils/__init__.py
--rw-rw-rw-   0        0        0     3972 2023-06-02 19:35:18.000000 reus-1.1.2/reus/utils/generate_standings.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:53:16.156519 reus-1.1.2/reus.egg-info/
--rw-rw-rw-   0        0        0      616 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 19:53:16.000000 reus-1.1.2/reus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:53:16.213519 reus-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-06-02 19:53:12.000000 reus-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.653947 reus-1.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-02 19:45:44.000000 reus-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      616 2023-06-30 20:05:10.652949 reus-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2502 2023-06-02 19:44:43.000000 reus-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.558948 reus-1.1.3/reus/
+-rw-rw-rw-   0        0        0      177 2023-06-27 19:12:23.000000 reus-1.1.3/reus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.614949 reus-1.1.3/reus/fbref/
+-rw-rw-rw-   0        0        0     3217 2023-06-27 19:15:12.000000 reus-1.1.3/reus/fbref/__init__.py
+-rw-rw-rw-   0        0        0     3164 2023-06-25 21:03:24.000000 reus-1.1.3/reus/fbref/fb_league_table.py
+-rw-rw-rw-   0        0        0     4728 2023-05-12 15:42:41.000000 reus-1.1.3/reus/fbref/fb_match_data.py
+-rw-rw-rw-   0        0        0     5262 2023-05-11 14:36:50.000000 reus-1.1.3/reus/fbref/fb_match_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     5016 2023-06-26 20:21:47.000000 reus-1.1.3/reus/fbref/fb_match_keeper_stats.py
+-rw-rw-rw-   0        0        0     2215 2023-05-11 14:38:13.000000 reus-1.1.3/reus/fbref/fb_match_lineups.py
+-rw-rw-rw-   0        0        0     8902 2023-06-26 20:31:10.000000 reus-1.1.3/reus/fbref/fb_match_metadata.py
+-rw-rw-rw-   0        0        0     4753 2023-05-11 14:41:39.000000 reus-1.1.3/reus/fbref/fb_match_misc_stats.py
+-rw-rw-rw-   0        0        0     6569 2023-05-11 14:43:26.000000 reus-1.1.3/reus/fbref/fb_match_passing_stats.py
+-rw-rw-rw-   0        0        0     4564 2023-05-11 14:43:49.000000 reus-1.1.3/reus/fbref/fb_match_passing_type_stats.py
+-rw-rw-rw-   0        0        0     6370 2023-05-11 14:44:03.000000 reus-1.1.3/reus/fbref/fb_match_possession_stats.py
+-rw-rw-rw-   0        0        0     3793 2023-05-10 17:59:04.000000 reus-1.1.3/reus/fbref/fb_match_shots.py
+-rw-rw-rw-   0        0        0     3479 2023-06-26 20:50:35.000000 reus-1.1.3/reus/fbref/fb_match_summary.py
+-rw-rw-rw-   0        0        0     6007 2023-05-11 14:46:36.000000 reus-1.1.3/reus/fbref/fb_match_summary_stats.py
+-rw-rw-rw-   0        0        0     8663 2023-06-26 21:30:13.000000 reus-1.1.3/reus/fbref/fb_match_team_stats.py
+-rw-rw-rw-   0        0        0      869 2022-09-09 21:55:47.000000 reus-1.1.3/reus/fbref/fb_match_urls.py
+-rw-rw-rw-   0        0        0     2655 2023-06-26 21:33:18.000000 reus-1.1.3/reus/fbref/fb_season_fixture_urls.py
+-rw-rw-rw-   0        0        0     2640 2023-06-26 21:32:31.000000 reus-1.1.3/reus/fbref/fb_season_urls.py
+-rw-rw-rw-   0        0        0     6142 2023-05-11 14:56:35.000000 reus-1.1.3/reus/fbref/fb_team_advanced_keeper_stats.py
+-rw-rw-rw-   0        0        0     4206 2023-05-11 15:22:22.000000 reus-1.1.3/reus/fbref/fb_team_data.py
+-rw-rw-rw-   0        0        0     4591 2023-05-11 14:56:06.000000 reus-1.1.3/reus/fbref/fb_team_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     4227 2023-05-11 15:11:09.000000 reus-1.1.3/reus/fbref/fb_team_goal_sca_stats.py
+-rw-rw-rw-   0        0        0     4272 2023-05-11 15:11:12.000000 reus-1.1.3/reus/fbref/fb_team_keeper_stats.py
+-rw-rw-rw-   0        0        0     4048 2023-05-11 15:11:14.000000 reus-1.1.3/reus/fbref/fb_team_misc_stats.py
+-rw-rw-rw-   0        0        0     6112 2023-05-11 15:11:17.000000 reus-1.1.3/reus/fbref/fb_team_passing_stats.py
+-rw-rw-rw-   0        0        0     3870 2023-05-11 15:11:20.000000 reus-1.1.3/reus/fbref/fb_team_passing_type_stats.py
+-rw-rw-rw-   0        0        0     5853 2023-06-25 22:53:54.000000 reus-1.1.3/reus/fbref/fb_team_player_advanced_keeper_stats.py
+-rw-rw-rw-   0        0        0     3149 2023-05-11 15:22:18.000000 reus-1.1.3/reus/fbref/fb_team_player_data.py
+-rw-rw-rw-   0        0        0     4425 2023-06-25 22:54:03.000000 reus-1.1.3/reus/fbref/fb_team_player_defensive_actions_stats.py
+-rw-rw-rw-   0        0        0     4215 2023-06-25 22:54:23.000000 reus-1.1.3/reus/fbref/fb_team_player_goal_sca_stats.py
+-rw-rw-rw-   0        0        0     4182 2023-06-25 22:54:19.000000 reus-1.1.3/reus/fbref/fb_team_player_keeper_stats.py
+-rw-rw-rw-   0        0        0     3989 2023-06-25 22:54:15.000000 reus-1.1.3/reus/fbref/fb_team_player_misc_stats.py
+-rw-rw-rw-   0        0        0     5882 2023-06-25 22:54:09.000000 reus-1.1.3/reus/fbref/fb_team_player_passing_stats.py
+-rw-rw-rw-   0        0        0     3866 2023-06-25 22:54:54.000000 reus-1.1.3/reus/fbref/fb_team_player_passing_type_stats.py
+-rw-rw-rw-   0        0        0     4929 2023-06-25 22:54:49.000000 reus-1.1.3/reus/fbref/fb_team_player_playing_time_stats.py
+-rw-rw-rw-   0        0        0     5607 2023-06-25 22:54:37.000000 reus-1.1.3/reus/fbref/fb_team_player_possession_stats.py
+-rw-rw-rw-   0        0        0     4267 2023-06-25 22:54:30.000000 reus-1.1.3/reus/fbref/fb_team_player_shooting_stats.py
+-rw-rw-rw-   0        0        0     5358 2023-06-25 22:54:44.000000 reus-1.1.3/reus/fbref/fb_team_player_summary_stats.py
+-rw-rw-rw-   0        0        0     4221 2023-05-10 22:30:19.000000 reus-1.1.3/reus/fbref/fb_team_playing_time_stats.py
+-rw-rw-rw-   0        0        0     5696 2023-05-11 15:11:25.000000 reus-1.1.3/reus/fbref/fb_team_possession_stats.py
+-rw-rw-rw-   0        0        0     4397 2023-05-11 15:11:27.000000 reus-1.1.3/reus/fbref/fb_team_shooting_stats.py
+-rw-rw-rw-   0        0        0     5217 2023-05-11 15:11:28.000000 reus-1.1.3/reus/fbref/fb_team_summary_stats.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.622947 reus-1.1.3/reus/fotmob/
+-rw-rw-rw-   0        0        0      418 2023-06-27 19:12:29.000000 reus-1.1.3/reus/fotmob/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-06-26 16:25:15.000000 reus-1.1.3/reus/fotmob/fm_league_matches.py
+-rw-rw-rw-   0        0        0     1616 2023-06-26 16:44:31.000000 reus-1.1.3/reus/fotmob/fm_league_table.py
+-rw-rw-rw-   0        0        0     3013 2023-06-26 16:09:49.000000 reus-1.1.3/reus/fotmob/fm_leagues.py
+-rw-rw-rw-   0        0        0    15386 2023-06-27 16:27:05.000000 reus-1.1.3/reus/fotmob/fm_match_data.py
+-rw-rw-rw-   0        0        0     1338 2023-06-30 17:29:48.000000 reus-1.1.3/reus/fotmob/fm_match_ids.py
+-rw-rw-rw-   0        0        0     1866 2023-06-26 17:19:08.000000 reus-1.1.3/reus/fotmob/fm_season_stat_leaders.py
+-rw-rw-rw-   0        0        0     1969 2023-06-26 17:19:04.000000 reus-1.1.3/reus/fotmob/fm_season_stats.py
+-rw-rw-rw-   0        0        0     4292 2023-06-25 20:45:57.000000 reus-1.1.3/reus/fotmob/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.631948 reus-1.1.3/reus/transfermarkt/
+-rw-rw-rw-   0        0        0      460 2023-06-27 19:12:26.000000 reus-1.1.3/reus/transfermarkt/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-05-12 15:42:49.000000 reus-1.1.3/reus/transfermarkt/tm_player_data.py
+-rw-rw-rw-   0        0        0     1660 2023-05-12 16:18:21.000000 reus-1.1.3/reus/transfermarkt/tm_player_injury.py
+-rw-rw-rw-   0        0        0     1843 2023-05-12 16:09:28.000000 reus-1.1.3/reus/transfermarkt/tm_player_market_value.py
+-rw-rw-rw-   0        0        0     6490 2023-06-27 19:05:48.000000 reus-1.1.3/reus/transfermarkt/tm_player_metadata.py
+-rw-rw-rw-   0        0        0     3465 2023-06-26 17:45:35.000000 reus-1.1.3/reus/transfermarkt/tm_player_transfers.py
+-rw-rw-rw-   0        0        0     6004 2023-06-27 16:49:32.000000 reus-1.1.3/reus/transfermarkt/tm_team_player_data.py
+-rw-rw-rw-   0        0        0     9026 2023-06-27 17:42:12.000000 reus-1.1.3/reus/transfermarkt/tm_team_transfers.py
+-rw-rw-rw-   0        0        0     2092 2023-05-12 16:07:09.000000 reus-1.1.3/reus/transfermarkt/util.py
+-rw-rw-rw-   0        0        0     1251 2023-06-27 19:18:33.000000 reus-1.1.3/reus/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.632949 reus-1.1.3/reus/utils/
+-rw-rw-rw-   0        0        0       66 2023-06-26 16:11:19.000000 reus-1.1.3/reus/utils/__init__.py
+-rw-rw-rw-   0        0        0     3972 2023-06-02 19:35:18.000000 reus-1.1.3/reus/utils/generate_standings.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.576947 reus-1.1.3/reus.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-06-30 20:05:10.000000 reus-1.1.3/reus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-30 20:05:10.000000 reus-1.1.3/reus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 20:05:10.000000 reus-1.1.3/reus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-30 20:05:10.000000 reus-1.1.3/reus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-30 20:05:10.000000 reus-1.1.3/reus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 20:05:10.653947 reus-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      883 2023-06-25 20:42:32.000000 reus-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.633948 reus-1.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-25 23:31:32.000000 reus-1.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.640948 reus-1.1.3/tests/fbref/
+-rw-rw-rw-   0        0        0        0 2023-06-25 23:31:35.000000 reus-1.1.3/tests/fbref/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-06-26 16:57:01.000000 reus-1.1.3/tests/fbref/test_fb_league_table.py
+-rw-rw-rw-   0        0        0     2639 2023-06-26 20:11:02.000000 reus-1.1.3/tests/fbref/test_fb_match_data.py
+-rw-rw-rw-   0        0        0      744 2023-06-26 16:56:48.000000 reus-1.1.3/tests/fbref/test_fb_match_urls.py
+-rw-rw-rw-   0        0        0      886 2023-06-25 23:32:49.000000 reus-1.1.3/tests/fbref/test_fb_season_fixture_urls.py
+-rw-rw-rw-   0        0        0      609 2023-06-25 23:37:33.000000 reus-1.1.3/tests/fbref/test_fb_season_urls.py
+-rw-rw-rw-   0        0        0     2771 2023-06-25 23:39:15.000000 reus-1.1.3/tests/fbref/test_fb_team_data.py
+-rw-rw-rw-   0        0        0     1724 2023-06-25 23:38:23.000000 reus-1.1.3/tests/fbref/test_fb_team_player_data.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.647948 reus-1.1.3/tests/fotmob/
+-rw-rw-rw-   0        0        0        0 2023-06-25 23:48:07.000000 reus-1.1.3/tests/fotmob/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-06-26 16:43:27.000000 reus-1.1.3/tests/fotmob/test_fm_league_matches.py
+-rw-rw-rw-   0        0        0     1951 2023-06-26 16:58:06.000000 reus-1.1.3/tests/fotmob/test_fm_league_table.py
+-rw-rw-rw-   0        0        0     1400 2023-06-26 16:04:59.000000 reus-1.1.3/tests/fotmob/test_fm_leagues.py
+-rw-rw-rw-   0        0        0     1374 2023-06-27 15:04:16.000000 reus-1.1.3/tests/fotmob/test_fm_match_data.py
+-rw-rw-rw-   0        0        0      623 2023-06-26 17:24:06.000000 reus-1.1.3/tests/fotmob/test_fm_match_ids.py
+-rw-rw-rw-   0        0        0     1833 2023-06-26 17:15:32.000000 reus-1.1.3/tests/fotmob/test_fm_season_stat_leaders.py
+-rw-rw-rw-   0        0        0      864 2023-06-26 17:18:56.000000 reus-1.1.3/tests/fotmob/test_fm_season_stats.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:05:10.651947 reus-1.1.3/tests/transfermarkt/
+-rw-rw-rw-   0        0        0        0 2023-06-25 23:48:07.000000 reus-1.1.3/tests/transfermarkt/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-06-26 17:53:31.000000 reus-1.1.3/tests/transfermarkt/test_tm_player_data.py
+-rw-rw-rw-   0        0        0      680 2023-06-26 17:54:34.000000 reus-1.1.3/tests/transfermarkt/test_tm_player_injury.py
+-rw-rw-rw-   0        0        0      830 2023-06-30 19:41:20.000000 reus-1.1.3/tests/transfermarkt/test_tm_team_player_data.py
+-rw-rw-rw-   0        0        0     1690 2023-06-30 19:59:59.000000 reus-1.1.3/tests/transfermarkt/test_tm_team_transfers.py
```

### Comparing `reus-1.1.2/LICENSE` & `reus-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/PKG-INFO` & `reus-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reus
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package that allows you to soccer information
 Home-page: https://github.com/ian-shepherd/reus
 Author: Ian Shepherd
 License: UNKNOWN
 Keywords: python,fbref,fotmob,transfermarkt,soccer,football
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reus-1.1.2/README.md` & `reus-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_league_table.py` & `reus-1.1.3/reus/fbref/fb_league_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,18 +42,21 @@
         try:
             xG = row.find("td", {"data-stat": "xg_for"}).text
             xGA = row.find("td", {"data-stat": "xg_against"}).text
             xGD = float(row.find("td", {"data-stat": "xg_diff"}).text)
             xGDp90 = float(row.find("td", {"data-stat": "xg_diff_per90"}).text)
         except AttributeError:
             xG = xGA = xGD = xGDp90 = None
-        last_5_ = row.find("td", {"data-stat": "last_5"})
-        last_5 = ""
-        for t in last_5_.find_all("div", {"class": "poptip"}):
-            last_5 += t.text
+        try:
+            last_5_ = row.find("td", {"data-stat": "last_5"})
+            last_5 = ""
+            for t in last_5_.find_all("div", {"class": "poptip"}):
+                last_5 += t.text
+        except AttributeError:
+            last_5 = None
         avg_attendance = row.find("td", {"data-stat": "attendance_per_g"}).text
         top_scorer = row.find("td", {"data-stat": "top_team_scorers"}).text
         goalkeeper = row.find("td", {"data-stat": "top_keeper"}).text
         notes = row.find("td", {"data-stat": "notes"}).text
 
         # generate dictionary for each player
         mydict = {
```

### Comparing `reus-1.1.2/reus/fbref/fb_match_data.py` & `reus-1.1.3/reus/fbref/fb_match_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_defensive_actions_stats.py` & `reus-1.1.3/reus/fbref/fb_match_defensive_actions_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_keeper_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_possession_stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,143 @@
-from .fb_match_metadata import fb_match_metadata
 from ..util import get_page_soup
 
 
-def fb_match_keeper_stats(pageSoup=None, url: str = None) -> tuple:
-    """Extracts goalkeeping stats for each keeper in a given match that includes advanced data
+def fb_team_player_possession_stats(pageSoup=None, url: str = None) -> list:
+    """Extracts possession stats for each player in a given team
 
     Args:
-        pageSoup (bs4, optional): bs4 object of a match. Defaults to None.
-        url (str, optional): path of fbref match page. Defaults to None.
+        pageSoup (bs4, optional): bs4 object of a team. Defaults to None.
+        url (str, optional): path of fbref team page. Defaults to None.
 
     Returns:
-        tuple: goalkeeping stats for home and away team
-            list: goalkeeping stats for home team players
-            list: goalkeeping stats for away team players
+        list: possession stats for each player
     """
 
     assert (
         pageSoup is not None or url is not None
     ), "Either pageSoup or url must be provided"
 
+    assert (
+        pageSoup is not None or url is not None
+    ), "Either pageSoup or url must be provided"
+
     if pageSoup is None:
         pageSoup = get_page_soup(url)
 
-    # Get team ids
-    metadata = fb_match_metadata(pageSoup)[0]
-    id_x = metadata.get("id_x")
-    id_y = metadata.get("id_y")
-
-    # Loop through both teams
-    for team_id in [id_x, id_y]:
-        # generate empty list for each team
-        mylist = []
-        # generate html id
-        id_ = "keeper_stats_" + team_id
-
-        # find goalkeeping object
-        stats_keeper = pageSoup.find("table", {"id": id_})
-        stats_keeper = stats_keeper.find_all("tr")
-
-        # iterate through each keeper and store metrics
-        for row in stats_keeper[2:]:
-            th = row.find("th")
-
-            # general
-            try:
-                name = th.text
-            except AttributeError:
-                name = th["csk"]
-
-            player_id = th.find("a", href=True)["href"].split("/")[3]
-            nation = row.find("td", {"data-stat": "nationality"}).text
-            age = row.find("td", {"data-stat": "age"}).text.split("-")
-            try:
-                age = int(age[0]) + int(age[1]) / 365
-            except ValueError:
-                age = None
-            minutes = row.find("td", {"data-stat": "minutes"}).text
-
-            # shot stopping
-            shots_against = row.find(
-                "td", {"data-stat": "gk_shots_on_target_against"}
-            ).text
-            goals_allowed = row.find("td", {"data-stat": "gk_goals_against"}).text
-            saves = row.find("td", {"data-stat": "gk_saves"}).text
-            save_pct = row.find("td", {"data-stat": "gk_save_pct"}).text
-            if save_pct == "":
-                save_pct = None
-            psxg = row.find("td", {"data-stat": "gk_psxg"}).text
-
-            # launched
-            launched_completed = row.find(
-                "td", {"data-stat": "gk_passes_completed_launched"}
-            ).text
-            launched_attempted = row.find(
-                "td", {"data-stat": "gk_passes_launched"}
-            ).text
-            launched_accuracy = row.find(
-                "td", {"data-stat": "gk_passes_pct_launched"}
-            ).text
-            if launched_accuracy == "":
-                launched_accuracy = None
-
-            # passes
-            passes_attempted = row.find("td", {"data-stat": "gk_passes"}).text
-            if passes_attempted == "":
-                passes_attempted = None
-            throws_attempted = row.find("td", {"data-stat": "gk_passes_throws"}).text
-            if throws_attempted == "":
-                throws_attempted = None
-            pct_launched = row.find("td", {"data-stat": "gk_pct_passes_launched"}).text
-            if pct_launched == "":
-                pct_launched = None
-            passes_avg_length = row.find(
-                "td", {"data-stat": "gk_passes_length_avg"}
-            ).text
-            if passes_avg_length == "":
-                passes_avg_length = None
-
-            # goal kicks
-            gk_attempted = row.find("td", {"data-stat": "gk_goal_kicks"}).text
-            if gk_attempted == "":
-                gk_attempted = None
-            gk_pct_launched = row.find(
-                "td", {"data-stat": "gk_pct_goal_kicks_launched"}
-            ).text
-            if gk_pct_launched == "":
-                gk_pct_launched = None
-            gk_avg_length = row.find(
-                "td", {"data-stat": "gk_goal_kick_length_avg"}
-            ).text
-            if gk_avg_length == "":
-                gk_avg_length = None
-
-            # crosses
-            crosses_faced = row.find("td", {"data-stat": "gk_crosses"}).text
-            if crosses_faced == "":
-                crosses_faced = None
-            crosses_stopped = row.find("td", {"data-stat": "gk_crosses_stopped"}).text
-            if crosses_stopped == "":
-                crosses_stopped = None
-            crosses_stopped_pct = row.find(
-                "td", {"data-stat": "gk_crosses_stopped_pct"}
-            ).text
-            if crosses_stopped_pct == "":
-                crosses_stopped_pct = None
-
-            # sweeper
-            defensive_actions = row.find(
-                "td", {"data-stat": "gk_def_actions_outside_pen_area"}
-            ).text
-            defensive_actions_avg_distance = row.find(
-                "td", {"data-stat": "gk_avg_distance_def_actions"}
-            ).text
-
-            # generate dictionary for team
-            mydict = {
-                "player_id": player_id,
-                "name": name,
-                "nation": nation,
-                "age": age,
-                "minutes": minutes,
-                "shots_against": shots_against,
-                "goals_allowed": goals_allowed,
-                "saves": saves,
-                "save_pct": save_pct,
-                "psxg": psxg,
-                "launched_completed": launched_completed,
-                "launched_attempted": launched_attempted,
-                "launched_accuracy": launched_accuracy,
-                "passes_attempted": passes_attempted,
-                "throws_attempted": throws_attempted,
-                "pct_launched": pct_launched,
-                "passes_avg_length": passes_avg_length,
-                "gk_attempted": gk_attempted,
-                "gk_pct_launched": gk_pct_launched,
-                "gk_avg_length": gk_avg_length,
-                "crosses_faced": crosses_faced,
-                "crosses_stopped": crosses_stopped,
-                "crosses_stopped_pct": crosses_stopped_pct,
-                "defensive_actions": defensive_actions,
-                "defensive_actions_avg_distance": defensive_actions_avg_distance,
-            }
-
-            # add to empty list
-            mylist.append(mydict)
-
-        # assign list to appropriate team
-        if team_id == id_x:
-            keeper_stats_x = mylist.copy()
-        else:
-            keeper_stats_y = mylist.copy()
+    # Find table object
+    div = pageSoup.find("div", {"id": "all_stats_possession"})
+    if div is None:
+        return None
+
+    table = div.find("table")
+    tbody = table.find("tbody")
+    rows = tbody.find_all("tr")
+
+    # Generate empty list
+    mylist = []
+
+    # iterate through each player and store attributes
+    for row in rows:
+        # general
+        th = row.find("th")
+        try:
+            name = th.text
+        except AttributeError:
+            name = th["csk"]
+        player_id = th.find("a", href=True)["href"].split("/")[3]
+        nation = row.find("td", {"data-stat": "nationality"}).text
+        position = row.find("td", {"data-stat": "position"}).text
+        age = row.find("td", {"data-stat": "age"}).text.split("-")
+        try:
+            age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
+        except ValueError:
+            age = None
+        minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
+
+        # touches
+        touches = row.find("td", {"data-stat": "touches"}).text
+        touches_def_pen_area = row.find(
+            "td", {"data-stat": "touches_def_pen_area"}
+        ).text
+        touches_def_3rd = row.find("td", {"data-stat": "touches_def_3rd"}).text
+        touches_mid_3rd = row.find("td", {"data-stat": "touches_mid_3rd"}).text
+        touches_att_3rd = row.find("td", {"data-stat": "touches_att_3rd"}).text
+        touches_att_pen_area = row.find(
+            "td", {"data-stat": "touches_att_pen_area"}
+        ).text
+        touches_live = row.find("td", {"data-stat": "touches_live_ball"}).text
+
+        # take ons
+        dribble_attempt = row.find("td", {"data-stat": "take_ons"}).text
+        dribble_success = row.find("td", {"data-stat": "take_ons_won"}).text
+        dribble_success_pct = row.find("td", {"data-stat": "take_ons_won_pct"}).text
+        if dribble_success_pct == "":
+            dribble_success_pct = None
+        dribble_tackled = row.find("td", {"data-stat": "take_ons_tackled"}).text
+        dribble_tackled_pct = row.find("td", {"data-stat": "take_ons_tackled_pct"}).text
+
+        # carries
+        carries = row.find("td", {"data-stat": "carries"}).text
+        carries_total_distance = row.find("td", {"data-stat": "carries_distance"}).text
+        carries_progressive_distance = row.find(
+            "td", {"data-stat": "carries_progressive_distance"}
+        ).text
+        progressive_carries = row.find("td", {"data-stat": "progressive_carries"}).text
+        carries_into_final_third = row.find(
+            "td", {"data-stat": "carries_into_final_third"}
+        ).text
+        carries_into_penalty_area = row.find(
+            "td", {"data-stat": "carries_into_penalty_area"}
+        ).text
+        miscontrols = row.find("td", {"data-stat": "miscontrols"}).text
+        dispossessed = row.find("td", {"data-stat": "dispossessed"}).text
+
+        # receiving
+        passes_received = row.find("td", {"data-stat": "passes_received"}).text
+        progressive_passes_received = row.find(
+            "td", {"data-stat": "progressive_passes_received"}
+        ).text
+
+        # match logs
+        match_logs = row.find("td", {"data-stat": "matches"}).find("a", href=True)[
+            "href"
+        ]
+
+        # generate dictionary for player
+        mydict = {
+            "player_id": player_id,
+            "name": name,
+            "nation": nation,
+            "position": position,
+            "age": age,
+            "90s": minutes_90,
+            "touches": touches,
+            "touches_def_pen_area": touches_def_pen_area,
+            "touches_def_3rd": touches_def_3rd,
+            "touches_mid_3rd": touches_mid_3rd,
+            "touches_att_3rd": touches_att_3rd,
+            "touches_att_pen_area": touches_att_pen_area,
+            "touches_live": touches_live,
+            "dribble_attempt": dribble_attempt,
+            "dribble_success": dribble_success,
+            "dribble_success_pct": dribble_success_pct,
+            "dribble_tackled": dribble_tackled,
+            "dribble_tackled_pct": dribble_tackled_pct,
+            "carries": carries,
+            "carry_total_distance": carries_total_distance,
+            "carry_progressive_distance": carries_progressive_distance,
+            "progressive_carries": progressive_carries,
+            "carries_into_final_third": carries_into_final_third,
+            "carries_into_penalty_area": carries_into_penalty_area,
+            "miscontrols": miscontrols,
+            "dispossessed": dispossessed,
+            "passes_received": passes_received,
+            "progressive_passes_received": progressive_passes_received,
+            "match_logs": match_logs,
+        }
+
+        # add to empty list
+        mylist.append(mydict)
 
-    return keeper_stats_x, keeper_stats_y
+    return mylist
```

### Comparing `reus-1.1.2/reus/fbref/fb_match_lineups.py` & `reus-1.1.3/reus/fbref/fb_match_lineups.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_metadata.py` & `reus-1.1.3/reus/fbref/fb_match_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 import re
 from ..util import get_page_soup
 
 
-def fb_match_metadata(pageSoup=None, url: str = None) -> tuple:
-    """Extracts general information (teams, managers, captains, date, time, venue, attendance, score, xG) for a given match
-
-    Args:
-        pageSoup (bs4, optional): bs4 object of a match. Defaults to None.
-        url (str, optional): path of fbref match page. Defaults to None.
-
-    Returns:
-        tuple: metadata and officials
-            dict: metadata information
-            dict: match officials
-    """
-
-    assert (
-        pageSoup is not None or url is not None
-    ), "Either pageSoup or url must be provided"
-
-    if pageSoup is None:
-        pageSoup = get_page_soup(url)
-
-    # Extract url
+def _extract_url(pageSoup):
     url = pageSoup.find("meta", {"property": "og:url"})["content"]
     url = url.replace("https://fbref.com", "")
     match_id = url.split("/")[3]
+    return url, match_id
+
 
+def _extract_teams(pageSoup):
     # Find scorebox object
     scorebox = pageSoup.find("div", {"class": "scorebox"})
     # teams = scorebox.find_all("div", {"itemprop": "performer"})
     teams = scorebox.find_all("strong")
 
-    # extract team id and name
-    team_idx = []
-    for i in range(len(teams)):
-        if teams[i].find("a", href=True) is not None and "squad" in teams[i].find(
-            "a", href=True
-        ).get("href"):
-            team_idx.append(i)
-    id_x = teams[team_idx[0]].find("a", href=True)["href"].split("/")[3]
-    id_y = teams[team_idx[1]].find("a", href=True)["href"].split("/")[3]
+    team_idx = [
+        i
+        for i, team in enumerate(teams)
+        if team.find("a", href=True)
+        and "squad" in team.find("a", href=True).get("href")
+    ]
+
     team_x = teams[team_idx[0]].find("a", href=True).text
     team_y = teams[team_idx[1]].find("a", href=True).text
 
-    # extract scores
+    id_x = teams[team_idx[0]].find("a", href=True)["href"].split("/")[3]
+    id_y = teams[team_idx[1]].find("a", href=True)["href"].split("/")[3]
+
+    return id_x, team_x, id_y, team_y
+
+
+def _extract_scores(pageSoup):
     scores = pageSoup.find_all("div", {"class": "scores"})
     score_x = scores[0].find("div", {"class": "score"}).text
     score_y = scores[1].find("div", {"class": "score"}).text
+
     # error handling for non-xG
     try:
         xg_x = scores[0].find("div", {"class": "score_xg"}).text
     except AttributeError:
         xg_x = None
     try:
         xg_y = scores[1].find("div", {"class": "score_xg"}).text
     except AttributeError:
         xg_y = None
 
-    # extract managers and captains
+    return score_x, score_y, xg_x, xg_y
+
+
+def _extract_managers_captains(pageSoup):
     managers = pageSoup.find_all("div", {"class": "datapoint"})
+
     manager_x = None
     manager_y = None
     captain_x = None
     captain_y = None
     captain_url_x = None
     captain_url_y = None
     captain_id_x = None
@@ -118,14 +110,60 @@
         captain_x = managers[0].find("a", href=True).text
         captain_y = managers[1].find("a", href=True).text
         captain_url_x = managers[0].find("a", href=True)["href"]
         captain_url_y = managers[1].find("a", href=True)["href"]
         captain_id_x = captain_url_x.split("/")[3]
         captain_id_y = captain_url_y.split("/")[3]
 
+    return (
+        manager_x,
+        manager_y,
+        captain_x,
+        captain_y,
+        captain_url_x,
+        captain_url_y,
+        captain_id_x,
+        captain_id_y,
+    )
+
+
+def fb_match_metadata(pageSoup=None, url: str = None) -> tuple:
+    """Extracts general info (teams, managers, captains, date, time, venue, attendance, score, xG) for a given match
+
+    Args:
+        pageSoup (bs4, optional): bs4 object of a match. Defaults to None.
+        url (str, optional): path of fbref match page. Defaults to None.
+
+    Returns:
+        tuple: metadata and officials
+            dict: metadata information
+            dict: match officials
+    """
+
+    assert (
+        pageSoup is not None or url is not None
+    ), "Either pageSoup or url must be provided"
+
+    if pageSoup is None:
+        pageSoup = get_page_soup(url)
+
+    url, match_id = _extract_url(pageSoup)
+    id_x, team_x, id_y, team_y = _extract_teams(pageSoup)
+    score_x, score_y, xg_x, xg_y = _extract_scores(pageSoup)
+    (
+        manager_x,
+        manager_y,
+        captain_x,
+        captain_y,
+        captain_url_x,
+        captain_url_y,
+        captain_id_x,
+        captain_id_y,
+    ) = _extract_managers_captains(pageSoup)
+
     # Find match information object
     scorebox_meta = pageSoup.find("div", {"class": "scorebox_meta"})
 
     # extract date and time information
     datetime = scorebox_meta.find("span", {"class": "venuetime"})
     date = datetime["data-venue-date"]
     kickoff = datetime["data-venue-time"]
```

### Comparing `reus-1.1.2/reus/fbref/fb_match_misc_stats.py` & `reus-1.1.3/reus/fbref/fb_match_misc_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_passing_stats.py` & `reus-1.1.3/reus/fbref/fb_match_passing_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_passing_type_stats.py` & `reus-1.1.3/reus/fbref/fb_match_passing_type_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_possession_stats.py` & `reus-1.1.3/reus/fbref/fb_match_possession_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_shots.py` & `reus-1.1.3/reus/fbref/fb_match_shots.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_summary.py` & `reus-1.1.3/reus/fbref/fb_match_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 from ..util import get_page_soup
 
 
+def _extract_event_type(event, divs):
+    # goal and shootout handling
+    if divs[2]["class"][1] == "own_goal":
+        event = "Own Goal"
+    elif event.startswith("Goal"):
+        event = "Goal"
+    elif divs[2]["class"][1] == "penalty_shootout_goal":
+        event = "Goal (shootout)"
+    elif divs[2]["class"][1] == "penalty_shootout_miss":
+        event = "Miss (shootout)"
+    elif divs[2]["class"][1] == "penalty_goal":
+        event = "Goal (penalty)"
+    elif divs[2]["class"][1] == "penalty_miss":
+        event = "Miss (penalty)"
+
+    return event
+
+
+def _extract_event_player(event, divs):
+    try:
+        event_player1 = divs[3].find("a", href=True)["href"]
+    except (AttributeError, TypeError):
+        return None, None
+
+    if event in ["Goal (penalty)", "Own Goal", "Goal (shootout)"]:
+        event_player2 = None
+    else:
+        try:
+            event_player2 = divs[3].find("small").find("a", href=True)["href"]
+        except (AttributeError, TypeError):
+            event_player2 = None
+
+    return event_player1, event_player2
+
+
 def fb_match_summary(pageSoup=None, url: str = None) -> list:
     """Extracts events (goals, bookings, and substitutions) from match summary for a given match
 
     Args:
         pageSoup (bs4, optional): bs4 object of a match. Defaults to None.
         url (str, optional): path of fbref match page. Defaults to None.
 
@@ -24,15 +59,14 @@
     events = summary.find_all("div", {"class": ["event a", "event b"]})
 
     # generate empty list
     eventList = []
 
     # iterate through each event
     for eve in events:
-
         # generate dictionary for each event
         mydict = {}
 
         # determine team
         if eve["class"][1] == "a":
             team = "x"
         else:
@@ -41,61 +75,41 @@
         divs = eve.find_all("div")
 
         mins = divs[0].text.split("\u2019")[0].strip()
         score = divs[0].find("small").text
         event = divs[5].text.split("—")[1].strip()
 
         # goal and shootout handling
-        if divs[2]["class"][1] == "own_goal":
-            event = "Own Goal"
-        elif event.startswith("Goal"):
-            event = "Goal"
-        elif divs[2]["class"][1] == "penalty_shootout_goal":
-            event = "Goal (shootout)"
-        elif divs[2]["class"][1] == "penalty_shootout_miss":
-            event = "Miss (shootout)"
-        elif divs[2]["class"][1] == "penalty_goal":
-            event = "Goal (penalty)"
-        elif divs[2]["class"][1] == "penalty_miss":
-            event = "Miss (penalty)"
+        event = _extract_event_type(event, divs)
+
+        score_x, score_y = map(int, score.split(":"))
 
         # determine score before goal
         if event in ["Goal", "Own Goal", "Goal (shootout)", "Goal (penalty)"]:
-            score_x, score_y = score.split(":")
             if team == "x":
-                score_x = int(score_x) - 1
-                score_pre = str(score_x) + ":" + score_y
+                score_x -= 1
+                score_pre = f"{score_x}:{score_y}"
             else:
-                score_y = int(score_y) - 1
-                score_pre = score_x + ":" + str(score_y)
+                score_y -= 1
+                score_pre = f"{score_x}:{score_y}"
         else:
             score_pre = score
 
-        score_post = score
-
         # extract primary and secondary (if applicable)
-        try:
-            event_player1 = divs[3].find("a", href=True)["href"]
-        except (AttributeError, TypeError):
+        event_player1, event_player2 = _extract_event_player(event, divs)
+        if event_player1 is None:
             continue
-        if event in ["Goal (penalty)", "Own Goal", "Goal (shootout)"]:
-            event_player2 = None
-        else:
-            try:
-                event_player2 = divs[3].find("small").find("a", href=True)["href"]
-            except (AttributeError, TypeError):
-                event_player2 = None
 
         # generate dictionary for each event
         mydict = {
             "team": team,
             "minute": mins,
             "event": event,
             "score_pre": score_pre,
-            "score_post": score_post,
+            "score_post": score,
             "player1": event_player1,
             "player2": event_player2,
         }
 
         # append event dictionary to list
         eventList.append(mydict)
```

### Comparing `reus-1.1.2/reus/fbref/fb_match_summary_stats.py` & `reus-1.1.3/reus/fbref/fb_match_summary_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_match_urls.py` & `reus-1.1.3/reus/fbref/fb_match_urls.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_season_fixture_urls.py` & `reus-1.1.3/reus/fbref/fb_season_fixture_urls.py`

 * *Files 25% similar despite different names*

```diff
@@ -55,72 +55,25 @@
     """
 
     df = pd.read_csv(
         "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/all_competitions.csv",
         keep_default_na=False,
     )
 
-    # Competition type
-    if competition_type is None:
-        competition_type = df.competition_type.unique()
-    elif not isinstance(competition_type, list):
-        competition_type = [competition_type]
-
-    df = df[df.competition_type.isin(competition_type)]
-
-    # Competition name
-    if competition_name is None:
-        competition_name = df.competition_name.unique()
-    elif not isinstance(competition_name, list):
-        competition_name = [competition_name]
-
-    df = df[df.competition_name.isin(competition_name)]
-
-    # Country
-    if country is None:
-        country = df.country.unique()
-    elif not isinstance(country, list):
-        country = [country]
-
-    df = df[df.country.isin(country)]
-
-    # Gender
-    if gender is None:
-        gender = df.gender.unique()
-    elif not isinstance(gender, list):
-        gender = [gender]
-
-    df = df[df.gender.isin(gender)]
-
-    # Governing body
-    if governing_body is None:
-        governing_body = df.governing_body.unique()
-    elif not isinstance(governing_body, list):
-        governing_body = [governing_body]
-
-    df = df[df.governing_body.isin(governing_body)]
-
-    # Tier
-    if tier is None:
-        tier = df.tier.unique()
-    elif not isinstance(tier, list):
-        tier = [tier]
-
-    df = df[df.tier.isin(tier)]
-
-    # Season end
-    if season_end_year is None:
-        season_end_year = df.season_end_year.unique()
-    elif not isinstance(season_end_year, list):
-        season_end_year = [season_end_year]
-
-    df = df[df.season_end_year.isin(season_end_year)]
-
-    # Advanced stats
-    if advanced is None:
-        advanced = df.advanced.unique()
-    elif not isinstance(advanced, list):
-        advanced = [advanced]
-
-    df = df[df.advanced.isin(advanced)]
+    filters = {
+        "competition_type": competition_type,
+        "competition_name": competition_name,
+        "country": country,
+        "gender": gender,
+        "governing_body": governing_body,
+        "tier": tier,
+        "season_end_year": season_end_year,
+        "advanced": advanced,
+    }
+
+    for column, value in filters.items():
+        if value is not None:
+            if not isinstance(value, list):
+                value = [value]
+            df = df[df[column].isin(value)]
 
     return df["fixtures_url"]
```

### Comparing `reus-1.1.2/reus/fbref/fb_season_urls.py` & `reus-1.1.3/reus/fotmob/fm_leagues.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,48 @@
 import pandas as pd
 
 
-def fb_season_urls(
+def fm_leagues(
     competition_type: str = None,
     competition_name: str = None,
+    ccode: str = None,
     country: str = None,
     gender: str = None,
-    governing_body: str = None,
-    tier: str = None,
-    season_end_year: int = None,
-    advanced: str = None,
-) -> pd.Series:
-    """Returns a series of urls for overview section of a season
+    league_id: str = None,
+    league_url: str = None,
+) -> pd.DataFrame:
+    """Returns a dataframe of league information
 
     Args:
         competition_type (str or list, optional): type of competition. Defaults to None. \n
             'Domestic Leagues - 1st Tier' \n
             'Domestic Leagues - 2nd Tier' \n
             'Domestic Leagues - 3rd Tier and Lower' \n
             'Domestic Cups' \n
             'Domestic Youth Leagues' \n
             'Club International Cups' \n
             'National Team Competitions' \n
             'National Team Qualification'
-        competition_name (str or list, optional): name of competition. Defaults to None.
-        country (str or list, optional): country of competition. Defaults to None.
-        gender (str or list, optional): gender of competition. Defaults to None.
+        competition_name (str): name of a league. Defaults to None.
+        ccode (str): country code of a league. Defaults to None.
+        country (str): country of a league. Defaults to None.
+        gender (str or list, optional): gender of competition. Defaults to None. \n
             'M' \n
             'W'
-        governing_body (str or list, optional): governing body of competition. Defaults to None. \n
-            'AFC' \n
-            'CAF' \n
-            'CONMEBOL' \n
-            'CONCACAF' \n
-            'OFC' \n
-            'UEFA' \n
-            'FIFA' \n
-            ''
-        tier (str or list, optional): tier of competition. Defaults to None. \n
-            '1st' \n
-            '2nd' \n
-            '3rd' \n
-            '4th' \n
-            '5th' \n
-            'Youth' \n
-            ''
-        season_end_year (int or list, optional): year at end of competition. Defaults to None.
-        advanced (str or list, optional): flag for if advanced data is available. Defaults to None. \n
-            'Y' \n
-            'N'
+        league_id (str): league id of a league. Defaults to None.
+        league_url (str): league url of a league. Defaults to None.
 
     Returns:
-        series: season urls
+        dataframe: league information
     """
 
+    # fix url to github
     df = pd.read_csv(
-        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/all_competitions.csv",
-        keep_default_na=False,
+        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/fotmob_leagues.csv",
+        encoding="latin-1",
     )
 
     # Competition type
     if competition_type is None:
         competition_type = df.competition_type.unique()
     elif not isinstance(competition_type, list):
         competition_type = [competition_type]
@@ -71,14 +53,22 @@
     if competition_name is None:
         competition_name = df.competition_name.unique()
     elif not isinstance(competition_name, list):
         competition_name = [competition_name]
 
     df = df[df.competition_name.isin(competition_name)]
 
+    # Country code
+    if ccode is None:
+        ccode = df.ccode.unique()
+    elif not isinstance(ccode, list):
+        ccode = [ccode]
+
+    df = df[df.ccode.isin(ccode)]
+
     # Country
     if country is None:
         country = df.country.unique()
     elif not isinstance(country, list):
         country = [country]
 
     df = df[df.country.isin(country)]
@@ -87,40 +77,24 @@
     if gender is None:
         gender = df.gender.unique()
     elif not isinstance(gender, list):
         gender = [gender]
 
     df = df[df.gender.isin(gender)]
 
-    # Governing body
-    if governing_body is None:
-        governing_body = df.governing_body.unique()
-    elif not isinstance(governing_body, list):
-        governing_body = [governing_body]
-
-    df = df[df.governing_body.isin(governing_body)]
-
-    # Tier
-    if tier is None:
-        tier = df.tier.unique()
-    elif not isinstance(tier, list):
-        tier = [tier]
-
-    df = df[df.tier.isin(tier)]
-
-    # Season end
-    if season_end_year is None:
-        season_end_year = df.season_end_year.unique()
-    elif not isinstance(season_end_year, list):
-        season_end_year = [season_end_year]
-
-    df = df[df.season_end_year.isin(season_end_year)]
-
-    # Advanced stats
-    if advanced is None:
-        advanced = df.advanced.unique()
-    elif not isinstance(advanced, list):
-        advanced = [advanced]
+    # League ID
+    if league_id is None:
+        league_id = df.id.unique()
+    elif not isinstance(league_id, list):
+        league_id = [league_id]
+
+    df = df[df.id.isin(league_id)]
+
+    # League URL
+    if league_url is None:
+        league_url = df.league_url.unique()
+    elif not isinstance(league_url, list):
+        league_url = [league_url]
 
-    df = df[df.advanced.isin(advanced)]
+    df = df[df.league_url.isin(league_url)]
 
-    return df["seasons_urls"]
+    return df
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_advanced_keeper_stats.py` & `reus-1.1.3/reus/fbref/fb_team_advanced_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_data.py` & `reus-1.1.3/reus/fbref/fb_team_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_defensive_actions_stats.py` & `reus-1.1.3/reus/fbref/fb_team_defensive_actions_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_goal_sca_stats.py` & `reus-1.1.3/reus/fbref/fb_team_goal_sca_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_keeper_stats.py` & `reus-1.1.3/reus/fbref/fb_team_keeper_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_misc_stats.py` & `reus-1.1.3/reus/fbref/fb_team_misc_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_passing_stats.py` & `reus-1.1.3/reus/fbref/fb_team_passing_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_passing_type_stats.py` & `reus-1.1.3/reus/fbref/fb_team_passing_type_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_advanced_keeper_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_advanced_keeper_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # goals
         goals_allowed = row.find("td", {"data-stat": "gk_goals_against"}).text
         pk_allowed = row.find("td", {"data-stat": "gk_pens_allowed"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_data.py` & `reus-1.1.3/reus/fbref/fb_team_player_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_defensive_actions_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_defensive_actions_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # tackles
         tackles_attempted = row.find("td", {"data-stat": "tackles"}).text
         tackles_successful = row.find("td", {"data-stat": "tackles_won"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_goal_sca_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_goal_sca_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # sca
         shot_creating_actions = row.find("td", {"data-stat": "sca"}).text
         shot_creating_actions_p90 = row.find("td", {"data-stat": "sca_per90"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_keeper_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_keeper_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
 
         # playing time
         matches = row.find("td", {"data-stat": "gk_games"}).text
         starts = row.find("td", {"data-stat": "gk_games_starts"}).text
         minutes = row.find("td", {"data-stat": "gk_minutes"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_misc_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_misc_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
 
         # performance
         cards_yellow = row.find("td", {"data-stat": "cards_yellow"}).text
         cards_red = row.find("td", {"data-stat": "cards_red"}).text
         cards_yellow_red = row.find("td", {"data-stat": "cards_yellow_red"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_passing_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_passing_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # total
         passes_completed = row.find("td", {"data-stat": "passes_completed"}).text
         passes_attempted = row.find("td", {"data-stat": "passes"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_passing_type_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_passing_type_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
         passes_attempted = row.find("td", {"data-stat": "passes"}).text
 
         # pass types
         live = row.find("td", {"data-stat": "passes_live"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_playing_time_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_playing_time_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
 
         # playing time
         matches = row.find("td", {"data-stat": "games"}).text
         minutes = row.find("td", {"data-stat": "minutes"}).text
         minutes_per_match = row.find("td", {"data-stat": "minutes_per_game"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_possession_stats.py` & `reus-1.1.3/reus/fbref/fb_team_possession_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,141 +1,132 @@
 from ..util import get_page_soup
 
 
-def fb_team_player_possession_stats(pageSoup=None, url: str = None) -> list:
-    """Extracts possession stats for each player in a given team
+def fb_team_possession_stats(pageSoup=None, url: str = None) -> list:
+    """Extracts possession stats for each team in a given league
 
     Args:
         pageSoup (bs4, optional): bs4 object of a team. Defaults to None.
         url (str, optional): path of fbref team page. Defaults to None.
 
     Returns:
-        list: possession stats for each player
+        tuple: possession stats for home and away team players
+            list: possession stats for each team
+            list: possession stats against each team
     """
 
     assert (
         pageSoup is not None or url is not None
     ), "Either pageSoup or url must be provided"
 
-    assert (
-        pageSoup is not None or url is not None
-    ), "Either pageSoup or url must be provided"
-
     if pageSoup is None:
         pageSoup = get_page_soup(url)
 
-    # Find table object
-    div = pageSoup.find("div", {"id": "all_stats_possession"})
-    if div is None:
-        return None
-
-    table = div.find("table")
-    tbody = table.find("tbody")
-    rows = tbody.find_all("tr")
-
-    # Generate empty list
-    mylist = []
-
-    # iterate through each player and store attributes
-    for row in rows:
-        # general
-        th = row.find("th")
-        try:
-            name = th.text
-        except AttributeError:
-            name = th["csk"]
-        player_id = th.find("a", href=True)["href"].split("/")[3]
-        nation = row.find("td", {"data-stat": "nationality"}).text
-        position = row.find("td", {"data-stat": "position"}).text
-        age = row.find("td", {"data-stat": "age"}).text.split("-")
-        try:
-            age = int(age[0]) + int(age[1]) / 365
-        except ValueError:
-            age = None
-        minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
-
-        # touches
-        touches = row.find("td", {"data-stat": "touches"}).text
-        touches_def_pen_area = row.find(
-            "td", {"data-stat": "touches_def_pen_area"}
-        ).text
-        touches_def_3rd = row.find("td", {"data-stat": "touches_def_3rd"}).text
-        touches_mid_3rd = row.find("td", {"data-stat": "touches_mid_3rd"}).text
-        touches_att_3rd = row.find("td", {"data-stat": "touches_att_3rd"}).text
-        touches_att_pen_area = row.find(
-            "td", {"data-stat": "touches_att_pen_area"}
-        ).text
-        touches_live = row.find("td", {"data-stat": "touches_live_ball"}).text
-
-        # take ons
-        dribble_attempt = row.find("td", {"data-stat": "take_ons"}).text
-        dribble_success = row.find("td", {"data-stat": "take_ons_won"}).text
-        dribble_success_pct = row.find("td", {"data-stat": "take_ons_won_pct"}).text
-        if dribble_success_pct == "":
-            dribble_success_pct = None
-        dribble_tackled = row.find("td", {"data-stat": "take_ons_tackled"}).text
-        dribble_tackled_pct = row.find("td", {"data-stat": "take_ons_tackled_pct"}).text
-
-        # carries
-        carries = row.find("td", {"data-stat": "carries"}).text
-        carries_total_distance = row.find("td", {"data-stat": "carries_distance"}).text
-        carries_progressive_distance = row.find(
-            "td", {"data-stat": "carries_progressive_distance"}
-        ).text
-        progressive_carries = row.find("td", {"data-stat": "progressive_carries"}).text
-        carries_into_final_third = row.find(
-            "td", {"data-stat": "carries_into_final_third"}
-        ).text
-        carries_into_penalty_area = row.find(
-            "td", {"data-stat": "carries_into_penalty_area"}
-        ).text
-        miscontrols = row.find("td", {"data-stat": "miscontrols"}).text
-        dispossessed = row.find("td", {"data-stat": "dispossessed"}).text
-
-        # receiving
-        passes_received = row.find("td", {"data-stat": "passes_received"}).text
-        progressive_passes_received = row.find(
-            "td", {"data-stat": "progressive_passes_received"}
-        ).text
-
-        # match logs
-        match_logs = row.find("td", {"data-stat": "matches"}).find("a", href=True)[
-            "href"
-        ]
-
-        # generate dictionary for player
-        mydict = {
-            "player_id": player_id,
-            "name": name,
-            "nation": nation,
-            "position": position,
-            "age": age,
-            "90s": minutes_90,
-            "touches": touches,
-            "touches_def_pen_area": touches_def_pen_area,
-            "touches_def_3rd": touches_def_3rd,
-            "touches_mid_3rd": touches_mid_3rd,
-            "touches_att_3rd": touches_att_3rd,
-            "touches_att_pen_area": touches_att_pen_area,
-            "touches_live": touches_live,
-            "dribble_attempt": dribble_attempt,
-            "dribble_success": dribble_success,
-            "dribble_success_pct": dribble_success_pct,
-            "dribble_tackled": dribble_tackled,
-            "dribble_tackled_pct": dribble_tackled_pct,
-            "carries": carries,
-            "carry_total_distance": carries_total_distance,
-            "carry_progressive_distance": carries_progressive_distance,
-            "progressive_carries": progressive_carries,
-            "carries_into_final_third": carries_into_final_third,
-            "carries_into_penalty_area": carries_into_penalty_area,
-            "miscontrols": miscontrols,
-            "dispossessed": dispossessed,
-            "passes_received": passes_received,
-            "progressive_passes_received": progressive_passes_received,
-            "match_logs": match_logs,
-        }
-
-        # add to empty list
-        mylist.append(mydict)
+    for side in ["for", "against"]:
+        # generate empty list for each team
+        mylist = []
+        # generate html id
+        id_ = "stats_squads_possession_" + side
+
+        # find goalkeeping object
+        stats = pageSoup.find("table", {"id": id_})
+        stats = stats.find_all("tr")
+
+        # iteratre through each team and store metrics
+        for row in stats[2:]:
+            th = row.find("th")
+            # general
+            team = th.find("a", {"href": True}).text.strip()
+            team_id = th.find("a", {"href": True})["href"].split("/")[3]
+            num_players = row.find("td", {"data-stat": "players_used"}).text
+            matches = row.find("td", {"data-stat": "minutes_90s"}).text
+
+            # touches
+            touches = row.find("td", {"data-stat": "touches"}).text
+            touches_def_pen_area = row.find(
+                "td", {"data-stat": "touches_def_pen_area"}
+            ).text
+            touches_def_3rd = row.find("td", {"data-stat": "touches_def_3rd"}).text
+            touches_mid_3rd = row.find("td", {"data-stat": "touches_mid_3rd"}).text
+            touches_att_3rd = row.find("td", {"data-stat": "touches_att_3rd"}).text
+            touches_att_pen_area = row.find(
+                "td", {"data-stat": "touches_att_pen_area"}
+            ).text
+            touches_live = row.find("td", {"data-stat": "touches_live_ball"}).text
+
+            # take ons
+            dribble_attempt = row.find("td", {"data-stat": "take_ons"}).text
+            dribble_success = row.find("td", {"data-stat": "take_ons_won"}).text
+            dribble_success_pct = row.find("td", {"data-stat": "take_ons_won_pct"}).text
+            if dribble_success_pct == "":
+                dribble_success_pct = None
+            dribble_tackled = row.find("td", {"data-stat": "take_ons_tackled"}).text
+            dribble_tackled_pct = row.find(
+                "td", {"data-stat": "take_ons_tackled_pct"}
+            ).text
+
+            # carries
+            carries = row.find("td", {"data-stat": "carries"}).text
+            carries_total_distance = row.find(
+                "td", {"data-stat": "carries_distance"}
+            ).text
+            carries_progressive_distance = row.find(
+                "td", {"data-stat": "carries_progressive_distance"}
+            ).text
+            progressive_carries = row.find(
+                "td", {"data-stat": "progressive_carries"}
+            ).text
+            carries_into_final_third = row.find(
+                "td", {"data-stat": "carries_into_final_third"}
+            ).text
+            carries_into_penalty_area = row.find(
+                "td", {"data-stat": "carries_into_penalty_area"}
+            ).text
+            miscontrols = row.find("td", {"data-stat": "miscontrols"}).text
+            dispossessed = row.find("td", {"data-stat": "dispossessed"}).text
+
+            # receiving
+            passes_received = row.find("td", {"data-stat": "passes_received"}).text
+            progressive_passes_received = row.find(
+                "td", {"data-stat": "progressive_passes_received"}
+            ).text
+
+            # generate dictionary for team
+            mydict = {
+                "team_id": team_id,
+                "team": team,
+                "num_players": num_players,
+                "matches": matches,
+                "touches": touches,
+                "touches_def_pen_area": touches_def_pen_area,
+                "touches_def_3rd": touches_def_3rd,
+                "touches_mid_3rd": touches_mid_3rd,
+                "touches_att_3rd": touches_att_3rd,
+                "touches_att_pen_area": touches_att_pen_area,
+                "touches_live": touches_live,
+                "dribble_attempt": dribble_attempt,
+                "dribble_success": dribble_success,
+                "dribble_success_pct": dribble_success_pct,
+                "dribble_tackled": dribble_tackled,
+                "dribble_tackled_pct": dribble_tackled_pct,
+                "carries": carries,
+                "carry_total_distance": carries_total_distance,
+                "carry_progressive_distance": carries_progressive_distance,
+                "progressive_carries": progressive_carries,
+                "carries_into_final_third": carries_into_final_third,
+                "carries_into_penalty_area": carries_into_penalty_area,
+                "miscontrols": miscontrols,
+                "dispossessed": dispossessed,
+                "passes_received": passes_received,
+                "progressive_passes_received": progressive_passes_received,
+            }
+
+            # add to empty list
+            mylist.append(mydict)
+
+        # assign list to appropriate team
+        if side == "for":
+            possession_stats_for = mylist.copy()
+        else:
+            possession_stats_against = mylist.copy()
 
-    return mylist
+    return possession_stats_for, possession_stats_against
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_shooting_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_shooting_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # standard
         goals = row.find("td", {"data-stat": "goals"}).text
         shots = row.find("td", {"data-stat": "shots"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_player_summary_stats.py` & `reus-1.1.3/reus/fbref/fb_team_player_summary_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             name = th["csk"]
         player_id = th.find("a", href=True)["href"].split("/")[3]
         nation = row.find("td", {"data-stat": "nationality"}).text
         position = row.find("td", {"data-stat": "position"}).text
         age = row.find("td", {"data-stat": "age"}).text.split("-")
         try:
             age = int(age[0]) + int(age[1]) / 365
+        except IndexError:
+            age = int(age[0])
         except ValueError:
             age = None
         minutes = row.find("td", {"data-stat": "minutes"}).text
         minutes_90 = row.find("td", {"data-stat": "minutes_90s"}).text
 
         # performance
         goals = row.find("td", {"data-stat": "goals"}).text
```

### Comparing `reus-1.1.2/reus/fbref/fb_team_playing_time_stats.py` & `reus-1.1.3/reus/fbref/fb_team_playing_time_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_shooting_stats.py` & `reus-1.1.3/reus/fbref/fb_team_shooting_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fbref/fb_team_summary_stats.py` & `reus-1.1.3/reus/fbref/fb_team_summary_stats.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/fotmob/fm_league_matches.py` & `reus-1.1.3/reus/fotmob/fm_league_matches.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
 from urllib.request import urlopen
 import pandas as pd
 
 
-def fm_league_matches(league_id: str, json_file: json = None) -> pd.DataFrame:
+def fm_league_matches(
+    league_id: str, season: str = None, json_file: json = None
+) -> pd.DataFrame:
     """Returns matches of a given league
 
     Args:
         league_id (str): id of a league
+        season (str, optional): season of a league. Use / divider for leagues over 2 calendar years. Defaults to None.
         json_file (json, optional): json file of match data. Defaults to None.
 
     Returns:
         dataframe: league matches
     """
 
     if json_file is None:
-        url = f"https://www.fotmob.com/api/leagues?id={league_id}"
+        url = f"https://www.fotmob.com/api/leagues?id={league_id}&season={season}"
 
         response = urlopen(url)
         data = json.loads(response.read())
     else:
         data = json_file
 
     df = pd.DataFrame(data["matches"]["allMatches"])
```

### Comparing `reus-1.1.2/reus/fotmob/fm_league_table.py` & `reus-1.1.3/reus/fotmob/fm_league_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 from urllib.request import urlopen
 import pandas as pd
 
 
-def fm_league_table(league_id: str, matches="All", json_file: json = None) -> dict:
+def fm_league_table(
+    league_id: str, season: str = None, matches="All", json_file: json = None
+) -> dict:
     """Returns standing of a given league
 
     Args:
         league_id (str): id of a league
+        season (str, optional): season of a league. Use / divider for leagues over 2 calendar years. Defaults to None.
         matches (str, optional): type of matches to include in standings. Defaults to "All". \n
             'All' \n
             'Home' \n
             'Away' \n
             'Form'
         json_file (json, optional): json file of league page. Defaults to None.
 
@@ -23,15 +26,15 @@
         "All",
         "Home",
         "Away",
         "Form",
     ], "matches must be one of 'All', 'Home', 'Away', or 'Form'"
 
     if json_file is None:
-        url = f"https://www.fotmob.com/api/leagues?id={league_id}"
+        url = f"https://www.fotmob.com/api/leagues?id={league_id}&season={season}"
 
         response = urlopen(url)
         data = json.loads(response.read())
     else:
         data = json_file
 
     mydict = {}
```

### Comparing `reus-1.1.2/reus/fotmob/fm_match_ids.py` & `reus-1.1.3/reus/fotmob/fm_match_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ccode: str = None,
     name: str = None,
     league_id: int = None,
 ) -> list:
     """Returns a list of match ids for a given date
 
     Args:
-        match_date (str): date of matches in format YYYY-MM-DD
+        match_date (str): date of matches in format YYYYMMDD
         ccode (str): country code of a league. Defaults to None.
         name (str): name of a league. Defaults to None.
         league_id (int): league id of a league. Defaults to None.
 
     Returns:
         list: match ids
     """
```

### Comparing `reus-1.1.2/reus/fotmob/fm_season_stats.py` & `reus-1.1.3/reus/fotmob/fm_season_stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,44 @@
 import json
 
 
 def fm_season_stats(
     league_id: str,
     team_or_player: str,
     stat_name: str,
+    season: str = None,
     url: str = None,
     json_file: json = None,
 ) -> pd.DataFrame:
     """Returns complete list of stat leaders of a given league
 
     Args:
         league_id (str): id of a league
         team_or_player (str): 'teams' or 'players'
-        stat_name (str, optional): name of stat. See documentation for list of available stats. Defaults to None.
+        stat_name (str): name of stat. See documentation for list of available stats.
+        season (str, optional): season of a league. Use / divider for leagues over 2 calendar years. Defaults to None.
         url (str, optional): url of stat leaders. Defaults to None.
         json_file (json, optional): json file of stat data. Defaults to None.
 
     Returns:
         dataframe: stat leaders
     """
 
     assert team_or_player in [
         "teams",
         "players",
     ], "team_or_player must be one of 'teams' or 'players'"
 
     if url is None and json_file is None:
-        leaders = fm_season_stat_leaders(league_id, team_or_player, stat_name)
+        leaders = fm_season_stat_leaders(
+            league_id=league_id,
+            team_or_player=team_or_player,
+            stat_name=stat_name,
+            season=season,
+        )
         url = leaders["all_url"].iloc[0]
 
         response = requests.get(url)
         data = response.json()
     else:
         data = json_file
```

### Comparing `reus-1.1.2/reus/fotmob/util.py` & `reus-1.1.3/reus/fotmob/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 def extract_player_stats(stats):
     mydict = {}
 
     playerStats = stats[0].get("stats")
+    tmp = {}
+    for k, v in playerStats.items():
+        tmp[k] = v.get("value")
+    playerStats = tmp
+
     mydict["rating"] = playerStats.get("FotMob rating")
     mydict["goals"] = playerStats.get("Goals")
     mydict["assists"] = playerStats.get("Assists")
     mydict["total_shots"] = playerStats.get("Total shots")
     mydict["accurate_passes"] = playerStats.get("Accurate passes")
     mydict["chances_created"] = playerStats.get("Chances created")
     mydict["xG"] = playerStats.get("Expected goals (xG)")
@@ -15,14 +20,19 @@
     mydict["fantasy_points"] = playerStats.get("Fantasy points")
     mydict["errors_lead_to_goal"] = playerStats.get("Error led to goal")
     if mydict["errors_lead_to_goal"] is None:
         mydict["errors_lead_to_goal"] = playerStats.get("Errors led to goal")
 
     try:
         playerStatsAttack = stats[1].get("stats")
+        tmp = {}
+        for k, v in playerStatsAttack.items():
+            tmp[k] = v.get("value")
+        playerStatsAttack = tmp
+
         mydict["shot_accuracy"] = playerStatsAttack.get("Shot accuracy")
         mydict["blocked_shots"] = playerStatsAttack.get("Blocked shots")
         mydict["big_chances_missed"] = playerStatsAttack.get("Big chance missed")
         mydict["touches"] = playerStatsAttack.get("Touches")
         mydict["successful_dribbles"] = playerStatsAttack.get("Successful dribbles")
         mydict["passes_into_final_third"] = playerStatsAttack.get(
             "Passes into final third"
@@ -34,26 +44,36 @@
         mydict["dispossessed"] = playerStatsAttack.get("Dispossessed")
     except IndexError:
         mydict["touches"] = playerStats.get("Touches")
         mydict["accurate_long_balls"] = playerStats.get("Accurate long balls")
 
     try:
         playerStatsDefense = stats[2].get("stats")
+        tmp = {}
+        for k, v in playerStatsDefense.items():
+            tmp[k] = v.get("value")
+        playerStatsDefense = tmp
+
         mydict["tackles_won"] = playerStatsDefense.get("Tackles won")
         mydict["blocks"] = playerStatsDefense.get("Blocks")
         mydict["clearances"] = playerStatsDefense.get("Clearances")
         mydict["headed_clearances"] = playerStatsDefense.get("Headed clearance")
         mydict["interceptions"] = playerStatsDefense.get("Interceptions")
         mydict["recoveries"] = playerStatsDefense.get("Recoveries")
         mydict["dribbled_past"] = playerStatsDefense.get("Dribbled past")
     except IndexError:
         pass
 
     try:
         playerStatsDuels = stats[3].get("stats")
+        tmp = {}
+        for k, v in playerStatsDuels.items():
+            tmp[k] = v.get("value")
+        playerStatsDuels = tmp
+
         mydict["ground_duels_won"] = playerStatsDuels.get("Ground duels won")
         mydict["aerial_duels_won"] = playerStatsDuels.get("Aerial duels won")
         mydict["was_fouled"] = playerStatsDuels.get("Was fouled")
         mydict["fouls_committed"] = playerStatsDuels.get("Fouls committed")
     except IndexError:
         pass
```

### Comparing `reus-1.1.2/reus/transfermarkt/tm_player_data.py` & `reus-1.1.3/reus/transfermarkt/tm_player_data.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/transfermarkt/tm_player_injury.py` & `reus-1.1.3/reus/transfermarkt/tm_player_injury.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/transfermarkt/tm_player_market_value.py` & `reus-1.1.3/reus/transfermarkt/tm_player_market_value.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/transfermarkt/tm_player_metadata.py` & `reus-1.1.3/reus/transfermarkt/tm_player_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,96 @@
 import re
 from ..util import get_page_soup_headers
 
 
+def _extract_text(attribute, tag, pattern, cat="text"):
+    try:
+        val = attribute.find(tag, text=pattern).find_next(tag)
+        if cat == "text":
+            return val.text.strip()
+        else:
+            return val.find("img")["title"]
+    except AttributeError:
+        return None
+
+
+def _extract_social_media(pageSoup, tag, pattern):
+    try:
+        val = (
+            pageSoup.find(tag, text="Social-Media:")
+            .find_next(tag)
+            .find("a", title=pattern)["href"]
+        )
+        return val
+    except (AttributeError, TypeError):
+        return None
+
+
+def extract_positions(pageSoup, position):
+    # position - primary
+    try:
+        position_data = pageSoup.find("div", {"class": "detail-position__box"})
+        position_main = (
+            position_data.find("dt", text="Main position:").find_next("dd").text.strip()
+        )
+    except AttributeError:
+        try:
+            position_main = position.split(" - ")[-1].strip()
+        except AttributeError:
+            position_main = None
+
+    # position - alternate
+    position_data = pageSoup.find("div", {"class": "detail-position__box"})
+    try:
+        pos_alt1 = position_data.find("dt", text="Other position:").find_next("dd").text
+    except AttributeError:
+        pos_alt1 = None
+
+    try:
+        pos_alt2 = position_data.find("dd", text=pos_alt1).find_next("dd").text
+    except AttributeError:
+        pos_alt2 = None
+
+    return position_main, pos_alt1, pos_alt2
+
+
+def _reorder_dict(mydict):
+    order = [
+        "id",
+        "name",
+        "url",
+        "headshot_url",
+        "full_name",
+        "born",
+        "birth_place",
+        "birth_country",
+        "age",
+        "height",
+        "nationality",
+        "position",
+        "position_main",
+        "position_alt1",
+        "position_alt2",
+        "foot",
+        "agent",
+        "outfitter",
+        "social_twitter",
+        "social_facebook",
+        "social_instagram",
+        "club",
+        "joined",
+        "contracted",
+        "extension",
+        "currency",
+        "mv",
+        "update",
+    ]
+    return {k: mydict[k] for k in order}
+
+
 def tm_player_metadata(pageSoup=None, url: str = None) -> dict:
     #
     """Extracts general player information (biographical, club, contract, market value, and miscellaneous)
 
     Args:
         pageSoup (bs4, optional): bs4 object of player page referenced in url. Defaults to None.
         url (str, optional): path of transfermarkt player page. Defaults to None.
@@ -25,213 +110,85 @@
     url = pageSoup.find("meta", {"property": "og:url"})["content"]
 
     # Find data object
     player_data = pageSoup.find("div", {"data-viewport": "Steckbrief"})
     headshot_url = pageSoup.find("div", {"class": "modal-trigger"}).find("img")["src"]
 
     # Extract data and error handling
-    # name
-    try:
-        full_name = (
-            player_data.find("span", text="Name in home country:")
-            .find_next("span")
-            .text.strip()
-        )
-    except AttributeError:
-        try:
-            full_name = (
-                player_data.find("span", text="Full name:")
-                .find_next("span")
-                .text.strip()
-            )
-        except AttributeError:
-            full_name = None
-
-    # birth date
-    try:
-        birth_date = (
-            player_data.find("span", text="Date of birth:")
-            .find_next("span")
-            .text.strip()
-        )
-        birth_date = birth_date.replace(" Happy Birthday", "")
-    except AttributeError:
-        birth_date = None
-
-    # birth place
-    try:
-        birth_place = (
-            player_data.find("span", text="Place of birth:")
-            .find_next("span")
-            .text.strip()
-        )
-    except AttributeError:
-        birth_place = None
-
-    # birth country
-    try:
-        birth_country = (
-            player_data.find("span", text="Place of birth:")
-            .find_next("span")
-            .find("img")["title"]
-        )
-    except AttributeError:
-        birth_country = None
-
-    # age
-    try:
-        age = player_data.find("span", text="Age:").find_next("span").text.strip()
-    except AttributeError:
-        age = None
-
-    # height
-    try:
-        height = player_data.find("span", text="Height:").find_next("span").text.strip()
-        height = height.replace(",", ".").replace("m", "").strip()
-    except AttributeError:
-        height = None
-
-    # nationality
-    try:
-        nationality = (
-            player_data.find("span", text="Citizenship:").find_next("span").text.strip()
-        )
-        nationality = re.split(r"\s{2,}", nationality)
-    except AttributeError:
-        nationality = None
+    attributes = {
+        "full_name": ["Name in home country:", "Full name:"],
+        "born": ["Date of birth:"],
+        "birth_place": ["Place of birth:"],
+        "birth_country": ["Place of birth:", "img"],
+        "age": ["Age:"],
+        "height": ["Height:"],
+        "nationality": ["Citizenship:"],
+        "position": ["Position:"],
+        "foot": ["Foot:"],
+        "agent": ["Player agent:"],
+        "outfitter": ["Outfitter:"],
+    }
 
-    # position
-    try:
-        position = (
-            player_data.find("span", text="Position:").find_next("span").text.strip()
-        )
-    except AttributeError:
-        position = None
+    player_info = {}
 
-    # foot
-    try:
-        foot = player_data.find("span", text="Foot:").find_next("span").text.strip()
-    except AttributeError:
-        foot = None
+    for attr, patterns in attributes.items():
+        cat = "img" if patterns[-1] == "img" else "text"
+        for pattern in patterns:
+            value = _extract_text(player_data, "span", pattern, cat)
+            player_info[attr] = value
+            if value is not None:
+                if attr == "birth_date":
+                    value = value.replace(" Happy Birthday", "")
+                elif attr == "height":
+                    value = value.replace(",", ".").replace("m", "").strip()
+                elif attr == "nationality":
+                    value = re.split(r"\s{2,}", value)[0]
 
-    # agent
-    try:
-        agent = (
-            player_data.find("span", text="Player agent:")
-            .find_next("span")
-            .text.strip()
-        )
-    except AttributeError:
-        agent = None
-
-    # outfitter
-    try:
-        outfitter = (
-            player_data.find("span", text="Outfitter:").find_next("span").text.strip()
-        )
-    except AttributeError:
-        outfitter = None
+                player_info[attr] = value
+                break
 
     # social media
-    try:
-        socialTwitter = (
-            pageSoup.find("span", text="Social-Media:")
-            .find_next("span")
-            .find("a", title="Twitter")["href"]
-        )
-    except AttributeError:
-        socialTwitter = None
-    except TypeError:
-        socialTwitter = None
-
-    try:
-        socialFacebook = (
-            pageSoup.find("span", text="Social-Media:")
-            .find_next("span")
-            .find("a", title="Facebook")["href"]
-        )
-    except AttributeError:
-        socialFacebook = None
-    except TypeError:
-        socialFacebook = None
-
-    try:
-        socialInstagram = (
-            pageSoup.find("span", text="Social-Media:")
-            .find_next("span")
-            .find("a", title="Instagram")["href"]
-        )
-    except AttributeError:
-        socialInstagram = None
-    except TypeError:
-        socialInstagram = None
-
-    # position - primary
-    try:
-        position_data = pageSoup.find("div", {"class": "detail-position__box"})
-        position_main = (
-            position_data.find("dt", text="Main position:").find_next("dd").text.strip()
-        )
-    except AttributeError:
-        try:
-            position_main = position.split(" - ")[-1].strip()
-        except AttributeError:
-            position_main = None
+    social_attributes = {
+        "social_twitter": "Twitter",
+        "social_facebook": "Facebook",
+        "social_instagram": "Instagram",
+    }
 
-    # position - alternate
-    try:
-        pos_alt1 = position_data.find("dt", text="Other position:").find_next("dd").text
-    except AttributeError:
-        pos_alt1 = None
-
-    try:
-        pos_alt2 = position_data.find("dd", text=pos_alt1).find_next("dd").text
-    except AttributeError:
-        pos_alt2 = None
+    for attr, pattern in social_attributes.items():
+        value = _extract_social_media(pageSoup, "span", pattern)
+        player_info[attr] = value
+
+    position_main, pos_alt1, pos_alt2 = extract_positions(
+        pageSoup, player_info["position"]
+    )
 
     # club
     club = pageSoup.find("div", {"class": "data-header__box--big"})
     club = club.find("img", alt=True)["alt"]
 
-    try:
-        joined = pageSoup.find("span", text="Joined:")
-        joined = joined.find_next("span").text.strip()
-    except AttributeError:
-        joined = None
-
-    # contract expiration
-    try:
-        contracted = pageSoup.find("span", text="Contract expires:")
-        contracted = contracted.find_next("span").text.strip()
-    except AttributeError:
-        contracted = None
+    meta_attributes = {
+        "joined": "Joined:",
+        "contracted": "Contract expires:",
+        "extension": "Date of last contract extension:",
+    }
 
-    # date of last contract extension
-    try:
-        extension = (
-            player_data.find("span", text="Date of last contract extension:")
-            .find_next("span")
-            .text.strip()
-        )
-    except AttributeError:
-        extension = None
+    for attr, pattern in meta_attributes.items():
+        value = _extract_text(pageSoup, "span", pattern)
+        player_info[attr] = value
 
     # market value
     try:
-        # value = pageSoup.find("div", {"class": "dataMarktwert"}).text
-        # updated = re.search("(?<=update: ).*$", value).group()
-        # value = value.split(" ")[0].strip()
         value = (
             pageSoup.find("div", {"class": "data-header__box--small"}).find("a").text
         )
         value = value.split("Last update: ")
         updated = value[1]
         value = value[0]
         currency = value[0]
-        mult = 1000000 if value[-1] == "m" else 1000
+        mult = 1000000 if value.strip()[-1] == "m" else 1000
         value = float(value[1:].replace("Th.", "").replace("m", "").strip()) * mult
     except AttributeError:
         value = None
         updated = None
         currency = None
 
     # url path, player_id, and name
@@ -241,34 +198,20 @@
 
     # Generate dictionary and store attributes
     mydict = {
         "id": id_,
         "name": name,
         "url": "/" + url.split("/")[-4] + "/profil/spieler/" + url.split("/")[-1],
         "headshot_url": headshot_url,
-        "full_name": full_name,
-        "born": birth_date,
-        "birth_place": birth_place,
-        "birth_country": birth_country,
-        "age": age,
-        "height": height,
-        "nationality": nationality[0],
-        "position": position,
         "position_main": position_main,
         "position_alt1": pos_alt1,
         "position_alt2": pos_alt2,
-        "foot": foot,
-        "agent": agent,
-        "outfitter": outfitter,
-        "social_twitter": socialTwitter,
-        "social_facebook": socialFacebook,
-        "social_instagram": socialInstagram,
         "club": club,
-        "joined": joined,
-        "contracted": contracted,
-        "extension": extension,
         "currency": currency,
         "mv": value,
         "update": updated,
+        **player_info,
     }
 
+    mydict = _reorder_dict(mydict)
+
     return mydict
```

### Comparing `reus-1.1.2/reus/transfermarkt/tm_player_transfers.py` & `reus-1.1.3/reus/transfermarkt/tm_player_transfers.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         else:
             transfer_type = "Transfer"
 
         # no market value
         mv = mv.replace("-", "0")
 
         # excess text
-        substring = ["Loan fee:", "€", "£", "$", "m", "Th.", "â\u201a¬"]
+        substring = ["Loan fee:", "€", "£", "$", "m", "Th.", "k", "â\u201a¬"]
         for s in substring:
             mv = mv.replace(s, "")
             fee = fee.replace(s, "")
 
         # generate dictionary for each transfer
         mydict = {
             "left": left,
```

### Comparing `reus-1.1.2/reus/transfermarkt/tm_team_player_data.py` & `reus-1.1.3/reus/transfermarkt/tm_team_player_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,153 @@
 from ..util import get_page_soup_headers
 from .util import tm_format_currency
 import pandas as pd
 
 
+def _get_team_id_and_club(team_id, club):
+    df = pd.read_csv(
+        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/team_translations.csv",
+        keep_default_na=False,
+    )
+    filter_condition = (
+        (df.fbref_name == club)
+        | (df.transfermarkt_name == club)
+        | (df.transfermarkt_link == club)
+        | (df.fcpython == club)
+        | (df.fivethirtyeight == club)
+    )
+    filtered_df = df[filter_condition]
+    club = filtered_df.transfermarkt_link.iloc[0]
+    team_id = int(filtered_df.transfermarkt.iloc[0])
+
+    return club, team_id
+
+
+def _extract_player_metadata(row, num):
+    # extract basic info
+    player_table = row.find("table")
+    url = player_table.find("a", href=True)["href"]
+    name = player_table.find("img")["alt"]
+    pos = player_table.find_all("tr")[1].text.strip()
+
+    # extract birth day and age
+    data = row.find_all("td", {"class": "zentriert"})
+    birth = data[1].text.strip()
+    birth = birth.split("(")
+    birth_date = birth[0].strip()
+    age = birth[1].replace(")", "").strip()
+
+    arrival_type = _extract_arrival_type(row)
+
+    # extract nation
+    nation = data[2].find("img")["alt"]
+
+    # extract height
+    try:
+        height = data[-5].text.strip()
+        height = height.replace(",", ".").replace("m", "").strip()
+    except TypeError:
+        height = None
+
+    # extract foot
+    try:
+        foot = data[-4].text.strip()
+        foot = None if foot == "-" else foot
+    except TypeError:
+        foot = None
+
+    # extract joined date
+    try:
+        joined = data[-3].text.strip()
+        joined = None if joined == "-" else joined
+    except TypeError:
+        joined = None
+
+    # extract signing information
+    signed_from, signed_from_url, signed_value, signed_currency = _extract_signing_info(
+        data
+    )
+
+    # extract contracted
+    try:
+        contracted = data[-1].text.strip()
+    except TypeError:
+        contracted = None
+
+    # extract market value
+    try:
+        mv = row.find("td", {"class": "rechts hauptlink"}).text
+        mv = tm_format_currency(mv)
+    except AttributeError:
+        mv = 0
+
+    # generate dictionary for each player
+    mydict = {
+        "name": name,
+        "url": url,
+        "number": num,
+        "position": pos,
+        "arrival_type": arrival_type,
+        "birth_date": birth_date,
+        "age": age,
+        "nation": nation,
+        "height": height,
+        "foot": foot,
+        "joined": joined,
+        "signed_from": signed_from,
+        "signed_from_url": signed_from_url,
+        "fee": signed_value,
+        "currency": signed_currency,
+        "contracted": contracted,
+        "market_value": mv,
+    }
+
+    return mydict
+
+
+def _extract_arrival_type(row):
+    # determine if new arrival and subsequent type
+    try:
+        arrival = row.find("a")["title"]
+        if "On loan" in arrival:
+            arrival_type = "Loan"
+        elif "Returned after loan spell" in arrival:
+            arrival_type = "Returned from Loan"
+        elif "Internal transfer" in arrival:
+            arrival_type = "Internal"
+        elif "free transfer" in arrival:
+            arrival_type = "free transfer"
+        elif "Joined from":
+            arrival_type = "Transfer"
+    except KeyError:
+        arrival_type = "N/A"
+
+    return arrival_type
+
+
+def _extract_signing_info(data):
+    try:
+        signed_from = data[-2].find("img")["alt"]
+        signed_from_url = data[-2].find("a", href=True)["href"]
+        signed_value = data[-2].find("a")["title"].split()[-1]
+        signed_currency = signed_value[0]
+        signed_value = signed_value.replace("-", "0").replace("transfer", "0")
+        if signed_value == "?":
+            signed_value = "unknown"
+        else:
+            signed_value = tm_format_currency(signed_value)
+    except TypeError:
+        signed_from = None
+        signed_from_url = None
+        signed_value = None
+        signed_currency = None
+
+    return signed_from, signed_from_url, signed_value, signed_currency
+
+
 def tm_team_player_data(
     club: str,
     season: str,
     domain: str = "us",
     team_id: int = None,
     transfermarkt_name: bool = False,
 ) -> list:
@@ -21,28 +162,15 @@
         transfermarkt_name (bool, optional): if True, club is a transfermarkt name. Defaults to False.
 
     Returns:
         list: squad players
     """
 
     if team_id is None and transfermarkt_name is False:
-        # Lookup team name
-        df = pd.read_csv(
-            "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/team_translations.csv",
-            keep_default_na=False,
-        )
-        df = df[
-            (df.fbref_name == club)
-            | (df.transfermarkt_name == club)
-            | (df.transfermarkt_link == club)
-            | (df.fcpython == club)
-            | (df.fivethirtyeight == club)
-        ]
-        club = df.transfermarkt_link.iloc[0]
-        team_id = int(df.transfermarkt.iloc[0])
+        club, team_id = _get_team_id_and_club(team_id, club)
 
     # Generate url
     try:
         page = f"https://www.transfermarkt.{domain}/{club}/kader/verein/{str(team_id)}/saison_id/{season}/plus/1"
     except IndexError:
         print("This team does not exist, please confirm spelling")
         exit()
@@ -63,115 +191,13 @@
     for row in rows:
         # check if valid row
         try:
             num = row.find("div", {"class": "rn_nummer"}).text
         except AttributeError:
             continue
 
-        # extract basic info
-        player_table = row.find("table")
-        url = player_table.find("a", href=True)["href"]
-        name = player_table.find("img")["alt"]
-        pos = player_table.find_all("tr")[1].text.strip()
-
-        # extract birth day and age
-        data = row.find_all("td", {"class": "zentriert"})
-        birth = data[1].text.strip()
-        birth = birth.split("(")
-        birth_date = birth[0].strip()
-        age = birth[1].replace(")", "").strip()
-
-        # determine if new arrival and subsequent type
-        try:
-            arrival = row.find("a")["title"]
-            if "On loan" in arrival:
-                arrival_type = "Loan"
-            elif "Returned after loan spell" in arrival:
-                arrival_type = "Returned from Loan"
-            elif "Internal transfer" in arrival:
-                arrival_type = "Internal"
-            elif "free transfer" in arrival:
-                arrival_type = "free transfer"
-            elif "Joined from":
-                arrival_type = "Transfer"
-        except KeyError:
-            arrival_type = "N/A"
-
-        # extract nation
-        nation = data[2].find("img")["alt"]
-
-        # extract height
-        try:
-            height = data[-5].text.strip()
-            height = height.replace(",", ".").replace("m", "").strip()
-        except TypeError:
-            height = None
-
-        # extract foot
-        try:
-            foot = data[-4].text.strip()
-            foot = None if foot == "-" else foot
-        except TypeError:
-            foot = None
-
-        # extract joined date
-        try:
-            joined = data[-3].text.strip()
-            joined = None if joined == "-" else joined
-        except TypeError:
-            joined = None
-
-        # extract signing information
-        try:
-            signed_from = data[-2].find("img")["alt"]
-            signed_from_url = data[-2].find("a", href=True)["href"]
-            signed_value = data[-2].find("a")["title"].split()[-1]
-            signed_currency = signed_value[0]
-            signed_value = signed_value.replace("-", "0").replace("transfer", "0")
-            if signed_value == "?":
-                signed_value = "unknown"
-            else:
-                signed_value = tm_format_currency(signed_value)
-        except TypeError:
-            signed_from = None
-            signed_from_url = None
-            signed_value = None
-            signed_currency = None
-
-        # extract contracted
-        try:
-            contracted = data[-1].text.strip()
-        except TypeError:
-            contracted = None
-
-        # extract market value
-        try:
-            mv = row.find("td", {"class": "rechts hauptlink"}).text
-            mv = tm_format_currency(mv)
-        except AttributeError:
-            mv = 0
-
-        # generate dictionary for each player
-        mydict = {
-            "name": name,
-            "url": url,
-            "number": num,
-            "position": pos,
-            "arrival_type": arrival_type,
-            "birth_date": birth_date,
-            "age": age,
-            "nation": nation,
-            "height": height,
-            "foot": foot,
-            "joined": joined,
-            "signed_from": signed_from,
-            "signed_from_url": signed_from_url,
-            "fee": signed_value,
-            "currency": signed_currency,
-            "contracted": contracted,
-            "market_value": mv,
-        }
+        mydict = _extract_player_metadata(row, num)
 
         # append dictionary to list
         mylist.append(mydict)
 
     return mylist
```

### Comparing `reus-1.1.2/reus/transfermarkt/tm_team_transfers.py` & `reus-1.1.3/reus/transfermarkt/tm_team_transfers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,32 @@
 from ..util import get_page_soup_headers
 from .util import tm_format_currency
 import pandas as pd
 
 
-def tm_team_transfers(
-    club: str,
-    season: str,
-    domain: str = "us",
-    position_group="All",
-    main_position="All",
-    window="All",
-    team_id: int = None,
-    transfermarkt_name: bool = False,
-) -> list:
-    """Extracts player transfer information
+def _get_team_id_and_club(team_id, club):
+    df = pd.read_csv(
+        "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/team_translations.csv",
+        keep_default_na=False,
+    )
+    filter_condition = (
+        (df.fbref_name == club)
+        | (df.transfermarkt_name == club)
+        | (df.transfermarkt_link == club)
+        | (df.fcpython == club)
+        | (df.fivethirtyeight == club)
+    )
+    filtered_df = df[filter_condition]
+    club = filtered_df.transfermarkt_link.iloc[0]
+    team_id = int(filtered_df.transfermarkt.iloc[0])
 
-    Args:
-        club (str): club name
-        season (str): year at start of season
-        domain (str, optional): domain to use for transfermarkt. Defaults to "us".
-        position_group (str): position group to filter by. Defaults to All.
-        main_position (str): main position to filter by. Defaults to All.
-        window (str): transfer window to filter by. Defaults to All.
-        team_id (int, optional): transfermarkt team id. Defaults to None.
-        transfermarkt_name (bool, optional): if True, club is a transfermarkt name. Defaults to False.
-
-    Returns:
-        list: team transfers
-    """
-
-    # Validate variables
-    assert position_group in [
-        "All",
-        "Goalkeepers",
-        "Defenders",
-        "Midfielders",
-        "Strikers",
-    ], "Select a valid position group"
-    assert main_position in [
-        "All",
-        "Goalkeeper",
-        "Sweeper",
-        "Centre-Back",
-        "Left-Back",
-        "Right-Back",
-        "Defensive Midfield",
-        "Central Midfield",
-        "Right Midfield",
-        "Left Midfield",
-        "Attacking Midfield",
-        "Left Winger",
-        "Right Winger",
-        "Second Striker",
-        "Centre-Forward",
-    ], "Select a valid main position"
-    assert window in ["All", "Summer", "Winter"], "Select a valid transfer window"
+    return club, team_id
 
-    if team_id is None and transfermarkt_name is False:
-        # Lookup team name
-        df = pd.read_csv(
-            "https://raw.githubusercontent.com/ian-shepherd/reus_data/main/raw-data/team_translations.csv",
-            keep_default_na=False,
-        )
-        df = df[
-            (df.fbref_name == club)
-            | (df.transfermarkt_name == club)
-            | (df.transfermarkt_link == club)
-            | (df.fcpython == club)
-            | (df.fivethirtyeight == club)
-        ]
-        club = df.transfermarkt_link.iloc[0]
-        team_id = int(df.transfermarkt.iloc[0])
 
+def _generate_subdirectory(position_group, main_position, window):
     # Determine position group subdirectory
     match position_group:
         case "All":
             pos_group_subdir = ""
         case "Goalkeepers":
             pos_group_subdir = "Torwart"
         case "Defenders":
@@ -123,49 +74,153 @@
         case "All":
             window_subdir = ""
         case "Summer":
             window_subdir = "s"
         case "Winter":
             window_subdir = "w"
 
+    return pos_group_subdir, pos_subdir, window_subdir
+
+
+def _extract_player_metadata(row, direction):
+    # row classes
+    hauptlink_class = row.find_all("td", {"class": "hauptlink"})
+    signing_class = row.find_all("img", {"class": "flaggenrahmen"})[-1]
+
+    # extract basic info
+    url = row.find("a", href=True)["href"]
+    name = row.find("img")["alt"]
+    pos = row.find("td", {"class": "hauptlink"}).find_next("td").text.strip()
+    age = row.find("td", {"class": "zentriert"}).text.strip()
+    nation = row.find_all("td", {"class": "zentriert"})[1].find("img")["alt"]
+
+    # transfer info
+    mv = row.find("td", {"class": "rechts"}).text.strip()
+    mv = mv.replace("-", "0")
+    transfer_club = hauptlink_class[1].text.strip()
+    try:
+        transfer_club_url = hauptlink_class[1].find("a", href=True)["href"]
+    except TypeError:
+        transfer_club_url = None
+    transfer_league = signing_class.find_next("a", href=True).text
+    transfer_league_url = signing_class.find_next("a", href=True)["href"]
+    transfer_country = signing_class["alt"]
+    signed_value = hauptlink_class[-1].text
+    signed_currency = signed_value[0]
+
+    # value cleaning
+    if "End of loan" in signed_value:
+        transfer_type = "End of loan"
+        signed_value = "0"
+    elif "Loan" in signed_value:
+        transfer_type = "Loan"
+        signed_value = signed_value.replace("Loan", "").replace("fee:", "").strip()
+    elif "loan transfer" in signed_value:
+        transfer_type = "Loan"
+        signed_value = "0"
+    elif "free transfer" in signed_value:
+        transfer_type = "free transfer"
+        signed_value = "0"
+    elif "?" in signed_value:
+        transfer_type = "Unknown"
+        signed_value = "0"
+    else:
+        signed_value = signed_value.replace("-", "0")
+        transfer_type = "Transfer"
+
+    # generate dictionary for each player
+    mydict = {
+        "direction": direction,
+        "transfer_type": transfer_type,
+        "name": name,
+        "url": url,
+        "position": pos,
+        "age": age,
+        "nation": nation,
+        "transfer_club": transfer_club,
+        "transfer_club_url": transfer_club_url,
+        "transfer_league": transfer_league,
+        "transfer_league_url": transfer_league_url,
+        "transfer_country": transfer_country,
+        "currency": signed_currency,
+        "fee": tm_format_currency(signed_value),
+        "market_value": tm_format_currency(mv),
+    }
+
+    return mydict
+
+
+def tm_team_transfers(
+    club: str,
+    season: str,
+    domain: str = "us",
+    position_group="All",
+    main_position="All",
+    window="All",
+    team_id: int = None,
+    transfermarkt_name: bool = False,
+) -> list:
+    """Extracts player transfer information
+
+    Args:
+        club (str): club name
+        season (str): year at start of season
+        domain (str, optional): domain to use for transfermarkt. Defaults to "us".
+        position_group (str): position group to filter by. Defaults to All.
+        main_position (str): main position to filter by. Defaults to All.
+        window (str): transfer window to filter by. Defaults to All.
+        team_id (int, optional): transfermarkt team id. Defaults to None.
+        transfermarkt_name (bool, optional): if True, club is a transfermarkt name. Defaults to False.
+
+    Returns:
+        list: team transfers
+    """
+
+    # Validate variables
+    assert position_group in [
+        "All",
+        "Goalkeepers",
+        "Defenders",
+        "Midfielders",
+        "Strikers",
+    ], "Select a valid position group"
+    assert main_position in [
+        "All",
+        "Goalkeeper",
+        "Sweeper",
+        "Centre-Back",
+        "Left-Back",
+        "Right-Back",
+        "Defensive Midfield",
+        "Central Midfield",
+        "Right Midfield",
+        "Left Midfield",
+        "Attacking Midfield",
+        "Left Winger",
+        "Right Winger",
+        "Second Striker",
+        "Centre-Forward",
+    ], "Select a valid main position"
+    assert window in ["All", "Summer", "Winter"], "Select a valid transfer window"
+
+    if team_id is None and transfermarkt_name is False:
+        club, team_id = _get_team_id_and_club(team_id, club)
+
+    pos_group_subdir, pos_subdir, window_subdir = _generate_subdirectory(
+        position_group, main_position, window
+    )
+
     # Generate url
     try:
         subdir = f"saison_id/{season}/pos/{pos_group_subdir}/detailpos/{pos_subdir}/w_s/{window_subdir}/plus/1#zugaenge"
         page = f"https://www.transfermarkt.{domain}/{club}/transfers/verein/{str(team_id)}/{subdir}"
     except IndexError:
         print("This team does not exist, please confirm spelling")
         exit()
 
-    # try:
-    #     subdir = "/".join(
-    #         (
-    #             "saison_id",
-    #             season,
-    #             "pos",
-    #             pos_group_subdir,
-    #             "detailpos",
-    #             pos_subdir,
-    #             "w_s",
-    #             window_subdir,
-    #             "plus/1#zugaenge",
-    #         )
-    #     )
-    #     page = "/".join(
-    #         (
-    #             domain,
-    #             df.transfermarkt_link.iloc[0],
-    #             "transfers/verein",
-    #             str(df.transfermarkt.iloc[0]),
-    #             subdir,
-    #         )
-    #     )
-    # except IndexError:
-    #     print("This team does not exist, please confirm spelling")
-    #     exit()
-
     pageSoup = get_page_soup_headers(page)
 
     # Find table objects
     tables = pageSoup.find_all("table", {"class": "items"})
 
     # Error handling for no transfers or non-conducive position combinations
     assert (
@@ -208,81 +263,17 @@
         # find rows
         rows = tbody.find_all("tr")
 
         # iterate through each transfer and store attributes
         for row in rows:
             # check if valid row
             try:
-                row_ = row["class"] not in ["odd", "even"]
+                row["class"] not in ["odd", "even"]
             except KeyError:
                 continue
 
-            # row classes
-            hauptlink_class = row.find_all("td", {"class": "hauptlink"})
-            signing_class = row.find_all("img", {"class": "flaggenrahmen"})[-1]
-
-            # extract basic info
-            url = row.find("a", href=True)["href"]
-            name = row.find("img")["alt"]
-            pos = row.find("td", {"class": "hauptlink"}).find_next("td").text.strip()
-            age = row.find("td", {"class": "zentriert"}).text.strip()
-            nation = row.find_all("td", {"class": "zentriert"})[1].find("img")["alt"]
-
-            # transfer info
-            mv = row.find("td", {"class": "rechts"}).text.strip()
-            mv = mv.replace("-", "0")
-            transfer_club = hauptlink_class[1].text.strip()
-            try:
-                transfer_club_url = hauptlink_class[1].find("a", href=True)["href"]
-            except TypeError:
-                transfer_club_url = None
-            transfer_league = signing_class.find_next("a", href=True).text
-            transfer_league_url = signing_class.find_next("a", href=True)["href"]
-            transfer_country = signing_class["alt"]
-            signed_value = hauptlink_class[-1].text
-            signed_currency = signed_value[0]
-
-            # value cleaning
-            if "End of loan" in signed_value:
-                transfer_type = "End of loan"
-                signed_value = "0"
-            elif "Loan" in signed_value:
-                transfer_type = "Loan"
-                signed_value = (
-                    signed_value.replace("Loan", "").replace("fee:", "").strip()
-                )
-            elif "loan transfer" in signed_value:
-                transfer_type = "Loan"
-                signed_value = "0"
-            elif "free transfer" in signed_value:
-                transfer_type = "free transfer"
-                signed_value = "0"
-            elif "?" in signed_value:
-                transfer_type = "Unknown"
-                signed_value = "0"
-            else:
-                signed_value = signed_value.replace("-", "0")
-                transfer_type = "Transfer"
-
-            # generate dictionary for each player
-            mydict = {
-                "direction": direction,
-                "transfer_type": transfer_type,
-                "name": name,
-                "url": url,
-                "position": pos,
-                "age": age,
-                "nation": nation,
-                "transfer_club": transfer_club,
-                "transfer_club_url": transfer_club_url,
-                "transfer_league": transfer_league,
-                "transfer_league_url": transfer_league_url,
-                "transfer_country": transfer_country,
-                "currency": signed_currency,
-                "fee": tm_format_currency(signed_value),
-                "market_value": tm_format_currency(mv),
-            }
+            mydict = _extract_player_metadata(row, direction)
 
             # append dictionary to list
             mylist.append(mydict)
 
     return mylist
```

### Comparing `reus-1.1.2/reus/transfermarkt/util.py` & `reus-1.1.3/reus/transfermarkt/util.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus/util.py` & `reus-1.1.3/reus/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from bs4 import BeautifulSoup
 
 
 def get_page_soup(url: str, save_html: bool = False) -> BeautifulSoup:
     """Returns html of a given url
 
     Args:
-        url (str): _description_
+        url (str): The URL to fetch the HTML from.
+        save_html (bool): Whether to save the HTML content or not.
 
     Returns:
         bs4: pageSoup
     """
 
     pageTree = requests.get(url)
     pageSoup = BeautifulSoup(pageTree.content, "html.parser")
@@ -21,23 +22,23 @@
         return pageSoup
 
 
 def get_page_soup_headers(url: str, save_html: bool = False) -> BeautifulSoup:
     """Returns html of a given url
 
     Args:
-        url (str): _description_
+        url (str): The URL to fetch the HTML from.
+        save_html (bool): Whether to save the HTML content or not.
 
     Returns:
         bs4: pageSoup
     """
 
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36"
-    }
+    USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36"  # noqa: E501
+    headers = {"User-Agent": USER_AGENT}
 
     pageTree = requests.get(url, headers=headers)
     pageSoup = BeautifulSoup(pageTree.content, "html.parser")
 
     if save_html:
         return pageSoup, pageTree.content
     else:
```

### Comparing `reus-1.1.2/reus/utils/generate_standings.py` & `reus-1.1.3/reus/utils/generate_standings.py`

 * *Files identical despite different names*

### Comparing `reus-1.1.2/reus.egg-info/PKG-INFO` & `reus-1.1.3/reus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reus
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package that allows you to soccer information
 Home-page: https://github.com/ian-shepherd/reus
 Author: Ian Shepherd
 License: UNKNOWN
 Keywords: python,fbref,fotmob,transfermarkt,soccer,football
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reus-1.1.2/setup.py` & `reus-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 DESCRIPTION = "A package that allows you to soccer information"
 LONG_DESCRIPTION = """
     A package that allows you to pull soccer statistics, player market values, and
      transfer information, primarily from FBref, Fotmob, and Transfermarkt"""
 
 setuptools.setup(
     name="reus",
```

