# Comparing `tmp/line-bot-sdk-2.4.2.tar.gz` & `tmp/line-bot-sdk-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-bot-sdk-2.4.2.tar", last modified: Mon Mar 13 02:21:26 2023, max compression
+gzip compressed data, was "line-bot-sdk-2.4.3.tar", last modified: Fri Jun 30 01:47:51 2023, max compression
```

## Comparing `line-bot-sdk-2.4.2.tar` & `line-bot-sdk-2.4.3.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.970447 line-bot-sdk-2.4.2/
--rw-r--r--   0 yutakasai   (503) staff       (20)    11347 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/LICENSE
--rw-r--r--   0 yutakasai   (503) staff       (20)      244 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/MANIFEST.in
--rw-r--r--   0 yutakasai   (503) staff       (20)    46240 2023-03-13 02:21:26.970625 line-bot-sdk-2.4.2/PKG-INFO
--rw-r--r--   0 yutakasai   (503) staff       (20)    45423 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/README.rst
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.934257 line-bot-sdk-2.4.2/docs/
--rw-r--r--   0 yutakasai   (503) staff       (20)     7667 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/Makefile
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.935452 line-bot-sdk-2.4.2/docs/source/
--rw-r--r--   0 yutakasai   (503) staff       (20)    10166 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/conf.py
--rw-r--r--   0 yutakasai   (503) staff       (20)      430 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/index.rst
--rw-r--r--   0 yutakasai   (503) staff       (20)     1959 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/linebot.models.rst
--rw-r--r--   0 yutakasai   (503) staff       (20)      457 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/docs/source/linebot.rst
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.937310 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/
--rw-r--r--   0 yutakasai   (503) staff       (20)    46240 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yutakasai   (503) staff       (20)     3287 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)        1 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       39 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/requires.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)        8 2023-03-13 02:21:26.000000 line-bot-sdk-2.4.2/line_bot_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.942800 line-bot-sdk-2.4.2/linebot/
--rw-r--r--   0 yutakasai   (503) staff       (20)      781 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/__about__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1056 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5946 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/aiohttp_async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    86776 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/api.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    88701 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/async_api.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5099 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3198 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/exceptions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    10498 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/http_client.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.950567 line-bot-sdk-2.4.2/linebot/models/
--rw-r--r--   0 yutakasai   (503) staff       (20)     4846 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9405 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/actions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1939 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/background.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3795 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/base.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1107 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/delivery_context.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1183 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/emojis.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1845 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/error.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    19053 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/events.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4941 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/filter.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    26498 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/flex_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     7011 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/imagemap.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    10480 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/insight.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1132 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/limit.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1180 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/mention.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1351 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/mentionee.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2403 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/operator.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2083 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/recipient.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    38321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/responses.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5012 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/rich_menu.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9375 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/send_messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3831 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/sources.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9133 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/template.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4718 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/things.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1065 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/unsend.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1210 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/models/video_play_complete.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1715 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/utils.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9610 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/linebot/webhook.py
--rw-r--r--   0 yutakasai   (503) staff       (20)      111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements-dev.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       55 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements-test.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       41 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/requirements.txt
--rw-r--r--   0 yutakasai   (503) staff       (20)       92 2023-03-13 02:21:26.971117 line-bot-sdk-2.4.2/setup.cfg
--rw-r--r--   0 yutakasai   (503) staff       (20)     7321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/setup.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.952125 line-bot-sdk-2.4.2/tests/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/__init__.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.964887 line-bot-sdk-2.4.2/tests/api/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6321 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_channel_access_token_v2_1.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4433 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_error_handle.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2073 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_bot_info.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1132 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_content.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4401 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_custom_aggregation_units.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3393 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_delivery.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2374 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_group.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    12659 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_insight.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6651 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_member_ids.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2750 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_member_profile.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2333 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_message_quota.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1948 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_profile.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1470 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_room.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1649 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_get_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2541 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_issue_channel_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1548 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_issue_link_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1836 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_leave.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    14943 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_narrowcast_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1565 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_revoke_channel_token.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    17746 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_rich_menu.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6049 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_rich_menu_alias.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3497 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_audio_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3558 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_image_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5876 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_imagemap_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3617 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_location_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3411 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_sticker_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    22270 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_template_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     8052 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6111 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_quick_reply.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2476 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_sender.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5440 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3631 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_send_video_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1456 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_set_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1892 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_test_webhook_endpoint.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     5204 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/api/test_validate_message_objects.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.966024 line-bot-sdk-2.4.2/tests/async_api/
--rw-r--r--   0 yutakasai   (503) staff       (20)     1688 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_async_error_handle.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1357 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_get_message_content.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1518 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/async_api/test_get_profile.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.969396 line-bot-sdk-2.4.2/tests/models/
--rw-r--r--   0 yutakasai   (503) staff       (20)      580 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/__init__.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2551 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/serialize_test_case.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3203 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_actions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1223 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_background.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2959 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_base.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2213 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_filter.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     9117 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_flex_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4112 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_imagemap.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     4084 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_send_messages.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     6757 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_template.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2721 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/models/test_text_message.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     3168 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_aiohttp_async_http_client.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     2662 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_exceptions.py
--rw-r--r--   0 yutakasai   (503) staff       (20)     1820 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_utils.py
--rw-r--r--   0 yutakasai   (503) staff       (20)    39339 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/test_webhook.py
-drwxr-xr-x   0 yutakasai   (503) staff       (20)        0 2023-03-13 02:21:26.969748 line-bot-sdk-2.4.2/tests/text/
--rw-r--r--   0 yutakasai   (503) staff       (20)    15137 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tests/text/webhook.json
--rw-r--r--   0 yutakasai   (503) staff       (20)      564 2023-03-13 02:21:10.000000 line-bot-sdk-2.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45423 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.455355 line-bot-sdk-2.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.455355 line-bot-sdk-2.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/linebot.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/docs/source/linebot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 01:47:51.000000 line-bot-sdk-2.4.3/line_bot_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/linebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86776 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88701 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/async_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/linebot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/delivery_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/mention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/mentionee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/unsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/models/video_play_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/linebot/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.459355 line-bot-sdk-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_channel_access_token_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_custom_aggregation_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_member_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_member_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_message_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_get_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_issue_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_issue_link_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_leave.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_narrowcast_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_revoke_channel_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_rich_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_rich_menu_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_audio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_image_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_imagemap_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_location_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_sticker_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_template_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_quick_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_send_video_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_set_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/api/test_validate_message_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/async_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_async_error_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_get_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/async_api/test_get_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.463355 line-bot-sdk-2.4.3/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/serialize_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_flex_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_imagemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_send_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/models/test_text_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_aiohttp_async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 01:47:51.471355 line-bot-sdk-2.4.3/tests/text/
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tests/text/webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 01:47:42.000000 line-bot-sdk-2.4.3/tox.ini
```

### Comparing `line-bot-sdk-2.4.2/LICENSE` & `line-bot-sdk-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/PKG-INFO` & `line-bot-sdk-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: line-bot-sdk
-Version: 2.4.2
+Version: 2.4.3
 Summary: LINE Messaging API SDK for Python
 Home-page: https://github.com/line/line-bot-sdk-python
 Author: RyosukeHasebe
 Author-email: hsb.1014@gmail.com
 Maintainer: RyosukeHasebe
 Maintainer-email: hsb.1014@gmail.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -1620,9 +1619,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
