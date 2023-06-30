# Comparing `tmp/twitch_edog0049a-0.0.37.tar.gz` & `tmp/twitch_edog0049a-0.0.38.tar.gz`

## Comparing `twitch_edog0049a-0.0.37.tar` & `twitch_edog0049a-0.0.38.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/Twitch.code-workspace
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/dddd.cfgd
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/CallbackServer/CallbackServer.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/CallbackServer/__init__.py
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/Scope.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/SubscriptionTypes.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Exceptions.py
--rw-r--r--   0        0        0    36055 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/TwitchAPI.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/_ApiRequest.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/__init__.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/api flow.svg
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Ads.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Analytics.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Bits.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ChannelPoints.py
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Channels.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Charity.py
--rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Chat.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Clips.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Entitlements.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/EventSub.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Extensions.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Games.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Goals.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/HypeTrain.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Moderation.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Music.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Polls.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Predictions.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Raids.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ResponseTypes.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Schedule.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Search.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Streams.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Subscriptions.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Tags.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Teams.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Users.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Utils.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Videos.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Whispers.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/__imports.py
--rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Ads_test.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Bits_Test.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/Exceptions.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/IrcController.py
--rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/MessageHandler.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TokenBucket.py
--rw-r--r--   0        0        0    22973 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/__init__.py
--rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventHandler/EventHandler.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventHandler/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/EventSubConnector.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/EventSubInterface.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/__init__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Exceptions.py
--rw-r--r--   0        0        0    39494 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth flow.svg
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/test/oauthtest.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/PubSubConnector.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/PubSubInterface.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/Topics.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/__init__.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/WebsocketClient.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/tests/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/tests/client_run_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/test/__init__.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/test/test1.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/LICENSE.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/pyproject.toml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/Twitch.code-workspace
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/dddd.cfgd
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/CallbackServer/CallbackServer.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/CallbackServer/__init__.py
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/Scope.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/SubscriptionTypes.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Exceptions.py
+-rw-r--r--   0        0        0    37750 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/TwitchAPI.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/_ApiRequest.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/__init__.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/api flow.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Ads.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Analytics.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Bits.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ChannelPoints.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Channels.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Charity.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Chat.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Clips.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Entitlements.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/EventSub.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Extensions.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Games.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Goals.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/HypeTrain.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/JWTGeneraotr.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Moderation.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Music.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Polls.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Predictions.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Raids.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ResponseTypes.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Schedule.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Search.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Streams.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Subscriptions.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Tags.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Teams.py
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Users.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Utils.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Videos.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Whispers.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__imports.py
+-rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Ads_test.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Bits_Test.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/Utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/API/test/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/Exceptions.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/IrcController.py
+-rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/MessageHandler.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TokenBucket.py
+-rw-r--r--   0        0        0    22973 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TwitchChatInterface.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/__init__.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventHandler/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/EventSubConnector.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/EventSubInterface.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/EventSub/__init__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Exceptions.py
+-rw-r--r--   0        0        0    39494 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth flow.svg
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/OAuth/test/oauthtest.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubConnector.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubInterface.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/Topics.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/PubSub/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/WebsocketClient.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/client_run_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/test/__init__.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/test/test1.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.38/PKG-INFO
```

### Comparing `twitch_edog0049a-0.0.37/dddd.cfgd` & `twitch_edog0049a-0.0.38/dddd.cfgd`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/CallbackServer/CallbackServer.py` & `twitch_edog0049a-0.0.38/CallbackServer/CallbackServer.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/Scope.py` & `twitch_edog0049a-0.0.38/src/Twitch/Scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 from collections.abc import Iterable
 
 
 class _Analytics:
     class _Read:
         
         @property
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/SubscriptionTypes.py` & `twitch_edog0049a-0.0.38/src/Twitch/SubscriptionTypes.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/TwitchAPI.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/TwitchAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,31 @@
 from Twitch.API.Resources import Utils
 
 class Credentials:
     def __init__(self, id: str, OauthToken: str, scopes: list) -> None:
         self.id = id
         self.Oauth = OauthToken
         self.scopes = scopes
+
 class twitchAPI:
     def __init__(self, clientCreds: Credentials, userCreds:Credentials) -> None:
         self.APIconnector = APIRequest("https://api.twitch.tv/helix")
+        
         self._credentials:dict[Utils.AuthRequired, Credentials] = {
             Utils.AuthRequired.CLIENT: clientCreds,
             Utils.AuthRequired.USER : userCreds,
         }
+
         self._APIReqestFailedExcptions: dict = {
             Utils.HTTPStatus.BAD_REQUEST : TwitchApiBadRequstException,
             Utils.HTTPStatus.UNAUTHORIZED : TwitchApiUnauthorizedException,
             Utils.HTTPStatus.NOT_FOUND : TwitchApiNotFoundException,
-            Utils.HTTPStatus.TOO_MANY_REQUESTS : TwitchApiTooManyRequestsException
+            Utils.HTTPStatus.TOO_MANY_REQUESTS : TwitchApiTooManyRequestsException,
         }
+
         self._ApiRequestSuccess: list= [
             Utils.HTTPStatus.OK,
             Utils.HTTPStatus.ACCEPTED,
             Utils.HTTPStatus.NO_CONTENT,
             Utils.HTTPStatus.CREATED,
         ]
     
@@ -73,15 +77,37 @@
             response.status = APIresponse.status
             for key, value in response.raw.items():
                     response.__setattr__(key, value)
             return
         raise self._APIReqestFailedExcptions[APIresponse.status](await APIresponse.json())
 
     async def StartCommercial(self, length: int) -> StartCommercialRepsonse:
-        request = StartCommercialRequest(self._credentials[Utils.UserType.BROADCASTER].id, length)
+        """
+        StartCommercial Starts a commercial on the specified channel.
+
+            NOTE: Only partners and affiliates may run commercials and they must be streaming live at the time.
+
+            NOTE: Only the broadcaster may start a commercial; the broadcaster’s editors and moderators may not start commercials on behalf of the broadcaster.
+
+            Authorization
+                Requires a user access token that includes the channel:edit:commercial scope.
+
+        :param length: The length of the commercial to run, in seconds. Twitch tries to serve a commercial that’s the requested length, but it may be shorter or longer. The maximum length you should request is 180 seconds.
+        :type length: int
+        :return: 
+        :rtype: StartCommercialRepsonse
+               data:	Object[]	An array that contains a single object with the status of your start commercial request.
+               {
+                        length:	Integer	The length of the commercial you requested. If you request a commercial that’s 
+                                longer than 180 seconds, the API uses 180 seconds.
+                        message:	String	A message that indicates whether Twitch was able to serve an ad.
+                        retry_after:	Integer	The number of seconds you must wait before running another commercial.
+                }
+        """
+        request = StartCommercialRequest(self._credentials[Utils.AuthRequired.USER].id, length)
         response = StartCommercialRepsonse()
         await self._twitchAPICall(request, response)
         return response
 
     async def GetExtensionAnalytics(self,extension_id: Optional[str]= None, 
                 type: Optional[str]= None,
                 started_at: Optional[datetime] = None,
@@ -127,16 +153,22 @@
                                        first: Optional[int]=None, 
                                        after: Optional[str]=None) -> GetExtensionTransactionsResponse:
         request = GetExtensionTransactionsRequest(extension_id, id, first, after)
         response = GetExtensionTransactionsResponse()
         await self._twitchAPICall(request, response)
         return response
 
-    async def GetChannelInformation(self, broadcaster_ids:list, userAuth=False) -> GetChannelInformationResponse:
-        request = GetChannelInformationRequest(broadcaster_ids, userAuth)
+    async def GetChannelInformationAsApp(self, broadcaster_id) -> GetChannelInformationResponse:
+        request = GetChannelInformationRequest(broadcaster_id)
+        response = GetChannelInformationResponse()
+        await self._twitchAPICall(request, response)
+        return response
+    
+    async def GetChannelInformationAsUser(self, broadcaster_id) -> GetChannelInformationResponse:
+        request = GetChannelInformationRequest(broadcaster_id, True)
         response = GetChannelInformationResponse()
         await self._twitchAPICall(request, response)
         return response
 
     async def ModifyChannelInformation(self, title:Optional[str]=None, 
                                        delay:Optional[int]=None, 
                                        tags:Optional[list[str]]=None) -> ModifyChannelInformationResponse:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/_ApiRequest.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/_ApiRequest.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/api flow.svg` & `twitch_edog0049a-0.0.38/src/Twitch/API/api flow.svg`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Ads.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Ads.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Analytics.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Entitlements.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,56 @@
 from Twitch.API.Resources.__imports import *
