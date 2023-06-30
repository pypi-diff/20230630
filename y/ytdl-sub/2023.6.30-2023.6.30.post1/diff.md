# Comparing `tmp/ytdl-sub-2023.6.30.tar.gz` & `tmp/ytdl-sub-2023.6.30.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2023.6.30.tar", last modified: Fri Jun 30 06:59:08 2023, max compression
+gzip compressed data, was "ytdl-sub-2023.6.30.post1.tar", last modified: Fri Jun 30 18:53:04 2023, max compression
```

## Comparing `ytdl-sub-2023.6.30.tar` & `ytdl-sub-2023.6.30.post1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.325631 ytdl-sub-2023.6.30/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-30 06:59:08.325631 ytdl-sub-2023.6.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-30 06:59:08.325631 ytdl-sub-2023.6.30/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.309631 ytdl-sub-2023.6.30/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 06:58:52.000000 ytdl-sub-2023.6.30/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/cli/download_args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/cli/main_args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/preset_class_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/base_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/multi_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/entry_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/file_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.317631 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.321631 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.321631 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.321631 ytdl-sub-2023.6.30/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.321631 ytdl-sub-2023.6.30/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.325631 ytdl-sub-2023.6.30/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.325631 ytdl-sub-2023.6.30/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-30 06:58:51.000000 ytdl-sub-2023.6.30/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:59:08.313631 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 06:59:08.000000 ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.863576 ytdl-sub-2023.6.30.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.867576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-30 18:52:49.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.867576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/download_args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/main_args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.867576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset_class_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.867576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/base_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.871576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.871576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.871576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.871576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/entry_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.871576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/file_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/helpers/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21584 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.875576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.879576 ytdl-sub-2023.6.30.post1/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21151 2023-06-30 18:52:48.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 18:53:04.867576 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 18:53:04.000000 ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2023.6.30/LICENSE` & `ytdl-sub-2023.6.30.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/PKG-INFO` & `ytdl-sub-2023.6.30.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.6.30
+Version: 2023.6.30.post1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.6.30/README.md` & `ytdl-sub-2023.6.30.post1/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/pyproject.toml` & `ytdl-sub-2023.6.30.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 disable = [
     "C0115", # Missing class docstring
     "C0114", # missing-module-docstring
     "R0903", # too-few-public-methods
     "R0801", # similar lines
     "R0913", # Too many arguments
     "R0901", # too-many-ancestors
+    "R0902", # too-many-instance-attributes
     "W0511", # TODO
 ]
 
 load-plugins = "pylint.extensions.docparams"
 
 [tool.pydocstyle]
 inherit = false
```

### Comparing `ytdl-sub-2023.6.30/setup.cfg` & `ytdl-sub-2023.6.30.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/cli/download_args_parser.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/download_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/cli/main.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/cli/main_args_parser.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/cli/main_args_parser.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/config_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     def keep_successful_logs(self) -> bool:
         """
         Optional. Whether to store logs when downloading is successful. Defaults to True.
         """
         return self._keep_successful_logs.value
 
 