-
-
```

### Comparing `line-bot-sdk-2.4.2/README.rst` & `line-bot-sdk-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/docs/Makefile` & `line-bot-sdk-2.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/docs/source/conf.py` & `line-bot-sdk-2.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/docs/source/linebot.models.rst` & `line-bot-sdk-2.4.3/docs/source/linebot.models.rst`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/line_bot_sdk.egg-info/PKG-INFO` & `line-bot-sdk-2.4.3/line_bot_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: line-bot-sdk
-Version: 2.4.2
+Version: 2.4.3
 Summary: LINE Messaging API SDK for Python
 Home-page: https://github.com/line/line-bot-sdk-python
 Author: RyosukeHasebe
 Author-email: hsb.1014@gmail.com
 Maintainer: RyosukeHasebe
 Maintainer-email: hsb.1014@gmail.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -1620,9 +1619,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
-
-
```

### Comparing `line-bot-sdk-2.4.2/line_bot_sdk.egg-info/SOURCES.txt` & `line-bot-sdk-2.4.3/line_bot_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/__about__.py` & `line-bot-sdk-2.4.3/linebot/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations
 #  under the License.
 
 """Meta data of line-bot-sdk."""
 
 
-__version__ = '2.4.2'
+__version__ = '2.4.3'
 __author__ = 'LINE Corporation'
 __copyright__ = 'Copyright 2016, LINE Corporation'
 __license__ = 'Apache 2.0'
 
 __all__ = (
     '__version__'
 )