-"""
-Get Extension Analytics
-"""
 
-class GetExtensionAnalyticsRequest(Utils.RequestBaseClass):
+class GetDropsEntitlementsRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.GET
-    scope = Scope.Analytics.Read.Extensions
-    authorization = Utils.AuthRequired.USER
-    endPoint = "/analytics/extensions"
-
-    def __init__(self, 
-                extension_id: Optional[str]= None, 
-                type: Optional[str]= None,
-                started_at: Optional[datetime] = None,
-                ended_at: Optional[datetime] = None,
-                first: Optional[int] = None,
-                after: Optional[str] = None
-                    ) -> None:
-        
-        self.extension_id = extension_id
-        self.type = type
-        self.started_at = started_at.isoformat("T") if isinstance(started_at, datetime) else started_at
-        self.ended_at = ended_at.isoformat("T") if isinstance(ended_at, datetime) else started_at
+    scope = None
+    authorization = Utils.AuthRequired.CLIENT
+    endPoint ="/entitlements/drops"
+
+    def __init__(self,id: Optional[str]=None, user_id: Optional[str]=None, 
+                game_id: Optional[str]=None, fulfillment_status:Optional[str]=None,
+                after:Optional[str]=None, first:Optional[int]=None, userAuth: bool=False) -> None:
+        if userAuth:
+            self.authorization = Utils.AuthRequired.USER
+        self.id = id
+        self.user_id = user_id
+        self.game_id = game_id
+        self.fulfillment_status = fulfillment_status
+        self.after = after
         self.first = first
