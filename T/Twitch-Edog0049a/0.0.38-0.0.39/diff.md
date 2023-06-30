# Comparing `tmp/twitch_edog0049a-0.0.38.tar.gz` & `tmp/twitch_edog0049a-0.0.39.tar.gz`

## Comparing `twitch_edog0049a-0.0.38.tar` & `twitch_edog0049a-0.0.39.tar`

### file list

```diff
@@ -1,80 +1,84 @@
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/Twitch.code-workspace
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/dddd.cfgd
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/CallbackServer/CallbackServer.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/CallbackServer/__init__.py
--rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/Scope.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/SubscriptionTypes.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Exceptions.py
--rw-r--r--   0        0        0    37750 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/TwitchAPI.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/_ApiRequest.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/__init__.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/api flow.svg
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Ads.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Analytics.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Bits.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ChannelPoints.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Channels.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Charity.py
--rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Chat.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Clips.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Entitlements.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/EventSub.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Extensions.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Games.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Goals.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/HypeTrain.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/JWTGeneraotr.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Moderation.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Music.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Polls.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Predictions.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Raids.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ResponseTypes.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Schedule.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Search.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Streams.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Subscriptions.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Tags.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Teams.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Users.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Utils.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Videos.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Whispers.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__imports.py
--rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Ads_test.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Bits_Test.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/Exceptions.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/IrcController.py
--rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/MessageHandler.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TokenBucket.py
--rw-r--r--   0        0        0    22973 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/__init__.py
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventHandler/EventHandler.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventHandler/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/EventSubConnector.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/EventSubInterface.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/__init__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Exceptions.py
--rw-r--r--   0        0        0    39494 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth flow.svg
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/test/oauthtest.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubConnector.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubInterface.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/Topics.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/WebsocketClient.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/client_run_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/test/__init__.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/test/test1.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/pyproject.toml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/Twitch.code-workspace
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/dddd.cfgd
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/CallbackServer/CallbackServer.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/CallbackServer/__init__.py
+-rw-r--r--   0        0        0    63944 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/distbackup/twitch_edog0049a-0.0.38-py3-none-any.whl
+-rw-r--r--   0        0        0   247556 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/distbackup/twitch_edog0049a-0.0.38.tar.gz
+-rw-r--r--   0        0        0    63945 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/distbackup/twitch_edog0049a-0.0.39-py3-none-any.whl
+-rw-r--r--   0        0        0   350071 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/distbackup/twitch_edog0049a-0.0.39.tar.gz
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/Scope.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/SubscriptionTypes.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Exceptions.py
+-rw-r--r--   0        0        0    37750 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/TwitchAPI.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/_ApiRequest.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/__init__.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/api flow.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Ads.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Analytics.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Bits.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/ChannelPoints.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Channels.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Charity.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Chat.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Clips.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Entitlements.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/EventSub.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Extensions.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Games.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Goals.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/HypeTrain.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/JWTGeneraotr.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Moderation.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Music.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Polls.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Predictions.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Raids.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/ResponseTypes.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Schedule.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Search.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Streams.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Subscriptions.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Tags.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Teams.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Users.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Utils.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Videos.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Whispers.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/__imports.py
+-rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/Resources/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/test/Ads_test.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/test/Bits_Test.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/test/Utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/API/test/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/Exceptions.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/IrcController.py
+-rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/MessageHandler.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/TokenBucket.py
+-rw-r--r--   0        0        0    22973 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/TwitchChatInterface.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/__init__.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/EventHandler/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/EventSub/EventSubConnector.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/EventSub/EventSubInterface.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/EventSub/__init__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/OAuth/Exceptions.py
+-rw-r--r--   0        0        0    39494 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/OAuth/Oauth flow.svg
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/OAuth/Oauth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/OAuth/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/OAuth/test/oauthtest.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/PubSub/PubSubConnector.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/PubSub/PubSubInterface.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/PubSub/Topics.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/PubSub/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/WebsocketClient.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/tests/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/tests/client_run_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/test/__init__.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/test/test1.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.39/PKG-INFO
```

### Comparing `twitch_edog0049a-0.0.38/dddd.cfgd` & `twitch_edog0049a-0.0.39/dddd.cfgd`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/CallbackServer/CallbackServer.py` & `twitch_edog0049a-0.0.39/CallbackServer/CallbackServer.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/Scope.py` & `twitch_edog0049a-0.0.39/src/Twitch/Scope.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/SubscriptionTypes.py` & `twitch_edog0049a-0.0.39/src/Twitch/SubscriptionTypes.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/TwitchAPI.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/TwitchAPI.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/_ApiRequest.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/_ApiRequest.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/api flow.svg` & `twitch_edog0049a-0.0.39/src/Twitch/API/api flow.svg`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Ads.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Ads.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Analytics.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Analytics.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Bits.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Bits.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ChannelPoints.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/ChannelPoints.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Channels.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Channels.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Charity.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Charity.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Chat.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Chat.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Clips.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Clips.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Entitlements.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Entitlements.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/EventSub.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/EventSub.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Extensions.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Extensions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Games.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Games.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/JWTGeneraotr.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/JWTGeneraotr.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Moderation.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Moderation.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Music.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Music.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Polls.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Polls.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Predictions.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Predictions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Raids.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Raids.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ResponseTypes.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/ResponseTypes.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Schedule.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Schedule.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Search.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Search.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Streams.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Streams.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Subscriptions.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Subscriptions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Tags.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Tags.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Teams.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Teams.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Users.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Users.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Utils.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Utils.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Videos.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Videos.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Whispers.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/Whispers.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__init__.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/test/Ads_test.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/test/Ads_test.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/API/test/Bits_Test.py` & `twitch_edog0049a-0.0.39/src/Twitch/API/test/Bits_Test.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/IrcController.py` & `twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/IrcController.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/MessageHandler.py` & `twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/MessageHandler.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TokenBucket.py` & `twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/TokenBucket.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TwitchChatInterface.py` & `twitch_edog0049a-0.0.39/src/Twitch/ChatInterface/TwitchChatInterface.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/EventHandler/EventHandler.py` & `twitch_edog0049a-0.0.39/src/Twitch/EventHandler/EventHandler.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Exceptions.py` & `twitch_edog0049a-0.0.39/src/Twitch/OAuth/Exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth flow.svg` & `twitch_edog0049a-0.0.39/src/Twitch/OAuth/Oauth flow.svg`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth.py` & `twitch_edog0049a-0.0.39/src/Twitch/OAuth/Oauth.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/OAuth/test/oauthtest.py` & `twitch_edog0049a-0.0.39/src/Twitch/OAuth/test/oauthtest.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubConnector.py` & `twitch_edog0049a-0.0.39/src/Twitch/PubSub/PubSubConnector.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/WebsocketClient.py` & `twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/WebsocketClient.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/client_run_test.py` & `twitch_edog0049a-0.0.39/src/Twitch/WebsocketClient/tests/client_run_test.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/test/test1.py` & `twitch_edog0049a-0.0.39/test/test1.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/LICENSE.txt` & `twitch_edog0049a-0.0.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.38/pyproject.toml` & `twitch_edog0049a-0.0.39/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Twitch_Edog0049a"
-version = "0.0.38"
+version = "0.0.39"
 description = 'Twitch library for chat, api, pubs, and eventsub'
 readme = {"file" = "README.md", "content-type" = "text/markdown"}
 requires-python = ">=3.8"
 license = "Apache-2.0 OR MIT"
 authors = [
   { name = "Eli Reid", email = "Elir@elireid.com" },
 ]
```