```

### Comparing `line-bot-sdk-2.4.2/linebot/__init__.py` & `line-bot-sdk-2.4.3/linebot/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/aiohttp_async_http_client.py` & `line-bot-sdk-2.4.3/linebot/aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/api.py` & `line-bot-sdk-2.4.3/linebot/api.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/async_api.py` & `line-bot-sdk-2.4.3/linebot/async_api.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/async_http_client.py` & `line-bot-sdk-2.4.3/linebot/async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/exceptions.py` & `line-bot-sdk-2.4.3/linebot/exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/http_client.py` & `line-bot-sdk-2.4.3/linebot/http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/__init__.py` & `line-bot-sdk-2.4.3/linebot/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     MemberLeftEvent,
     BeaconEvent,
     ThingsEvent,
     UnknownEvent,
     Postback,
     Beacon,
     Link,
+    VideoPlayCompleteEvent,
+    UnsendEvent,
 )
 from .filter import (  # noqa
     Filter,
     DemographicFilter,
     GenderFilter,
     AppTypeFilter,
     AreaFilter,
```

### Comparing `line-bot-sdk-2.4.2/linebot/models/actions.py` & `line-bot-sdk-2.4.3/linebot/models/actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/background.py` & `line-bot-sdk-2.4.3/linebot/models/background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/base.py` & `line-bot-sdk-2.4.3/linebot/models/base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/delivery_context.py` & `line-bot-sdk-2.4.3/linebot/models/delivery_context.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/emojis.py` & `line-bot-sdk-2.4.3/linebot/models/emojis.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/error.py` & `line-bot-sdk-2.4.3/linebot/models/error.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/events.py` & `line-bot-sdk-2.4.3/linebot/models/events.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/filter.py` & `line-bot-sdk-2.4.3/linebot/models/filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/flex_message.py` & `line-bot-sdk-2.4.3/linebot/models/flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/imagemap.py` & `line-bot-sdk-2.4.3/linebot/models/imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/insight.py` & `line-bot-sdk-2.4.3/linebot/models/insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/limit.py` & `line-bot-sdk-2.4.3/linebot/models/limit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/mention.py` & `line-bot-sdk-2.4.3/linebot/models/mention.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/mentionee.py` & `line-bot-sdk-2.4.3/linebot/models/mentionee.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/messages.py` & `line-bot-sdk-2.4.3/linebot/models/messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/operator.py` & `line-bot-sdk-2.4.3/linebot/models/operator.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/recipient.py` & `line-bot-sdk-2.4.3/linebot/models/recipient.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/responses.py` & `line-bot-sdk-2.4.3/linebot/models/responses.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/rich_menu.py` & `line-bot-sdk-2.4.3/linebot/models/rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/send_messages.py` & `line-bot-sdk-2.4.3/linebot/models/send_messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/sources.py` & `line-bot-sdk-2.4.3/linebot/models/sources.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/template.py` & `line-bot-sdk-2.4.3/linebot/models/template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/things.py` & `line-bot-sdk-2.4.3/linebot/models/things.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/unsend.py` & `line-bot-sdk-2.4.3/linebot/models/unsend.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/models/video_play_complete.py` & `line-bot-sdk-2.4.3/linebot/models/video_play_complete.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/utils.py` & `line-bot-sdk-2.4.3/linebot/utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/linebot/webhook.py` & `line-bot-sdk-2.4.3/linebot/webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/setup.py` & `line-bot-sdk-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/__init__.py` & `line-bot-sdk-2.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/__init__.py` & `line-bot-sdk-2.4.3/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_channel_access_token_v2_1.py` & `line-bot-sdk-2.4.3/tests/api/test_channel_access_token_v2_1.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_error_handle.py` & `line-bot-sdk-2.4.3/tests/api/test_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_bot_info.py` & `line-bot-sdk-2.4.3/tests/api/test_get_bot_info.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_content.py` & `line-bot-sdk-2.4.3/tests/api/test_get_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_custom_aggregation_units.py` & `line-bot-sdk-2.4.3/tests/api/test_get_custom_aggregation_units.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_delivery.py` & `line-bot-sdk-2.4.3/tests/api/test_get_delivery.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_group.py` & `line-bot-sdk-2.4.3/tests/api/test_get_group.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_insight.py` & `line-bot-sdk-2.4.3/tests/api/test_get_insight.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_member_ids.py` & `line-bot-sdk-2.4.3/tests/api/test_get_member_ids.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_member_profile.py` & `line-bot-sdk-2.4.3/tests/api/test_get_member_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_message_quota.py` & `line-bot-sdk-2.4.3/tests/api/test_get_message_quota.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_profile.py` & `line-bot-sdk-2.4.3/tests/api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_room.py` & `line-bot-sdk-2.4.3/tests/api/test_get_room.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_get_webhook_endpoint.py` & `line-bot-sdk-2.4.3/tests/api/test_get_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_issue_channel_token.py` & `line-bot-sdk-2.4.3/tests/api/test_issue_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_issue_link_token.py` & `line-bot-sdk-2.4.3/tests/api/test_issue_link_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_leave.py` & `line-bot-sdk-2.4.3/tests/api/test_leave.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_narrowcast_message.py` & `line-bot-sdk-2.4.3/tests/api/test_narrowcast_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_revoke_channel_token.py` & `line-bot-sdk-2.4.3/tests/api/test_revoke_channel_token.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_rich_menu.py` & `line-bot-sdk-2.4.3/tests/api/test_rich_menu.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_rich_menu_alias.py` & `line-bot-sdk-2.4.3/tests/api/test_rich_menu_alias.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_audio_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_audio_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_image_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_image_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_imagemap_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_imagemap_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_location_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_location_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_sticker_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_sticker_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_template_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_template_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_text_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_quick_reply.py` & `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_quick_reply.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_sender.py` & `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_sender.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py` & `line-bot-sdk-2.4.3/tests/api/test_send_text_message_with_statistics_per_aggregation_unit.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_send_video_message.py` & `line-bot-sdk-2.4.3/tests/api/test_send_video_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_set_webhook_endpoint.py` & `line-bot-sdk-2.4.3/tests/api/test_set_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_test_webhook_endpoint.py` & `line-bot-sdk-2.4.3/tests/api/test_test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/api/test_validate_message_objects.py` & `line-bot-sdk-2.4.3/tests/api/test_validate_message_objects.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/async_api/test_async_error_handle.py` & `line-bot-sdk-2.4.3/tests/async_api/test_async_error_handle.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/async_api/test_get_message_content.py` & `line-bot-sdk-2.4.3/tests/async_api/test_get_message_content.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/async_api/test_get_profile.py` & `line-bot-sdk-2.4.3/tests/async_api/test_get_profile.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/__init__.py` & `line-bot-sdk-2.4.3/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/serialize_test_case.py` & `line-bot-sdk-2.4.3/tests/models/serialize_test_case.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_actions.py` & `line-bot-sdk-2.4.3/tests/models/test_actions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_background.py` & `line-bot-sdk-2.4.3/tests/models/test_background.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_base.py` & `line-bot-sdk-2.4.3/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_filter.py` & `line-bot-sdk-2.4.3/tests/models/test_filter.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_flex_message.py` & `line-bot-sdk-2.4.3/tests/models/test_flex_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_imagemap.py` & `line-bot-sdk-2.4.3/tests/models/test_imagemap.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_send_messages.py` & `line-bot-sdk-2.4.3/tests/models/test_send_messages.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_template.py` & `line-bot-sdk-2.4.3/tests/models/test_template.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/models/test_text_message.py` & `line-bot-sdk-2.4.3/tests/models/test_text_message.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_aiohttp_async_http_client.py` & `line-bot-sdk-2.4.3/tests/test_aiohttp_async_http_client.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_exceptions.py` & `line-bot-sdk-2.4.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_utils.py` & `line-bot-sdk-2.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/test_webhook.py` & `line-bot-sdk-2.4.3/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tests/text/webhook.json` & `line-bot-sdk-2.4.3/tests/text/webhook.json`

 * *Files identical despite different names*

### Comparing `line-bot-sdk-2.4.2/tox.ini` & `line-bot-sdk-2.4.3/tox.ini`

 * *Files identical despite different names*