-        self.after = after 
         super().__init__()
+      
+class GetDropsEntitlementsItem:
+    id: str
+    benefit_id: str 
+    timestamp: str
+    user_id: str
+    game_id: str
+    fulfillment_status: str 
+    entitlement_id: str
+    last_updated: str
 
-class ExtensionAnalyticsItem(Utils.DateRangeMixin):
-    extension_id:str
-    URL:str
-    type:str
-
-class GetExtensionAnalyticsResponse(Utils.PagenationMixin, Utils.ResponseBaseClass):
+class GetDropsEntitlementsResponse(Utils.pagenation, Utils.ResponseBaseClass):
     def __init__(self) -> None:
-        super().__init__(ExtensionAnalyticsItem)
+        super().__init__(GetDropsEntitlementsItem)
 
-"""
-Get Game Analytics
-"""   
-class GetGameAnalyticsRequest(Utils.RequestBaseClass):
-    requestType = Utils.HTTPMethod.GET
-    scope = Scope.Analytics.Read.Extensions
-    authorization = Utils.AuthRequired.USER
-    endPoint = "/analytics/extensions"
-    game_id: str
-    date_range: Utils.dateRange
 
-    def __init__(self, 
-                 game_id: Optional[str] = None,
-                 type: Optional[str]= None,
-                 started_at: Optional[datetime] = None,
-                 ended_at: Optional[datetime] = None,
-                 first: Optional[int] = None,
-                 after: Optional[str] = None
-                    ) -> None:
-        
-        self.game_id = game_id
-        self.type = type
-        self.started_at = started_at.isoformat("T") if isinstance(started_at, datetime) else started_at
-        self.ended_at = ended_at.isoformat("T") if isinstance(ended_at, datetime) else started_at
-        self.first = first
-        self.after = after 
+class UpdateDropsEntitlementsRequest(Utils.RequestBaseClass):
+    requestType = Utils.HTTPMethod.PATCH
+    scope = None
+    authorization = Utils.AuthRequired.CLIENT
+    endPoint ="/entitlements/drops"
+
+    def __init__(self, entitlement_ids: Optional[list[str]]=None, fulfillment_status:Optional[str]=None, userAuth: bool=False) -> None:
+        if userAuth:
+            self.authorization = Utils.AuthRequired.USER
+        self.entitlement_ids = entitlement_ids
+        self.fulfillment_status = fulfillment_status
         super().__init__()
 