-# pylint: disable=too-many-instance-attributes
 class ConfigOptions(StrictDictValidator):
     _required_keys = {"working_directory"}
     _optional_keys = {
         "umask",
         "dl_aliases",
         "persist_logs",
         "lock_directory",
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/config/preset.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/config/preset_class_mappings.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset_class_mappings.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/config/preset_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 from yt_dlp.utils import sanitize_filename
 
+from ytdl_sub.config.defaults import DEFAULT_DOWNLOAD_ARCHIVE_NAME
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.validators.file_path_validators import OverridesStringFormatterFilePathValidator
 from ytdl_sub.validators.file_path_validators import StringFormatterFileNameValidator
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_datetime import StringDatetimeValidator
 from ytdl_sub.validators.string_formatter_validators import DictFormatterValidator
@@ -231,24 +232,25 @@
            output_options:
              # required
              output_directory: "/path/to/videos_or_music"
              file_name: "{title_sanitized}.{ext}"
              # optional
              thumbnail_name: "{title_sanitized}.{thumbnail_ext}"
              info_json_name: "{title_sanitized}.{info_json_ext}"
+             download_archive_name: ".ytdl-sub-{subscription_name}-download-archive.txt"
              maintain_download_archive: True
              keep_files_before: now
              keep_files_after: 19000101
     """
 
     _required_keys = {"output_directory", "file_name"}
     _optional_keys = {
         "thumbnail_name",
         "info_json_name",
-        "subtitles_name",
+        "download_archive_name",
         "maintain_download_archive",
         "keep_files_before",
         "keep_files_after",
     }
 
     @classmethod
     def partial_validate(cls, name: str, value: Any) -> None:
@@ -278,14 +280,20 @@
         self._thumbnail_name = self._validate_key_if_present(
             key="thumbnail_name", validator=StringFormatterFileNameValidator
         )
         self._info_json_name = self._validate_key_if_present(
             key="info_json_name", validator=StringFormatterFileNameValidator
         )
 
+        self._download_archive_name = self._validate_key_if_present(
+            key="download_archive_name",
+            validator=OverridesStringFormatterValidator,
+            default=DEFAULT_DOWNLOAD_ARCHIVE_NAME,
+        )
+
         self._maintain_download_archive = self._validate_key_if_present(
             key="maintain_download_archive", validator=BoolValidator, default=False
         )
 
         self._keep_files_before = self._validate_key_if_present(
             "keep_files_before", StringDatetimeValidator
         )
@@ -330,14 +338,22 @@
         Optional. The file name for the media's info json file. This can include directories such
         as ``"Season {upload_year}/{title}.{info_json_ext}"``, and will be placed in the output
         directory. Can be set to empty string or `null` to disable info json writes.
         """
         return self._info_json_name
 
     @property
+    def download_archive_name(self) -> Optional[OverridesStringFormatterValidator]:
+        """
+        Optional. The file name to store a subscriptions download archive placed relative to
+        the output directory. Defaults to ``.ytdl-sub-{subscription_name}-download-archive.txt``
+        """
+        return self._download_archive_name
+
+    @property
     def maintain_download_archive(self) -> bool:
         """
         Optional. Maintains a download archive file in the output directory for a subscription.
         It is named ``.ytdl-sub-{subscription_name}-download-archive.json``, stored in the
         output directory.
 
         The download archive contains a mapping of ytdl IDs to downloaded files. This is used to
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/base_downloader.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.logger import Logger
 from ytdl_sub.utils.thumbnail import ThumbnailTypes
 from ytdl_sub.utils.thumbnail import convert_download_thumbnail
 from ytdl_sub.utils.thumbnail import download_and_convert_url_thumbnail
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
-# pylint: disable=too-many-instance-attributes
-
 download_logger = Logger.get(name="downloader")
 
 
 class DownloaderValidator(BaseDownloaderValidator, ABC):
     """
     Placeholder class to define downloader options
     """
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/multi_url.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/multi_url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/url.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/url.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/entry_variables.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/entry_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/entries/variables/kwargs.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/entries/variables/kwargs.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/main.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/plugin.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/helpers/__init__.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         preset_options: Preset
         """
         self.name = name
         self._config_options = config_options
         self._preset_options = preset_options
 
         self._enhanced_download_archive = EnhancedDownloadArchive(
-            subscription_name=name,
+            file_name=self.overrides.apply_formatter(self.output_options.download_archive_name),
             working_directory=self.working_directory,
             output_directory=self.output_directory,
         )
 
     @property
     def downloader_class(self) -> Type[BaseDownloader]:
         """
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,15 @@
                 after=self.output_options.keep_files_after,
                 overrides=self.overrides,
             )
             if date_range_to_keep:
                 self._enhanced_download_archive.remove_stale_files(date_range=date_range_to_keep)
 
             self._enhanced_download_archive.save_download_mappings()
-            FileHandler.delete(self._enhanced_download_archive.archive_working_file_path)
-            FileHandler.delete(self._enhanced_download_archive.mapping_working_file_path)
+            FileHandler.delete(self._enhanced_download_archive.working_file_path)
 
     @contextlib.contextmanager
     def _remove_empty_directories_in_output_directory(self):
         try:
             yield
         finally:
             if not self._enhanced_download_archive.is_dry_run:
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         return {"break_on_reject": True}
 
     @property
     def _output_options(self) -> Dict:
         ytdl_options = {}
 
         if self._preset.output_options.maintain_download_archive:
-            ytdl_options["download_archive"] = str(
-                Path(self._working_directory) / self._enhanced_download_archive.archive_file_name
-            )
+            ytdl_options["download_archive"] = self._enhanced_download_archive.working_file_path
 
         return ytdl_options
 
     def _plugin_ytdl_options(self, plugin: Type[PluginT]) -> Dict:
         if not (audio_extract_plugin := self._get_plugin(plugin)):
             return {}
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from yt_dlp.utils import make_archive_id
 
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.variables.kwargs import SPLIT_BY_CHAPTERS_PARENT_ENTRY
 from ytdl_sub.utils.file_handler import FileHandler
 from ytdl_sub.utils.file_handler import FileHandlerTransactionLog
 from ytdl_sub.utils.file_handler import FileMetadata
-from ytdl_sub.utils.logger import Logger
 
 
 @dataclass
 class DownloadMapping:
     upload_date: str
     extractor: str
     file_names: Set[str]
@@ -366,29 +365,27 @@
         # If a mapping file exists in the output directory, load it up.
         if os.path.isfile(mapping_file_path):
             return DownloadMappings.from_file(json_file_path=mapping_file_path)
         return DownloadMappings()
 
     def __init__(
         self,
-        subscription_name: str,
+        file_name: str,
         working_directory: str,
         output_directory: str,
         dry_run: bool = False,
     ):
-        self.subscription_name = subscription_name
+        self._file_name = file_name
         self._file_handler = FileHandler(
             working_directory=working_directory, output_directory=output_directory, dry_run=dry_run
         )
         self._download_mapping = self._maybe_load_download_mappings(
-            mapping_file_path=self._mapping_output_file_path
+            mapping_file_path=self.output_file_path
         )
 
-        self._logger = Logger.get(name=subscription_name)
-
         self.num_entries_added: int = 0
         self.num_entries_modified: int = 0
         self.num_entries_removed: int = 0
 
     @property
     def num_entries(self) -> int:
         """
@@ -414,38 +411,28 @@
         """
         self._file_handler = FileHandler(
             working_directory=self.working_directory,
             output_directory=self.output_directory,
             dry_run=dry_run,
         )
         self._download_mapping = self._maybe_load_download_mappings(
-            mapping_file_path=self._mapping_output_file_path
+            mapping_file_path=self.output_file_path
         )
         return self
 
     @property
     def is_dry_run(self) -> bool:
         """
         Returns
         -------
         True if this session is a dry-run. False otherwise.
         """
         return self._file_handler.dry_run
 
     @property
-    def archive_file_name(self) -> str:
-        """
-        Returns
-        -------
-        The download archive's file name (no path)
-        Used to recreate yt-dlp's download archive in the working directory
-        """
-        return f".ytdl-sub-{self.subscription_name}-download-archive.txt"
-
-    @property
     def working_directory(self) -> str:
         """
         Returns
         -------
         Path to the working directory
         """
         return self._file_handler.working_directory
@@ -456,48 +443,39 @@
         Returns
         -------
         Path to the output directory
         """
         return self._file_handler.output_directory
 
     @property
-    def _mapping_file_name(self) -> str:
+    def file_name(self) -> str:
         """
         Returns
         -------
         The download mapping's file name (no path)
         """
-        return f".ytdl-sub-{self.subscription_name}-download-archive.json"
+        return self._file_name
 
     @property
-    def _mapping_output_file_path(self) -> str:
+    def output_file_path(self) -> str:
         """
         Returns
         -------
         The download mapping's file path in the output directory.
         """
-        return str(Path(self.output_directory) / self._mapping_file_name)
+        return str(Path(self.output_directory) / self.file_name)
 
     @property
-    def mapping_working_file_path(self) -> str:
+    def working_file_path(self) -> str:
         """
         Returns
         -------
         The download mapping's file path in the working directory.
         """
-        return str(Path(self.working_directory) / self._mapping_file_name)
-
-    @property
-    def archive_working_file_path(self) -> str:
-        """
-        Returns
-        -------
-        The download archive's file path in the working directory.
-        """
-        return str(Path(self.working_directory) / self.archive_file_name)
+        return str(Path(self.working_directory) / self.file_name)
 
     @property
     def mapping(self) -> DownloadMappings:
         """
         Returns
         -------
         Loaded DownloadMappings
@@ -522,15 +500,15 @@
         """
         # If the download mapping is empty, do nothing since the ytdl downloader will create a new
         # download archive file
         if self.mapping.is_empty:
             return self
 
         # Otherwise, create a ytdl download archive file in the working directory.
-        self.mapping.to_download_archive().to_file(self.archive_working_file_path)
+        self.mapping.to_download_archive().to_file(self.working_file_path)
 
         return self
 
     def remove_stale_files(self, date_range: DateRange) -> "EnhancedDownloadArchive":
         """
         Checks all entries within the mappings. If any entries' upload dates are not within the
         provided date range, delete them.
@@ -562,16 +540,16 @@
         Saves the updated download mappings to the output directory if any files were changed.
 
         Returns
         -------
         self
         """
         if not self.get_file_handler_transaction_log().is_empty:
-            self._download_mapping.to_file(output_json_file=self.mapping_working_file_path)
-            self.save_file_to_output_directory(file_name=self._mapping_file_name)
+            self._download_mapping.to_file(output_json_file=self.working_file_path)
+            self.save_file_to_output_directory(file_name=self.file_name)
         return self
 
     def delete_file_from_output_directory(self, file_name: str):
         """
         Deletes a file from the output directory
 
         Parameters
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2023.6.30
+Version: 2023.6.30.post1
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2023.6.30/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2023.6.30.post1/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