-class GameAnalyticsItem(Utils.DateRangeMixin):
-    def __init__(self) -> None:
-        self.game_id:str
-        self.URL:str
-        self.type:str
-class GetGameAnalyticsResponse(Utils.PagenationMixin, Utils.ResponseBaseClass):
+class UpdateDropsEntitlementsItem:
+     status: str
+     ids: list[str]
+
+class UpdateDropsEntitlementsResponse(Utils.ResponseBaseClass):
     def __init__(self) -> None:
-        super().__init__(GameAnalyticsItem)
+        super().__init__(UpdateDropsEntitlementsItem)
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Bits.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Bits.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 """
 
 class GetCheermotesRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.GET
     scope = None
     authorization = Utils.AuthRequired.CLIENT 
     endPoint = "/bits/cheermotes"
-    def __init__(self,broadcaster_id:Optional[str] = None, userAuth: bool=False) -> None:
+    def __init__(self, broadcaster_id:Optional[str] = None, userAuth: bool=False) -> None:
         if userAuth:
             self.authorization = Utils.AuthRequired.USER
 
         self.broadcaster_id = broadcaster_id
         super().__init__()
 
 class ImageItem:
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ChannelPoints.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ChannelPoints.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Channels.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 """
 
 class GetChannelInformationRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.GET
     scope = None
     authorization = Utils.AuthRequired.CLIENT
     endPoint = "/channels"
-    def __init__(self, broadcaster_ids: list[str], userAuth: bool=False) -> None:
+    def __init__(self, broadcaster_id: str, userAuth: bool=False) -> None:
         if userAuth:
             self.authorization = Utils.AuthRequired.USER
-  
-        self.broadcaster_ids: list[str] = broadcaster_ids
+        self.broadcaster_id = broadcaster_id
         super().__init__()
 
 class ChannelInformationItem:
     broadcaster_id: str
     broadcaster_login: str
     broadcaster_name: str
     broadcaster_language: str
@@ -44,14 +43,15 @@
                  broadcaster_id: str,
                  game_id:Optional[str] =None,
                  broadcaster_language:Optional[str]=None,
                  title:Optional[str]=None,
                  delay:Optional[int]=None,
                  tags:Optional[list[str]]=None
                  ) -> None:
+        
         self.broadcaster_id = broadcaster_id
         self.game_id = game_id
         self.broadcaster_language = broadcaster_language
         self.title = title
         self.delay = delay
         self.tags = tags
         super().__init__()
@@ -88,15 +88,15 @@
 """
 Get Followed Channels - BETA
 """
 class GetFollowedChannelsRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.GET
     scope = Scope.User.Read.Follows
     authorization = Utils.AuthRequired.USER
-    endPoint ="channels/followed"
+    endPoint ="/channels/followed"
     def __init__(self, user_id: str, 
                  broadcaster_id: Optional[str]=None, 
                  first: Optional[int]=None, 
                  after:Optional[str]=None) -> None:
         
         self.user_id: str = user_id
         self.broadcaster_id: str = broadcaster_id
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Charity.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Charity.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Chat.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Chat.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Clips.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Clips.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Entitlements.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Raids.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from Twitch.API.Resources.__imports import *
-class GetDropsEntitlementsRequest(Utils.RequestBaseClass):
+
+class StartaraidRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class GetDropsEntitlementsResponse(Utils.ResponseBaseClass):
+class StartaraidResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class UpdateDropsEntitlementsRequest(Utils.RequestBaseClass):
+class CancelaraidRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class UpdateDropsEntitlementsResponse(Utils.ResponseBaseClass):
+class CancelaraidResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
-            super().__init__()
+            super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/EventSub.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 from Twitch.API.Resources.__imports import *
 
-class CreateEventSubSubscriptionRequest(Utils.RequestBaseClass):
+class GetAllStreamTagsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class CreateEventSubSubscriptionResponse(Utils.ResponseBaseClass):
+class GetAllStreamTagsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class DeleteEventSubSubscriptionRequest(Utils.RequestBaseClass):
+class GetStreamTagsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class DeleteEventSubSubscriptionResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
-
-class GetEventSubSubscriptionsRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
-
-class GetEventSubSubscriptionsResponse(Utils.ResponseBaseClass):
+class GetStreamTagsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Extensions.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Extensions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 from Twitch.API.Resources.__imports import *
 
 class GetExtensionConfigurationSegmentRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
+        requestType = Utils.HTTPMethod.GET
+        scope = None
+        authorization = Utils.AuthRequired.JTW
+        endPoint ="/extensions/configurations"
+        def __init__(self,extension_id: str, segment: str, broadcaster_id: Optional[str]=None) -> None:
+            self.extension_id = extension_id        
+            self.segment = segment
+            self.broadcaster_id = broadcaster_id
+            super().__init__()
+
+class GetExtensionConfigurationSegmentItem:
+    broadcaster_id: str
+    segment: str
+    version: str
+    content: str 
 
 class GetExtensionConfigurationSegmentResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
-            super().__init__()
+            super().__init__(GetExtensionConfigurationSegmentItem)
 
 class SetExtensionConfigurationSegmentRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
+        requestType = Utils.HTTPMethod.PUT
+        scope = None
+        authorization = Utils.AuthRequired.JTW
+        endPoint ="/extensions/configurations"
+        def __init__(self, extension_id: str, segment: str, broadcaster_id: Optional[str]=None, content: Optional[str]=None, version: Optional[str]=None) -> None:
+            self.extension_id = extension_id
+            self.segment = segment
+            self.broadcaster_id = broadcaster_id
+            self.content = content
+            self.version = version
+            super().__init__()
     
 
 class SetExtensionConfigurationSegmentResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
-            super().__init__()
+            super().__init__(None)
 
 class SetExtensionRequiredConfigurationRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Games.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Games.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Moderation.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Moderation.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Music.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Music.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Polls.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Predictions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from Twitch.API.Resources.__imports import *
 
-class GetPollsRequest(Utils.RequestBaseClass):
+class GetPredictionsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class GetPollsResponse(Utils.ResponseBaseClass):
+class GetPredictionsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class CreatePollRequest(Utils.RequestBaseClass):
+class CreatePredictionRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class CreatePollResponse(Utils.ResponseBaseClass):
+class CreatePredictionResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class EndPollRequest(Utils.RequestBaseClass):
+class EndPredictionRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class EndPollResponse(Utils.ResponseBaseClass):
+class EndPredictionResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Predictions.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Streams.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,56 @@
 from Twitch.API.Resources.__imports import *
 
-class GetPredictionsRequest(Utils.RequestBaseClass):
+class GetStreamKeyRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class GetPredictionsResponse(Utils.ResponseBaseClass):
+class GetStreamKeyResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class CreatePredictionRequest(Utils.RequestBaseClass):
+class GetStreamsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class CreatePredictionResponse(Utils.ResponseBaseClass):
+class GetStreamsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class EndPredictionRequest(Utils.RequestBaseClass):
+class GetFollowedStreamsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class EndPredictionResponse(Utils.ResponseBaseClass):
+class GetFollowedStreamsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
-            super().__init__()
+            super().__init__()
+
+class CreateStreamMarkerRequest(Utils.RequestBaseClass):
+        requestType = Utils.HTTPMethod.POST
+        scope = Scope.Channel.Manage.Redemptions
+        authorization = Utils.AuthRequired.USER
+        endPoint ="//channel_points//custom_rewards"
+    
+
+class CreateStreamMarkerResponse(Utils.ResponseBaseClass):
+        def __init__(self) -> None:
+            super().__init__()
+
+class GetStreamMarkersRequest(Utils.RequestBaseClass):
+        requestType = Utils.HTTPMethod.POST
+        scope = Scope.Channel.Manage.Redemptions
+        authorization = Utils.AuthRequired.USER
+        endPoint ="//channel_points//custom_rewards"
+    
+
+class GetStreamMarkersResponse(Utils.ResponseBaseClass):
+        def __init__(self) -> None:
+            super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Raids.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from Twitch.API.Resources.__imports import *
 
-class StartaraidRequest(Utils.RequestBaseClass):
+class SearchCategoriesRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class StartaraidResponse(Utils.ResponseBaseClass):
+class SearchCategoriesResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class CancelaraidRequest(Utils.RequestBaseClass):
+class SearchChannelsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class CancelaraidResponse(Utils.ResponseBaseClass):
+class SearchChannelsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
-            super().__init__()
+            super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ResponseTypes.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/ResponseTypes.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Schedule.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Schedule.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Search.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Teams.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from Twitch.API.Resources.__imports import *
 
-class SearchCategoriesRequest(Utils.RequestBaseClass):
+class GetChannelTeamsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class SearchCategoriesResponse(Utils.ResponseBaseClass):
+class GetChannelTeamsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
 
-class SearchChannelsRequest(Utils.RequestBaseClass):
+class GetTeamsRequest(Utils.RequestBaseClass):
         requestType = Utils.HTTPMethod.POST
         scope = Scope.Channel.Manage.Redemptions
         authorization = Utils.AuthRequired.USER
         endPoint ="//channel_points//custom_rewards"
     
 
-class SearchChannelsResponse(Utils.ResponseBaseClass):
+class GetTeamsResponse(Utils.ResponseBaseClass):
         def __init__(self) -> None:
             super().__init__()
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Streams.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Polls.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,83 @@
-from Twitch.API.Resources.__imports import *
-
-class GetStreamKeyRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
-
-class GetStreamKeyResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
-
-class GetStreamsRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
 
-class GetStreamsResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
-
-class GetFollowedStreamsRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
+from Twitch.API.Resources.__imports import *
 
-class GetFollowedStreamsResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
-
-class CreateStreamMarkerRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
-    
+class GetPollsRequest(Utils.RequestBaseClass):
+    requestType = Utils.HTTPMethod.GET
+    scope = Scope.Channel.Read.Polls
+    authorization = Utils.AuthRequired.USER
+    endPoint = "/polls"
+    def __init__(self, broadcaster_id: str, id: Optional[str] = None, first: Optional[str]=None, after: Optional[str]=None) -> None:
+        super().__init__()
+        self.broadcaster_id = broadcaster_id
+        self.id = id
+        self.first = first
+        self.after = after
+
+class Choices:
+    id: str
+    title: str
+    votes: int
+    channel_points_votes: int
+    bits_votes: int
+
+
+class PollsItem:
+    id: str
+    broadcaster_id: str
+    broadcaster_name: str
+    broadcaster_login: str
+    title: str
+    choices: Choices
+    bits_voting_enabled: bool
+    bit_per_vote: int
+    channel_points_voting_enabled: bool
+    channel_points_per_vote: int
+    status: str
+    duration: int
+    started_at: str
+    ended_at: str
 
-class CreateStreamMarkerResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
-
-class GetStreamMarkersRequest(Utils.RequestBaseClass):
-        requestType = Utils.HTTPMethod.POST
-        scope = Scope.Channel.Manage.Redemptions
-        authorization = Utils.AuthRequired.USER
-        endPoint ="//channel_points//custom_rewards"
     
-
-class GetStreamMarkersResponse(Utils.ResponseBaseClass):
-        def __init__(self) -> None:
-            super().__init__()
+class GetPollsResponse(Utils.PagenationMixin, Utils.ResponseBaseClass):
+    def __init__(self) -> None:
+        super().__init__(PollsItem)
+
+Title: TypeAlias = str
+class CreatePollRequest(Utils.RequestBaseClass):
+    requestType = Utils.HTTPMethod.POST
+    scope = Scope.Channel.Manage.Polls
+    authorization = Utils.AuthRequired.USER
+    endPoint ="/polls"
+
+    def __init__(self, broadcaste_id: str, title: str, 
+                 choices: List[Title], duration: int, 
+                 channel_points_voting_enabled: Optional[bool]=None, 
+                 channel_points_per_vote: Optional[int]=None) -> None:
+        self.broadcaster_id = broadcaste_id
+        self.title = title
+        self.choices = choices
+        self.duration = duration
+        self.channel_points_voting_enabled = channel_points_voting_enabled
+        self.channel_points_per_vote = channel_points_per_vote
+        super().__init__()
+
+class CreatePollResponse(Utils.ResponseBaseClass):
+    def __init__(self) -> None:
+        super().__init__(PollsItem)
+
+class EndPollRequest(Utils.RequestBaseClass):
+    requestType = Utils.HTTPMethod.PATCH
+    scope = Scope.Channel.Manage.Polls
+    authorization = Utils.AuthRequired.USER
+    endPoint ="/polls"
+
+    def __init__(self, broadcaster_id: str, id: str, status: str) -> None:
+        self.broadcaster_id = broadcaster_id
+        self.id = id
+        self.status = status
+        super().__init__()
+
+
+class EndPollResponse(Utils.ResponseBaseClass):
+    def __init__(self) -> None:
+        super().__init__(None)
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Subscriptions.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Subscriptions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Users.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from Twitch.API.Resources.__imports import *
 
 class GetUsersRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.GET
     scope = Scope.User.Read.Email
     authorization = Utils.AuthRequired.CLIENT
     endPoint ="/users"
-    def __init__(self, id:Optional[str|list] = None, login: Optional[str|list]=None) -> None:
+    def __init__(self, id: Optional[str|list] = None, login: Optional[str|list]=None) -> None:
             self.id =   id  
             self.login = login
             super().__init__()
 
 class UserItem:
     id: str 
     login: str 
@@ -29,14 +29,15 @@
 
 class UpdateUserRequest(Utils.RequestBaseClass):
     requestType = Utils.HTTPMethod.PUT
     scope = Scope.User.Read.Email
     authorization = Utils.AuthRequired.USER
     endPoint ="/users"
     def __init__(self, description: str) -> None:
+        self.description = description
         super().__init__()
 
 
 class UpdateUserResponse(Utils.ResponseBaseClass):
     def __init__(self) -> None:
         super().__init__(UserItem)
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Utils.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 from http import HTTPMethod, HTTPStatus
 from Twitch import Scope
 
 class AuthRequired(Enum):
     USER = "user access token"
     CLIENT = "app access token"
+    JTW = "jwt token"
 
 
 @dataclass
 class pagenation:
     cursor: str = field(default="")
 
 @dataclass
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Videos.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Videos.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Whispers.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/Whispers.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/Resources/__init__.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/API/test/Ads_test.py` & `twitch_edog0049a-0.0.38/src/Twitch/API/test/Ads_test.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/IrcController.py` & `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/IrcController.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/MessageHandler.py` & `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/MessageHandler.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TokenBucket.py` & `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TokenBucket.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TwitchChatInterface.py` & `twitch_edog0049a-0.0.38/src/Twitch/ChatInterface/TwitchChatInterface.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/EventHandler/EventHandler.py` & `twitch_edog0049a-0.0.38/src/Twitch/EventHandler/EventHandler.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/OAuth/Exceptions.py` & `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth flow.svg` & `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth flow.svg`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth.py` & `twitch_edog0049a-0.0.38/src/Twitch/OAuth/Oauth.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/OAuth/test/oauthtest.py` & `twitch_edog0049a-0.0.38/src/Twitch/OAuth/test/oauthtest.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/PubSub/PubSubConnector.py` & `twitch_edog0049a-0.0.38/src/Twitch/PubSub/PubSubConnector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from ..WebsocketClient.WebsocketClient import WebsocketClient
 import json
+from Twitch.WebsocketClient.WebsocketClient import WebsocketClient
+from queue import Queue
 
 class TopicTracker:
     pass
 
 class PubSubConnector:
-    def __init__(self,topics:list ) -> None:
-        self.messageQ : list = []
+    def __init__(self, topics: list) -> None:
+        self.messageQ: Queue = Queue()
         self._socketClient = WebsocketClient("wss://pubsub-edge.twitch.tv",
                                             self._messageConsumer, self._messageSender)
         self._socketClient.events.on(self._socketClient.EVENTENUM.CONNECTED)
 
     async def _messageConsumer(self, message):
         messageData = json.loads(message)
 
     async def _messageSender(self):
-        if len(self.messageQ)>0:
-            return self.messageQ.pop()
+        if self.messageQ.not_empty:
+            return self.messageQ.get()
         
     async def connect(self):
         self._socketClient.connect()
     
     def onConnect(self, sender, message):
         pass
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/WebsocketClient.py` & `twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/WebsocketClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import websockets
 from websockets.client import WebSocketClientProtocol
 from Twitch.EventHandler import EventHandler
 from enum import Enum
 class WebsocketClient:
     TIMERDEFAULT =.1
     class EVENTENUM():
-        CONNECTED = "1"
-        DISCONNECTED = "2"
-        RECONNECTED = "3"
-        RECONNECTING = "4"
-        MESSAGE = "5"
+        CONNECTED = 1
+        DISCONNECTED = 2
+        RECONNECTED = 3
+        RECONNECTING = 4
+        MESSAGE = 5
+        MESSAGEFAIL = 6
 
     def __init__(self, url: str, consumer: Awaitable, producer: Awaitable, autoReconnect:bool = True, maxRetries: Optional[int] = -1) -> None:
         self.events: EventHandler = EventHandler
         self._connection: WebSocketClientProtocol = None
         self._consumer: Awaitable = consumer
         self._producer: Awaitable = producer
         self._url:str = url
         self._autoReconnect: bool = autoReconnect
         self._reconnectTimer: float = self.TIMERDEFAULT
         self._retries: int = maxRetries
+        self._messageFailed: bool = False
         self.loop: asyncio.AbstractEventLoop = asyncio.new_event_loop()
 
     def disconnect(self):
         if self.loop.is_running():
             self.loop.stop()
 
     def connect(self):
@@ -47,25 +49,27 @@
             self.events.emit(self,self.EVENTENUM.DISCONNECTED, reason)
             if self._autoReconnect:
                 await self.reconnect()
         except: 
             if self._autoReconnect:
                 await self.reconnect()
 
-    async def reconnect(self):
+    async def reconnect(self) -> bool:
         triesLeft = self._retries
         while self._autoReconnect and triesLeft!=0:
             try: 
                 self.events.emit(self,self.EVENTENUM.RECONNECTING)
                 await asyncio.sleep(self._reconnectTimer)
                 self._reconnectTimer = self._reconnectTimer * 2
                 await self._connect()
+                return True
             except Exception as e:
                 if triesLeft > 0:
                     triesLeft -= 1
+        return False        
             
     def stopReconnect(self): 
         self._autoReconnect = False
     
     def autoReconnect(self):
         self._autoReconnect = True
 
@@ -78,9 +82,17 @@
     async def _producerHandler(self):
         while True:
             message = await self._producer()
             if message is not None:
                 try:
                     await self._connection.send(message)
                 except websockets.ConnectionClosed:
-                    await self.reconnect()
-            await asyncio.sleep(0)
+                    if await self.reconnect():
+                        while not self._connection.open: 
+                            await asyncio.sleep(0)
+                        await self._connection.send(message)
+                    else:
+                        self.events.emit(self, self.EVENTENUM.MESSAGEFAIL, message)
+            await asyncio.sleep(0)
+
+   
+
```

### Comparing `twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/tests/client_run_test.py` & `twitch_edog0049a-0.0.38/src/Twitch/WebsocketClient/tests/client_run_test.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/test/test1.py` & `twitch_edog0049a-0.0.38/test/test1.py`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/LICENSE.txt` & `twitch_edog0049a-0.0.38/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twitch_edog0049a-0.0.37/pyproject.toml` & `twitch_edog0049a-0.0.38/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Twitch_Edog0049a"
-version = "0.0.37"
+version = "0.0.38"
 description = 'Twitch library for chat, api, pubs, and eventsub'
 readme = {"file" = "README.md", "content-type" = "text/markdown"}
 requires-python = ">=3.8"
 license = "Apache-2.0 OR MIT"
 authors = [
   { name = "Eli Reid", email = "Elir@elireid.com" },
 ]
```

