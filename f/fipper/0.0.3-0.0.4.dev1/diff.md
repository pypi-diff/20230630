# Comparing `tmp/fipper-0.0.3.tar.gz` & `tmp/fipper-0.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fipper-0.0.3.tar", last modified: Fri Jun  2 05:49:41 2023, max compression
+gzip compressed data, was "fipper-0.0.4.dev1.tar", last modified: Fri Jun 30 09:23:35 2023, max compression
```

## Comparing `fipper-0.0.3.tar` & `fipper-0.0.4.dev1.tar`

### file list

```diff
@@ -1,486 +1,486 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.434093 fipper-0.0.3/
--rw-rw-rw-   0        0        0    35184 2023-06-02 04:40:39.000000 fipper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      291 2023-06-02 04:40:39.000000 fipper-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      781 2023-06-02 04:40:39.000000 fipper-0.0.3/NOTICE
--rw-rw-rw-   0        0        0     2197 2023-06-02 05:49:41.432094 fipper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2023-06-02 04:40:39.000000 fipper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.265275 fipper-0.0.3/compiler/
--rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.269271 fipper-0.0.3/compiler/api/
--rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/__init__.py
--rw-rw-rw-   0        0        0    23018 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/compiler.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.276266 fipper-0.0.3/compiler/api/source/
--rw-rw-rw-   0        0        0     2273 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/source/auth_key.tl
--rw-rw-rw-   0        0        0   159892 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/source/main_api.tl
--rw-rw-rw-   0        0        0     3501 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/source/sys_msgs.tl
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.281263 fipper-0.0.3/compiler/api/template/
--rw-rw-rw-   0        0        0      772 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/template/combinator.txt
--rw-rw-rw-   0        0        0      652 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/api/template/type.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.288259 fipper-0.0.3/compiler/errors/
--rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/__init__.py
--rw-rw-rw-   0        0        0     5055 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/compiler.py
--rw-rw-rw-   0        0        0     1298 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/sort.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.306247 fipper-0.0.3/compiler/errors/source/
--rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/303_SEE_OTHER.tsv
--rw-rw-rw-   0        0        0    22646 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-rw-rw-   0        0        0      687 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-rw-rw-   0        0        0     2027 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/403_FORBIDDEN.tsv
--rw-rw-rw-   0        0        0     1189 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/420_FLOOD.tsv
--rw-rw-rw-   0        0        0     4263 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-rw-rw-   0        0        0      157 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.310244 fipper-0.0.3/compiler/errors/template/
--rw-rw-rw-   0        0        0      190 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/template/class.txt
--rw-rw-rw-   0        0        0      127 2023-06-02 04:40:39.000000 fipper-0.0.3/compiler/errors/template/sub_class.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.349222 fipper-0.0.3/fipper/
--rw-rw-rw-   0        0        0     1441 2023-06-02 05:49:28.000000 fipper-0.0.3/fipper/__init__.py
--rw-rw-rw-   0        0        0    42052 2023-06-02 05:49:28.000000 fipper-0.0.3/fipper/client.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.393193 fipper-0.0.3/fipper/connection/
--rw-rw-rw-   0        0        0      873 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/__init__.py
--rw-rw-rw-   0        0        0     2916 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/connection.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.394192 fipper-0.0.3/fipper/connection/transport/
--rw-rw-rw-   0        0        0      857 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.411182 fipper-0.0.3/fipper/connection/transport/tcp/
--rw-rw-rw-   0        0        0     1068 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/__init__.py
--rw-rw-rw-   0        0        0     4225 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp.py
--rw-rw-rw-   0        0        0     1825 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp_abridged.py
--rw-rw-rw-   0        0        0     2908 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp_abridged_o.py
--rw-rw-rw-   0        0        0     1970 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp_full.py
--rw-rw-rw-   0        0        0     1556 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp_intermediate.py
--rw-rw-rw-   0        0        0     2530 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/connection/transport/tcp/tcp_intermediate_o.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.424174 fipper-0.0.3/fipper/crypto/
--rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/crypto/__init__.py
--rw-rw-rw-   0        0        0     4143 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/crypto/aes.py
--rw-rw-rw-   0        0        0     4890 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/crypto/mtproto.py
--rw-rw-rw-   0        0        0     2528 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/crypto/prime.py
--rw-rw-rw-   0        0        0    11002 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/crypto/rsa.py
--rw-rw-rw-   0        0        0    10453 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/dispatcher.py
--rw-rw-rw-   0        0        0   212040 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/emoji.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.461667 fipper-0.0.3/fipper/enums/
--rw-rw-rw-   0        0        0     1785 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/auto_name.py
--rw-rw-rw-   0        0        0     2375 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/chat_action.py
--rw-rw-rw-   0        0        0     4328 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/chat_event_action.py
--rw-rw-rw-   0        0        0     1306 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/chat_member_status.py
--rw-rw-rw-   0        0        0     1484 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/chat_members_filter.py
--rw-rw-rw-   0        0        0     1276 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/chat_type.py
--rw-rw-rw-   0        0        0     2544 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/message_entity_type.py
--rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/message_media_type.py
--rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/message_service_type.py
--rw-rw-rw-   0        0        0     2475 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/messages_filter.py
--rw-rw-rw-   0        0        0     1456 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/next_code_type.py
--rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/parse_mode.py
--rw-rw-rw-   0        0        0     1076 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/poll_type.py
--rw-rw-rw-   0        0        0     1567 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/sent_code_type.py
--rw-rw-rw-   0        0        0     1340 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/enums/user_status.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.468662 fipper-0.0.3/fipper/errors/
--rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/errors/__init__.py
--rw-rw-rw-   0        0        0     3410 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/errors/rpc_error.py
--rw-rw-rw-   0        0        0    15633 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/file_id.py
--rw-rw-rw-   0        0        0    25461 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.508636 fipper-0.0.3/fipper/handlers/
--rw-rw-rw-   0        0        0     1560 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0     2052 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/chat_join_request_handler.py
--rw-rw-rw-   0        0        0     2087 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/chat_member_updated_handler.py
--rw-rw-rw-   0        0        0     2143 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/chosen_inline_result_handler.py
--rw-rw-rw-   0        0        0     2502 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/conversation_handler.py
--rw-rw-rw-   0        0        0     2588 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/deleted_messages_handler.py
--rw-rw-rw-   0        0        0     1739 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/disconnect_handler.py
--rw-rw-rw-   0        0        0     2020 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/edited_message_handler.py
--rw-rw-rw-   0        0        0     1585 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/handler.py
--rw-rw-rw-   0        0        0     2025 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0     2902 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/message_handler.py
--rw-rw-rw-   0        0        0     1956 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/poll_handler.py
--rw-rw-rw-   0        0        0     2987 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/raw_update_handler.py
--rw-rw-rw-   0        0        0     2028 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/handlers/user_status_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.512635 fipper-0.0.3/fipper/methods/
--rw-rw-rw-   0        0        0     1365 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.521628 fipper-0.0.3/fipper/methods/advanced/
--rw-rw-rw-   0        0        0     1017 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     3206 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/advanced/invoke.py
--rw-rw-rw-   0        0        0     4673 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/advanced/resolve_peer.py
--rw-rw-rw-   0        0        0     8382 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/advanced/save_file.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.579103 fipper-0.0.3/fipper/methods/auth/
--rw-rw-rw-   0        0        0     1708 2023-06-02 05:49:28.000000 fipper-0.0.3/fipper/methods/auth/__init__.py
--rw-rw-rw-   0        0        0     1506 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/accept_terms_of_service.py
--rw-rw-rw-   0        0        0     1990 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/check_password.py
--rw-rw-rw-   0        0        0     1794 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/connect.py
--rw-rw-rw-   0        0        0     1540 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/disconnect.py
--rw-rw-rw-   0        0        0     1339 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/get_password_hint.py
--rw-rw-rw-   0        0        0     1709 2023-06-02 05:49:28.000000 fipper-0.0.3/fipper/methods/auth/initialize.py
--rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/log_out.py
--rw-rw-rw-   0        0        0     1878 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/recover_password.py
--rw-rw-rw-   0        0        0     2202 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/resend_code.py
--rw-rw-rw-   0        0        0     2851 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/send_code.py
--rw-rw-rw-   0        0        0     1510 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/send_recovery_code.py
--rw-rw-rw-   0        0        0     3149 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/sign_in.py
--rw-rw-rw-   0        0        0     2788 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/sign_in_bot.py
--rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/sign_up.py
--rw-rw-rw-   0        0        0     1905 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/auth/terminate.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.621594 fipper-0.0.3/fipper/methods/bots/
--rw-rw-rw-   0        0        0     2096 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/__init__.py
--rw-rw-rw-   0        0        0     3386 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/answer_callback_query.py
--rw-rw-rw-   0        0        0     5090 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/answer_inline_query.py
--rw-rw-rw-   0        0        0     2030 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/answer_web_app_query.py
--rw-rw-rw-   0        0        0     2412 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/delete_bot_commands.py
--rw-rw-rw-   0        0        0     2628 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/get_bot_commands.py
--rw-rw-rw-   0        0        0     2102 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/get_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2377 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/get_chat_menu_button.py
--rw-rw-rw-   0        0        0     2860 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/get_game_high_scores.py
--rw-rw-rw-   0        0        0     3445 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/get_inline_bot_results.py
--rw-rw-rw-   0        0        0     2918 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/request_callback_answer.py
--rw-rw-rw-   0        0        0     4044 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/send_game.py
--rw-rw-rw-   0        0        0     3056 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/send_inline_bot_result.py
--rw-rw-rw-   0        0        0     2767 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/set_bot_commands.py
--rw-rw-rw-   0        0        0     3255 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/set_bot_default_privileges.py
--rw-rw-rw-   0        0        0     2092 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/set_chat_menu_button.py
--rw-rw-rw-   0        0        0     4036 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/bots/set_game_score.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.738523 fipper-0.0.3/fipper/methods/chats/
--rw-rw-rw-   0        0        0     3540 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/__init__.py
--rw-rw-rw-   0        0        0     3448 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/add_chat_members.py
--rw-rw-rw-   0        0        0     2281 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/archive_chats.py
--rw-rw-rw-   0        0        0     4721 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/ban_chat_member.py
--rw-rw-rw-   0        0        0     1863 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/create_channel.py
--rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/create_group.py
--rw-rw-rw-   0        0        0     2003 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/create_supergroup.py
--rw-rw-rw-   0        0        0     1631 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/delete_channel.py
--rw-rw-rw-   0        0        0     2371 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/delete_chat_photo.py
--rw-rw-rw-   0        0        0     1649 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/delete_supergroup.py
--rw-rw-rw-   0        0        0     2018 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/delete_user_history.py
--rw-rw-rw-   0        0        0     3355 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat.py
--rw-rw-rw-   0        0        0     4129 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat_event_log.py
--rw-rw-rw-   0        0        0     3418 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat_member.py
--rw-rw-rw-   0        0        0     5420 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat_members.py
--rw-rw-rw-   0        0        0     2327 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat_members_count.py
--rw-rw-rw-   0        0        0     1768 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_chat_online_count.py
--rw-rw-rw-   0        0        0     3456 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_dialogs.py
--rw-rw-rw-   0        0        0     2153 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_dialogs_count.py
--rw-rw-rw-   0        0        0     2467 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_nearby_chats.py
--rw-rw-rw-   0        0        0     2191 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/get_send_as_chats.py
--rw-rw-rw-   0        0        0     2758 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/join_chat.py
--rw-rw-rw-   0        0        0     2676 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/leave_chat.py
--rw-rw-rw-   0        0        0     1569 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/mark_chat_unread.py
--rw-rw-rw-   0        0        0     3230 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/pin_chat_message.py
--rw-rw-rw-   0        0        0     3954 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/promote_chat_member.py
--rw-rw-rw-   0        0        0     4397 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/restrict_chat_member.py
--rw-rw-rw-   0        0        0     3215 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_administrator_title.py
--rw-rw-rw-   0        0        0     2307 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_description.py
--rw-rw-rw-   0        0        0     3488 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_permissions.py
--rw-rw-rw-   0        0        0     4708 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_photo.py
--rw-rw-rw-   0        0        0     1774 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_protected_content.py
--rw-rw-rw-   0        0        0     2644 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_title.py
--rw-rw-rw-   0        0        0     2356 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_chat_username.py
--rw-rw-rw-   0        0        0     2031 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_send_as_chat.py
--rw-rw-rw-   0        0        0     2140 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/set_slow_mode.py
--rw-rw-rw-   0        0        0     2295 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/unarchive_chats.py
--rw-rw-rw-   0        0        0     2363 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/unban_chat_member.py
--rw-rw-rw-   0        0        0     1989 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/unpin_all_chat_messages.py
--rw-rw-rw-   0        0        0     2194 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/chats/unpin_chat_message.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.757511 fipper-0.0.3/fipper/methods/contacts/
--rw-rw-rw-   0        0        0     1187 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/__init__.py
--rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/add_contact.py
--rw-rw-rw-   0        0        0     2504 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/delete_contacts.py
--rw-rw-rw-   0        0        0     1642 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/get_contacts.py
--rw-rw-rw-   0        0        0     1457 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/get_contacts_count.py
--rw-rw-rw-   0        0        0     1980 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/contacts/import_contacts.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.796486 fipper-0.0.3/fipper/methods/decorators/
--rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0     2213 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_chat_join_request.py
--rw-rw-rw-   0        0        0     2234 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_chat_member_updated.py
--rw-rw-rw-   0        0        0     2262 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_chosen_inline_result.py
--rw-rw-rw-   0        0        0     2228 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_deleted_messages.py
--rw-rw-rw-   0        0        0     1584 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_disconnect.py
--rw-rw-rw-   0        0        0     2217 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_edited_message.py
--rw-rw-rw-   0        0        0     2212 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0     2183 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_message.py
--rw-rw-rw-   0        0        0     2165 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_poll.py
--rw-rw-rw-   0        0        0     1861 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_raw_update.py
--rw-rw-rw-   0        0        0     2197 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/decorators/on_user_status.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.839460 fipper-0.0.3/fipper/methods/invite_links/
--rw-rw-rw-   0        0        0     2493 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/approve_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1975 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/approve_chat_join_request.py
--rw-rw-rw-   0        0        0     3444 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/create_chat_invite_link.py
--rw-rw-rw-   0        0        0     1944 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/decline_all_chat_join_requests.py
--rw-rw-rw-   0        0        0     1976 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/decline_chat_join_request.py
--rw-rw-rw-   0        0        0     2079 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/delete_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     1797 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/delete_chat_invite_link.py
--rw-rw-rw-   0        0        0     3615 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/edit_chat_invite_link.py
--rw-rw-rw-   0        0        0     2637 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/export_chat_invite_link.py
--rw-rw-rw-   0        0        0     3654 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_admin_invite_links.py
--rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-rw-rw-   0        0        0     2045 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link.py
--rw-rw-rw-   0        0        0     3003 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link_joiners.py
--rw-rw-rw-   0        0        0     1979 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-rw-rw-   0        0        0     3023 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/get_chat_join_requests.py
--rw-rw-rw-   0        0        0     2387 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/invite_links/revoke_chat_invite_link.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.991366 fipper-0.0.3/fipper/methods/messages/
--rw-rw-rw-   0        0        0     4194 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/__init__.py
--rw-rw-rw-   0        0        0     6095 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/copy_media_group.py
--rw-rw-rw-   0        0        0     5280 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/copy_message.py
--rw-rw-rw-   0        0        0     3226 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/delete_messages.py
--rw-rw-rw-   0        0        0     7705 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/download_media.py
--rw-rw-rw-   0        0        0     2326 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_inline_caption.py
--rw-rw-rw-   0        0        0     9990 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_inline_media.py
--rw-rw-rw-   0        0        0     2519 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_inline_reply_markup.py
--rw-rw-rw-   0        0        0     3189 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_inline_text.py
--rw-rw-rw-   0        0        0     3040 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_message_caption.py
--rw-rw-rw-   0        0        0    12725 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_message_media.py
--rw-rw-rw-   0        0        0     3039 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_message_reply_markup.py
--rw-rw-rw-   0        0        0     3986 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/edit_message_text.py
--rw-rw-rw-   0        0        0     4662 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/forward_messages.py
--rw-rw-rw-   0        0        0     4152 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_chat_history.py
--rw-rw-rw-   0        0        0     2455 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_chat_history_count.py
--rw-rw-rw-   0        0        0     2023 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_custom_emoji_stickers.py
--rw-rw-rw-   0        0        0     2286 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_discussion_message.py
--rw-rw-rw-   0        0        0     2888 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_discussion_replies.py
--rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_discussion_replies_count.py
--rw-rw-rw-   0        0        0     3011 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_media_group.py
--rw-rw-rw-   0        0        0     4846 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/get_messages.py
--rw-rw-rw-   0        0        0     2227 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/inline_session.py
--rw-rw-rw-   0        0        0     2594 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/read_chat_history.py
--rw-rw-rw-   0        0        0     2175 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/retract_vote.py
--rw-rw-rw-   0        0        0     4259 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/search_global.py
--rw-rw-rw-   0        0        0     2208 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/search_global_count.py
--rw-rw-rw-   0        0        0     5486 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/search_messages.py
--rw-rw-rw-   0        0        0     3277 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/search_messages_count.py
--rw-rw-rw-   0        0        0    12513 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_animation.py
--rw-rw-rw-   0        0        0    11326 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_audio.py
--rw-rw-rw-   0        0        0     5579 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_cached_media.py
--rw-rw-rw-   0        0        0     2887 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_chat_action.py
--rw-rw-rw-   0        0        0     4970 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_contact.py
--rw-rw-rw-   0        0        0     4939 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_dice.py
--rw-rw-rw-   0        0        0    10656 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_document.py
--rw-rw-rw-   0        0        0     4671 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_location.py
--rw-rw-rw-   0        0        0    19643 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_media_group.py
--rw-rw-rw-   0        0        0     7418 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_message.py
--rw-rw-rw-   0        0        0     9303 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_photo.py
--rw-rw-rw-   0        0        0     8222 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_poll.py
--rw-rw-rw-   0        0        0     2428 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_reaction.py
--rw-rw-rw-   0        0        0     8489 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_sticker.py
--rw-rw-rw-   0        0        0     5516 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_venue.py
--rw-rw-rw-   0        0        0    11877 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_video.py
--rw-rw-rw-   0        0        0     9487 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_video_note.py
--rw-rw-rw-   0        0        0     9600 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/send_voice.py
--rw-rw-rw-   0        0        0     2884 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/stop_poll.py
--rw-rw-rw-   0        0        0     4033 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/stream_media.py
--rw-rw-rw-   0        0        0     2563 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/vote_poll.py
--rw-rw-rw-   0        0        0     2895 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/wait_for_callback_query.py
--rw-rw-rw-   0        0        0     2816 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/messages/wait_for_message.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.006358 fipper-0.0.3/fipper/methods/password/
--rw-rw-rw-   0        0        0     1117 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/password/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/password/change_cloud_password.py
--rw-rw-rw-   0        0        0     3086 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/password/enable_cloud_password.py
--rw-rw-rw-   0        0        0     2199 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/password/remove_cloud_password.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.042335 fipper-0.0.3/fipper/methods/users/
--rw-rw-rw-   0        0        0     1708 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/__init__.py
--rw-rw-rw-   0        0        0     1819 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/block_user.py
--rw-rw-rw-   0        0        0     2288 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/delete_profile_photos.py
--rw-rw-rw-   0        0        0     4548 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_chat_photos.py
--rw-rw-rw-   0        0        0     2577 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_chat_photos_count.py
--rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_common_chats.py
--rw-rw-rw-   0        0        0     1701 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_default_emoji_statuses.py
--rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_me.py
--rw-rw-rw-   0        0        0     2621 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/get_users.py
--rw-rw-rw-   0        0        0     1930 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/set_emoji_status.py
--rw-rw-rw-   0        0        0     2787 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/set_profile_photo.py
--rw-rw-rw-   0        0        0     1925 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/set_username.py
--rw-rw-rw-   0        0        0     1829 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/unblock_user.py
--rw-rw-rw-   0        0        0     2442 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/users/update_profile.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.067319 fipper-0.0.3/fipper/methods/utilities/
--rw-rw-rw-   0        0        0     1292 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/add_handler.py
--rw-rw-rw-   0        0        0     2300 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/compose.py
--rw-rw-rw-   0        0        0     1593 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/export_session_string.py
--rw-rw-rw-   0        0        0     2833 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/idle.py
--rw-rw-rw-   0        0        0     2259 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/remove_handler.py
--rw-rw-rw-   0        0        0     2354 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/restart.py
--rw-rw-rw-   0        0        0     2925 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/run.py
--rw-rw-rw-   0        0        0     2432 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/start.py
--rw-rw-rw-   0        0        0     2178 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/stop.py
--rw-rw-rw-   0        0        0     1749 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/methods/utilities/stop_transmission.py
--rw-rw-rw-   0        0        0    63796 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/mime_types.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.080312 fipper-0.0.3/fipper/parser/
--rw-rw-rw-   0        0        0      865 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/parser/__init__.py
--rw-rw-rw-   0        0        0     7587 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/parser/html.py
--rw-rw-rw-   0        0        0     5937 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/parser/markdown.py
--rw-rw-rw-   0        0        0     2132 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/parser/parser.py
--rw-rw-rw-   0        0        0     1586 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/parser/utils.py
--rw-rw-rw-   0        0        0        0 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.082311 fipper-0.0.3/fipper/raw/
--rw-rw-rw-   0        0        0     1066 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.104297 fipper-0.0.3/fipper/raw/core/
--rw-rw-rw-   0        0        0     1343 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/__init__.py
--rw-rw-rw-   0        0        0     1745 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/future_salt.py
--rw-rw-rw-   0        0        0     1954 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/future_salts.py
--rw-rw-rw-   0        0        0     1876 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/gzip_packed.py
--rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/list.py
--rw-rw-rw-   0        0        0     1907 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/message.py
--rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/msg_container.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.121286 fipper-0.0.3/fipper/raw/core/primitives/
--rw-rw-rw-   0        0        0     1036 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/bool.py
--rw-rw-rw-   0        0        0     1814 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/bytes.py
--rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/double.py
--rw-rw-rw-   0        0        0     1403 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/int.py
--rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/string.py
--rw-rw-rw-   0        0        0     2081 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/primitives/vector.py
--rw-rw-rw-   0        0        0     2575 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/raw/core/tl_object.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.129281 fipper-0.0.3/fipper/session/
--rw-rw-rw-   0        0        0      891 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/__init__.py
--rw-rw-rw-   0        0        0    10760 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/auth.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.142273 fipper-0.0.3/fipper/session/internals/
--rw-rw-rw-   0        0        0      938 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/internals/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/internals/data_center.py
--rw-rw-rw-   0        0        0     1406 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/internals/msg_factory.py
--rw-rw-rw-   0        0        0     1632 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/internals/msg_id.py
--rw-rw-rw-   0        0        0     1291 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/internals/seq_no.py
--rw-rw-rw-   0        0        0    12801 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/session/session.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.153267 fipper-0.0.3/fipper/storage/
--rw-rw-rw-   0        0        0      949 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/storage/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/storage/file_storage.py
--rw-rw-rw-   0        0        0     2823 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/storage/memory_storage.py
--rw-rw-rw-   0        0        0     6638 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/storage/sqlite_storage.py
--rw-rw-rw-   0        0        0     2872 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/storage/storage.py
--rw-rw-rw-   0        0        0     3846 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/sync.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.162261 fipper-0.0.3/fipper/types/
--rw-rw-rw-   0        0        0     1137 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.168258 fipper-0.0.3/fipper/types/authorization/
--rw-rw-rw-   0        0        0      960 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/authorization/__init__.py
--rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/authorization/sent_code.py
--rw-rw-rw-   0        0        0     1978 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/authorization/terms_of_service.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.229219 fipper-0.0.3/fipper/types/bots_and_keyboards/
--rw-rw-rw-   0        0        0     2901 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command.py
--rw-rw-rw-   0        0        0     2841 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope.py
--rw-rw-rw-   0        0        0     1319 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-rw-rw-   0        0        0     1284 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-rw-rw-   0        0        0     1275 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-rw-rw-   0        0        0     1599 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-rw-rw-   0        0        0     1676 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-rw-rw-   0        0        0     1859 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-rw-rw-   0        0        0     1335 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_default.py
--rw-rw-rw-   0        0        0     1058 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/callback_game.py
--rw-rw-rw-   0        0        0    13062 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/callback_query.py
--rw-rw-rw-   0        0        0     2443 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/force_reply.py
--rw-rw-rw-   0        0        0     2276 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/game_high_score.py
--rw-rw-rw-   0        0        0     8312 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/inline_keyboard_button.py
--rw-rw-rw-   0        0        0     2526 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-rw-rw-   0        0        0     3605 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/keyboard_button.py
--rw-rw-rw-   0        0        0     3800 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/login_url.py
--rw-rw-rw-   0        0        0     1633 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button.py
--rw-rw-rw-   0        0        0     1235 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_commands.py
--rw-rw-rw-   0        0        0     1238 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_default.py
--rw-rw-rw-   0        0        0     1850 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_web_app.py
--rw-rw-rw-   0        0        0     4221 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/sent_web_app_message.py
--rw-rw-rw-   0        0        0     1350 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/bots_and_keyboards/web_app_info.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.279188 fipper-0.0.3/fipper/types/inline_mode/
--rw-rw-rw-   0        0        0     2802 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/chosen_inline_result.py
--rw-rw-rw-   0        0        0     7459 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query.py
--rw-rw-rw-   0        0        0     2434 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result.py
--rw-rw-rw-   0        0        0     5917 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_animation.py
--rw-rw-rw-   0        0        0     3391 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_article.py
--rw-rw-rw-   0        0        0     4611 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_audio.py
--rw-rw-rw-   0        0        0     4339 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_animation.py
--rw-rw-rw-   0        0        0     4116 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_audio.py
--rw-rw-rw-   0        0        0     4487 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_document.py
--rw-rw-rw-   0        0        0     4409 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_photo.py
--rw-rw-rw-   0        0        0     3099 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_sticker.py
--rw-rw-rw-   0        0        0     4494 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_video.py
--rw-rw-rw-   0        0        0     4296 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_voice.py
--rw-rw-rw-   0        0        0     4236 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_contact.py
--rw-rw-rw-   0        0        0     5371 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_document.py
--rw-rw-rw-   0        0        0     4731 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_location.py
--rw-rw-rw-   0        0        0     5394 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     4875 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_venue.py
--rw-rw-rw-   0        0        0     5611 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_video.py
--rw-rw-rw-   0        0        0     4460 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/inline_mode/inline_query_result_voice.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.297177 fipper-0.0.3/fipper/types/input_media/
--rw-rw-rw-   0        0        0     1344 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/__init__.py
--rw-rw-rw-   0        0        0     1677 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media.py
--rw-rw-rw-   0        0        0     3305 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media_animation.py
--rw-rw-rw-   0        0        0     3358 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media_audio.py
--rw-rw-rw-   0        0        0     2832 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media_document.py
--rw-rw-rw-   0        0        0     2536 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media_photo.py
--rw-rw-rw-   0        0        0     3500 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_media_video.py
--rw-rw-rw-   0        0        0     1782 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_media/input_phone_contact.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.306172 fipper-0.0.3/fipper/types/input_message_content/
--rw-rw-rw-   0        0        0     1030 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_message_content/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_message_content/input_message_content.py
--rw-rw-rw-   0        0        0     2696 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/input_message_content/input_text_message_content.py
--rw-rw-rw-   0        0        0     1121 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/list.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.361140 fipper-0.0.3/fipper/types/messages_and_media/
--rw-rw-rw-   0        0        0     1883 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/__init__.py
--rw-rw-rw-   0        0        0     4153 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/animation.py
--rw-rw-rw-   0        0        0     4178 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/audio.py
--rw-rw-rw-   0        0        0     2270 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/contact.py
--rw-rw-rw-   0        0        0     1628 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/dice.py
--rw-rw-rw-   0        0        0     3495 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/document.py
--rw-rw-rw-   0        0        0     3131 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/game.py
--rw-rw-rw-   0        0        0     1709 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/location.py
--rw-rw-rw-   0        0        0   150486 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/message.py
--rw-rw-rw-   0        0        0     4456 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/message_entity.py
--rw-rw-rw-   0        0        0     1846 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/message_reactions.py
--rw-rw-rw-   0        0        0     4427 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/photo.py
--rw-rw-rw-   0        0        0     7226 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/poll.py
--rw-rw-rw-   0        0        0     1578 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/poll_option.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/reaction.py
--rw-rw-rw-   0        0        0     7101 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/sticker.py
--rw-rw-rw-   0        0        0     1472 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/stripped_thumbnail.py
--rw-rw-rw-   0        0        0     3858 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/thumbnail.py
--rw-rw-rw-   0        0        0     2355 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/venue.py
--rw-rw-rw-   0        0        0     4511 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/video.py
--rw-rw-rw-   0        0        0     3697 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/video_note.py
--rw-rw-rw-   0        0        0     3292 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/voice.py
--rw-rw-rw-   0        0        0     1614 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/web_app_data.py
--rw-rw-rw-   0        0        0     6520 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/messages_and_media/web_page.py
--rw-rw-rw-   0        0        0     3973 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/object.py
--rw-rw-rw-   0        0        0     1023 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/update.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.418104 fipper-0.0.3/fipper/types/user_and_chats/
--rw-rw-rw-   0        0        0     2364 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/__init__.py
--rw-rw-rw-   0        0        0    33702 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat.py
--rw-rw-rw-   0        0        0     2289 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_admin_with_invite_links.py
--rw-rw-rw-   0        0        0    20240 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_event.py
--rw-rw-rw-   0        0        0     5687 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_event_filter.py
--rw-rw-rw-   0        0        0     4699 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_invite_link.py
--rw-rw-rw-   0        0        0     4364 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_join_request.py
--rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_joiner.py
--rw-rw-rw-   0        0        0     9647 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_member.py
--rw-rw-rw-   0        0        0     3756 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_member_updated.py
--rw-rw-rw-   0        0        0     4478 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_permissions.py
--rw-rw-rw-   0        0        0     4066 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_photo.py
--rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_preview.py
--rw-rw-rw-   0        0        0     5061 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_privileges.py
--rw-rw-rw-   0        0        0     2417 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/chat_reactions.py
--rw-rw-rw-   0        0        0     2749 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/dialog.py
--rw-rw-rw-   0        0        0     2491 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/emoji_status.py
--rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/invite_link_importer.py
--rw-rw-rw-   0        0        0     1711 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/restriction.py
--rw-rw-rw-   0        0        0    13477 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/user.py
--rw-rw-rw-   0        0        0     1385 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/video_chat_ended.py
--rw-rw-rw-   0        0        0     1656 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/video_chat_members_invited.py
--rw-rw-rw-   0        0        0     1572 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/video_chat_scheduled.py
--rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/types/user_and_chats/video_chat_started.py
--rw-rw-rw-   0        0        0    10933 2023-06-02 04:40:39.000000 fipper-0.0.3/fipper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:40.388198 fipper-0.0.3/fipper.egg-info/
--rw-rw-rw-   0        0        0     2197 2023-06-02 05:49:39.000000 fipper-0.0.3/fipper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17932 2023-06-02 05:49:40.000000 fipper-0.0.3/fipper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:49:39.000000 fipper-0.0.3/fipper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 05:49:39.000000 fipper-0.0.3/fipper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       54 2023-06-02 05:49:39.000000 fipper-0.0.3/fipper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 05:49:39.000000 fipper-0.0.3/fipper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       57 2023-06-02 04:40:39.000000 fipper-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 05:49:41.434093 fipper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2106 2023-06-02 04:40:39.000000 fipper-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.422100 fipper-0.0.3/tests/
--rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:49:41.428097 fipper-0.0.3/tests/filters/
--rw-rw-rw-   0        0        0     1237 2023-06-02 04:40:39.000000 fipper-0.0.3/tests/filters/__init__.py
--rw-rw-rw-   0        0        0     3518 2023-06-02 04:40:39.000000 fipper-0.0.3/tests/filters/test_command.py
--rw-rw-rw-   0        0        0     8400 2023-06-02 04:40:39.000000 fipper-0.0.3/tests/test_file_id.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.545199 fipper-0.0.4.dev1/
+-rw-rw-rw-   0        0        0    35184 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/LICENSE
+-rw-rw-rw-   0        0        0      291 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0      781 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/NOTICE
+-rw-rw-rw-   0        0        0     2202 2023-06-30 09:23:35.544198 fipper-0.0.4.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.462837 fipper-0.0.4.dev1/compiler/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.466834 fipper-0.0.4.dev1/compiler/api/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/__init__.py
+-rw-rw-rw-   0        0        0    23018 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/compiler.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.474830 fipper-0.0.4.dev1/compiler/api/source/
+-rw-rw-rw-   0        0        0     2273 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/source/auth_key.tl
+-rw-rw-rw-   0        0        0   159892 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/source/main_api.tl
+-rw-rw-rw-   0        0        0     3501 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/source/sys_msgs.tl
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.478827 fipper-0.0.4.dev1/compiler/api/template/
+-rw-rw-rw-   0        0        0      772 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/template/combinator.txt
+-rw-rw-rw-   0        0        0      652 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/api/template/type.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.485823 fipper-0.0.4.dev1/compiler/errors/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/__init__.py
+-rw-rw-rw-   0        0        0     5055 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/compiler.py
+-rw-rw-rw-   0        0        0     1298 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.502813 fipper-0.0.4.dev1/compiler/errors/source/
+-rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-rw-rw-   0        0        0    22646 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-rw-rw-   0        0        0      687 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-rw-rw-   0        0        0     2027 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-rw-rw-   0        0        0     1189 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-rw-rw-   0        0        0      475 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/420_FLOOD.tsv
+-rw-rw-rw-   0        0        0     4263 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-rw-rw-   0        0        0      157 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.507810 fipper-0.0.4.dev1/compiler/errors/template/
+-rw-rw-rw-   0        0        0      190 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/template/class.txt
+-rw-rw-rw-   0        0        0      127 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/compiler/errors/template/sub_class.txt
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.528797 fipper-0.0.4.dev1/fipper/
+-rw-rw-rw-   0        0        0     1447 2023-06-30 09:23:01.000000 fipper-0.0.4.dev1/fipper/__init__.py
+-rw-rw-rw-   0        0        0    42668 2023-06-30 09:17:30.000000 fipper-0.0.4.dev1/fipper/client.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.574768 fipper-0.0.4.dev1/fipper/connection/
+-rw-rw-rw-   0        0        0      873 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/__init__.py
+-rw-rw-rw-   0        0        0     2916 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/connection.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.576767 fipper-0.0.4.dev1/fipper/connection/transport/
+-rw-rw-rw-   0        0        0      857 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.592757 fipper-0.0.4.dev1/fipper/connection/transport/tcp/
+-rw-rw-rw-   0        0        0     1068 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/__init__.py
+-rw-rw-rw-   0        0        0     4225 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp.py
+-rw-rw-rw-   0        0        0     1825 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_abridged.py
+-rw-rw-rw-   0        0        0     2908 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_abridged_o.py
+-rw-rw-rw-   0        0        0     1970 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_full.py
+-rw-rw-rw-   0        0        0     1556 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_intermediate.py
+-rw-rw-rw-   0        0        0     2530 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_intermediate_o.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.603750 fipper-0.0.4.dev1/fipper/crypto/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4143 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/crypto/aes.py
+-rw-rw-rw-   0        0        0     4890 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/crypto/mtproto.py
+-rw-rw-rw-   0        0        0     2528 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/crypto/prime.py
+-rw-rw-rw-   0        0        0    11002 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/crypto/rsa.py
+-rw-rw-rw-   0        0        0    10453 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/dispatcher.py
+-rw-rw-rw-   0        0        0   212040 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/emoji.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.639729 fipper-0.0.4.dev1/fipper/enums/
+-rw-rw-rw-   0        0        0     1785 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/auto_name.py
+-rw-rw-rw-   0        0        0     2375 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/chat_action.py
+-rw-rw-rw-   0        0        0     4328 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/chat_event_action.py
+-rw-rw-rw-   0        0        0     1306 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/chat_member_status.py
+-rw-rw-rw-   0        0        0     1484 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/chat_members_filter.py
+-rw-rw-rw-   0        0        0     1276 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/chat_type.py
+-rw-rw-rw-   0        0        0     2544 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/message_entity_type.py
+-rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/message_media_type.py
+-rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/message_service_type.py
+-rw-rw-rw-   0        0        0     2475 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/messages_filter.py
+-rw-rw-rw-   0        0        0     1456 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/next_code_type.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/parse_mode.py
+-rw-rw-rw-   0        0        0     1076 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/poll_type.py
+-rw-rw-rw-   0        0        0     1567 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/sent_code_type.py
+-rw-rw-rw-   0        0        0     1340 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/enums/user_status.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.645725 fipper-0.0.4.dev1/fipper/errors/
+-rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/errors/__init__.py
+-rw-rw-rw-   0        0        0     3410 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/errors/rpc_error.py
+-rw-rw-rw-   0        0        0    15633 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/file_id.py
+-rw-rw-rw-   0        0        0    25461 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.678705 fipper-0.0.4.dev1/fipper/handlers/
+-rw-rw-rw-   0        0        0     1560 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0     2052 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/chat_join_request_handler.py
+-rw-rw-rw-   0        0        0     2087 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/chat_member_updated_handler.py
+-rw-rw-rw-   0        0        0     2143 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/chosen_inline_result_handler.py
+-rw-rw-rw-   0        0        0     2502 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/conversation_handler.py
+-rw-rw-rw-   0        0        0     2588 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/deleted_messages_handler.py
+-rw-rw-rw-   0        0        0     1739 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/disconnect_handler.py
+-rw-rw-rw-   0        0        0     2020 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/edited_message_handler.py
+-rw-rw-rw-   0        0        0     1585 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/handler.py
+-rw-rw-rw-   0        0        0     2025 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0     2902 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/message_handler.py
+-rw-rw-rw-   0        0        0     1956 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/poll_handler.py
+-rw-rw-rw-   0        0        0     2987 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/raw_update_handler.py
+-rw-rw-rw-   0        0        0     2028 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/handlers/user_status_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.680704 fipper-0.0.4.dev1/fipper/methods/
+-rw-rw-rw-   0        0        0     1365 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.688700 fipper-0.0.4.dev1/fipper/methods/advanced/
+-rw-rw-rw-   0        0        0     1017 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/advanced/__init__.py
+-rw-rw-rw-   0        0        0     3206 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/advanced/invoke.py
+-rw-rw-rw-   0        0        0     4673 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/advanced/resolve_peer.py
+-rw-rw-rw-   0        0        0     8382 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/advanced/save_file.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.731672 fipper-0.0.4.dev1/fipper/methods/auth/
+-rw-rw-rw-   0        0        0     1708 2023-06-02 05:49:28.000000 fipper-0.0.4.dev1/fipper/methods/auth/__init__.py
+-rw-rw-rw-   0        0        0     1506 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/accept_terms_of_service.py
+-rw-rw-rw-   0        0        0     1990 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/check_password.py
+-rw-rw-rw-   0        0        0     1829 2023-06-30 09:17:30.000000 fipper-0.0.4.dev1/fipper/methods/auth/connect.py
+-rw-rw-rw-   0        0        0     1540 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/disconnect.py
+-rw-rw-rw-   0        0        0     1339 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/get_password_hint.py
+-rw-rw-rw-   0        0        0     1709 2023-06-02 05:49:28.000000 fipper-0.0.4.dev1/fipper/methods/auth/initialize.py
+-rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/log_out.py
+-rw-rw-rw-   0        0        0     1878 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/recover_password.py
+-rw-rw-rw-   0        0        0     2202 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/resend_code.py
+-rw-rw-rw-   0        0        0     2851 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/send_code.py
+-rw-rw-rw-   0        0        0     1510 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/send_recovery_code.py
+-rw-rw-rw-   0        0        0     3149 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/sign_in.py
+-rw-rw-rw-   0        0        0     2788 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/sign_in_bot.py
+-rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/sign_up.py
+-rw-rw-rw-   0        0        0     1905 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/auth/terminate.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.777644 fipper-0.0.4.dev1/fipper/methods/bots/
+-rw-rw-rw-   0        0        0     2096 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/__init__.py
+-rw-rw-rw-   0        0        0     3386 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/answer_callback_query.py
+-rw-rw-rw-   0        0        0     5090 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/answer_inline_query.py
+-rw-rw-rw-   0        0        0     2030 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/answer_web_app_query.py
+-rw-rw-rw-   0        0        0     2412 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/delete_bot_commands.py
+-rw-rw-rw-   0        0        0     2628 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/get_bot_commands.py
+-rw-rw-rw-   0        0        0     2102 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/get_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2377 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/get_chat_menu_button.py
+-rw-rw-rw-   0        0        0     2860 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/get_game_high_scores.py
+-rw-rw-rw-   0        0        0     3445 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/get_inline_bot_results.py
+-rw-rw-rw-   0        0        0     2918 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/request_callback_answer.py
+-rw-rw-rw-   0        0        0     4044 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/send_game.py
+-rw-rw-rw-   0        0        0     3056 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/send_inline_bot_result.py
+-rw-rw-rw-   0        0        0     2767 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/set_bot_commands.py
+-rw-rw-rw-   0        0        0     3255 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/set_bot_default_privileges.py
+-rw-rw-rw-   0        0        0     2092 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/set_chat_menu_button.py
+-rw-rw-rw-   0        0        0     4036 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/bots/set_game_score.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.868588 fipper-0.0.4.dev1/fipper/methods/chats/
+-rw-rw-rw-   0        0        0     3540 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/__init__.py
+-rw-rw-rw-   0        0        0     3448 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/add_chat_members.py
+-rw-rw-rw-   0        0        0     2281 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/archive_chats.py
+-rw-rw-rw-   0        0        0     4721 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/ban_chat_member.py
+-rw-rw-rw-   0        0        0     1863 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/create_channel.py
+-rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/create_group.py
+-rw-rw-rw-   0        0        0     2003 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/create_supergroup.py
+-rw-rw-rw-   0        0        0     1631 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/delete_channel.py
+-rw-rw-rw-   0        0        0     2371 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/delete_chat_photo.py
+-rw-rw-rw-   0        0        0     1649 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/delete_supergroup.py
+-rw-rw-rw-   0        0        0     2018 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/delete_user_history.py
+-rw-rw-rw-   0        0        0     3355 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat.py
+-rw-rw-rw-   0        0        0     4129 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat_event_log.py
+-rw-rw-rw-   0        0        0     3418 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat_member.py
+-rw-rw-rw-   0        0        0     5420 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat_members.py
+-rw-rw-rw-   0        0        0     2327 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat_members_count.py
+-rw-rw-rw-   0        0        0     1768 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_chat_online_count.py
+-rw-rw-rw-   0        0        0     3456 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_dialogs.py
+-rw-rw-rw-   0        0        0     2153 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_dialogs_count.py
+-rw-rw-rw-   0        0        0     2467 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_nearby_chats.py
+-rw-rw-rw-   0        0        0     2191 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/get_send_as_chats.py
+-rw-rw-rw-   0        0        0     2758 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/join_chat.py
+-rw-rw-rw-   0        0        0     2676 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/leave_chat.py
+-rw-rw-rw-   0        0        0     1569 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/mark_chat_unread.py
+-rw-rw-rw-   0        0        0     3230 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/pin_chat_message.py
+-rw-rw-rw-   0        0        0     3954 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/promote_chat_member.py
+-rw-rw-rw-   0        0        0     4397 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/restrict_chat_member.py
+-rw-rw-rw-   0        0        0     3215 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_administrator_title.py
+-rw-rw-rw-   0        0        0     2307 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_description.py
+-rw-rw-rw-   0        0        0     3488 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_permissions.py
+-rw-rw-rw-   0        0        0     4708 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_photo.py
+-rw-rw-rw-   0        0        0     1774 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_protected_content.py
+-rw-rw-rw-   0        0        0     2644 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_title.py
+-rw-rw-rw-   0        0        0     2356 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_chat_username.py
+-rw-rw-rw-   0        0        0     2031 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_send_as_chat.py
+-rw-rw-rw-   0        0        0     2140 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/set_slow_mode.py
+-rw-rw-rw-   0        0        0     2295 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/unarchive_chats.py
+-rw-rw-rw-   0        0        0     2363 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/unban_chat_member.py
+-rw-rw-rw-   0        0        0     1989 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/unpin_all_chat_messages.py
+-rw-rw-rw-   0        0        0     2194 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/chats/unpin_chat_message.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.882580 fipper-0.0.4.dev1/fipper/methods/contacts/
+-rw-rw-rw-   0        0        0     1187 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/__init__.py
+-rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/add_contact.py
+-rw-rw-rw-   0        0        0     2504 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/delete_contacts.py
+-rw-rw-rw-   0        0        0     1642 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/get_contacts.py
+-rw-rw-rw-   0        0        0     1457 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/get_contacts_count.py
+-rw-rw-rw-   0        0        0     1980 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/contacts/import_contacts.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.911562 fipper-0.0.4.dev1/fipper/methods/decorators/
+-rw-rw-rw-   0        0        0     1671 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0     2213 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_chat_join_request.py
+-rw-rw-rw-   0        0        0     2234 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_chat_member_updated.py
+-rw-rw-rw-   0        0        0     2262 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_chosen_inline_result.py
+-rw-rw-rw-   0        0        0     2228 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_deleted_messages.py
+-rw-rw-rw-   0        0        0     1584 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_disconnect.py
+-rw-rw-rw-   0        0        0     2217 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_edited_message.py
+-rw-rw-rw-   0        0        0     2212 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0     2183 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_message.py
+-rw-rw-rw-   0        0        0     2165 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_poll.py
+-rw-rw-rw-   0        0        0     1861 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_raw_update.py
+-rw-rw-rw-   0        0        0     2197 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/decorators/on_user_status.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.952537 fipper-0.0.4.dev1/fipper/methods/invite_links/
+-rw-rw-rw-   0        0        0     2493 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/approve_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1975 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/approve_chat_join_request.py
+-rw-rw-rw-   0        0        0     3444 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/create_chat_invite_link.py
+-rw-rw-rw-   0        0        0     1944 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/decline_all_chat_join_requests.py
+-rw-rw-rw-   0        0        0     1976 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/decline_chat_join_request.py
+-rw-rw-rw-   0        0        0     2079 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     1797 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/delete_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3615 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/edit_chat_invite_link.py
+-rw-rw-rw-   0        0        0     2637 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/export_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3654 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admin_invite_links.py
+-rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-rw-rw-   0        0        0     2045 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-rw-rw-   0        0        0     1971 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link.py
+-rw-rw-rw-   0        0        0     3003 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-rw-rw-   0        0        0     1979 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-rw-rw-   0        0        0     3023 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_join_requests.py
+-rw-rw-rw-   0        0        0     2387 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/invite_links/revoke_chat_invite_link.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.071464 fipper-0.0.4.dev1/fipper/methods/messages/
+-rw-rw-rw-   0        0        0     4194 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/__init__.py
+-rw-rw-rw-   0        0        0     6095 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/copy_media_group.py
+-rw-rw-rw-   0        0        0     5280 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/copy_message.py
+-rw-rw-rw-   0        0        0     3226 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/delete_messages.py
+-rw-rw-rw-   0        0        0     7705 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/download_media.py
+-rw-rw-rw-   0        0        0     2326 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_caption.py
+-rw-rw-rw-   0        0        0     9990 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_media.py
+-rw-rw-rw-   0        0        0     2519 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_reply_markup.py
+-rw-rw-rw-   0        0        0     3189 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_text.py
+-rw-rw-rw-   0        0        0     3040 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_message_caption.py
+-rw-rw-rw-   0        0        0    12725 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_message_media.py
+-rw-rw-rw-   0        0        0     3039 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_message_reply_markup.py
+-rw-rw-rw-   0        0        0     3986 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/edit_message_text.py
+-rw-rw-rw-   0        0        0     4662 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/forward_messages.py
+-rw-rw-rw-   0        0        0     4152 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_chat_history.py
+-rw-rw-rw-   0        0        0     2455 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_chat_history_count.py
+-rw-rw-rw-   0        0        0     2023 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_custom_emoji_stickers.py
+-rw-rw-rw-   0        0        0     2286 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_message.py
+-rw-rw-rw-   0        0        0     2888 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_replies.py
+-rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_replies_count.py
+-rw-rw-rw-   0        0        0     3011 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_media_group.py
+-rw-rw-rw-   0        0        0     4846 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/get_messages.py
+-rw-rw-rw-   0        0        0     2227 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/inline_session.py
+-rw-rw-rw-   0        0        0     2594 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/read_chat_history.py
+-rw-rw-rw-   0        0        0     2175 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/retract_vote.py
+-rw-rw-rw-   0        0        0     4259 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/search_global.py
+-rw-rw-rw-   0        0        0     2208 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/search_global_count.py
+-rw-rw-rw-   0        0        0     5486 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/search_messages.py
+-rw-rw-rw-   0        0        0     3277 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/search_messages_count.py
+-rw-rw-rw-   0        0        0    12513 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_animation.py
+-rw-rw-rw-   0        0        0    11326 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_audio.py
+-rw-rw-rw-   0        0        0     5579 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_cached_media.py
+-rw-rw-rw-   0        0        0     2887 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_chat_action.py
+-rw-rw-rw-   0        0        0     4970 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_contact.py
+-rw-rw-rw-   0        0        0     4939 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_dice.py
+-rw-rw-rw-   0        0        0    10656 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_document.py
+-rw-rw-rw-   0        0        0     4671 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_location.py
+-rw-rw-rw-   0        0        0    19643 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_media_group.py
+-rw-rw-rw-   0        0        0     7418 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_message.py
+-rw-rw-rw-   0        0        0     9303 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_photo.py
+-rw-rw-rw-   0        0        0     8222 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_poll.py
+-rw-rw-rw-   0        0        0     2428 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_reaction.py
+-rw-rw-rw-   0        0        0     8489 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_sticker.py
+-rw-rw-rw-   0        0        0     5516 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_venue.py
+-rw-rw-rw-   0        0        0    11877 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_video.py
+-rw-rw-rw-   0        0        0     9487 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_video_note.py
+-rw-rw-rw-   0        0        0     9600 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/send_voice.py
+-rw-rw-rw-   0        0        0     2884 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/stop_poll.py
+-rw-rw-rw-   0        0        0     4033 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/stream_media.py
+-rw-rw-rw-   0        0        0     2563 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/vote_poll.py
+-rw-rw-rw-   0        0        0     2895 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/wait_for_callback_query.py
+-rw-rw-rw-   0        0        0     2816 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/messages/wait_for_message.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.080460 fipper-0.0.4.dev1/fipper/methods/password/
+-rw-rw-rw-   0        0        0     1117 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/password/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/password/change_cloud_password.py
+-rw-rw-rw-   0        0        0     3086 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/password/enable_cloud_password.py
+-rw-rw-rw-   0        0        0     2199 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/password/remove_cloud_password.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.132452 fipper-0.0.4.dev1/fipper/methods/users/
+-rw-rw-rw-   0        0        0     1708 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/__init__.py
+-rw-rw-rw-   0        0        0     1819 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/block_user.py
+-rw-rw-rw-   0        0        0     2288 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/delete_profile_photos.py
+-rw-rw-rw-   0        0        0     4548 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_chat_photos.py
+-rw-rw-rw-   0        0        0     2577 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_chat_photos_count.py
+-rw-rw-rw-   0        0        0     2416 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_common_chats.py
+-rw-rw-rw-   0        0        0     1701 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_default_emoji_statuses.py
+-rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_me.py
+-rw-rw-rw-   0        0        0     2621 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/get_users.py
+-rw-rw-rw-   0        0        0     1930 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/set_emoji_status.py
+-rw-rw-rw-   0        0        0     2787 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/set_profile_photo.py
+-rw-rw-rw-   0        0        0     1925 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/set_username.py
+-rw-rw-rw-   0        0        0     1829 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/unblock_user.py
+-rw-rw-rw-   0        0        0     2442 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/users/update_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.161433 fipper-0.0.4.dev1/fipper/methods/utilities/
+-rw-rw-rw-   0        0        0     1292 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/add_handler.py
+-rw-rw-rw-   0        0        0     2300 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/compose.py
+-rw-rw-rw-   0        0        0     1593 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/export_session_string.py
+-rw-rw-rw-   0        0        0     2833 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/idle.py
+-rw-rw-rw-   0        0        0     2259 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/remove_handler.py
+-rw-rw-rw-   0        0        0     2354 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/restart.py
+-rw-rw-rw-   0        0        0     2925 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     2432 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/start.py
+-rw-rw-rw-   0        0        0     2178 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/stop.py
+-rw-rw-rw-   0        0        0     1749 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/methods/utilities/stop_transmission.py
+-rw-rw-rw-   0        0        0    63796 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/mime_types.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.172427 fipper-0.0.4.dev1/fipper/parser/
+-rw-rw-rw-   0        0        0      865 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/parser/__init__.py
+-rw-rw-rw-   0        0        0     7587 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/parser/html.py
+-rw-rw-rw-   0        0        0     5937 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/parser/markdown.py
+-rw-rw-rw-   0        0        0     2132 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/parser/parser.py
+-rw-rw-rw-   0        0        0     1586 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/parser/utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.174427 fipper-0.0.4.dev1/fipper/raw/
+-rw-rw-rw-   0        0        0     1066 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.193414 fipper-0.0.4.dev1/fipper/raw/core/
+-rw-rw-rw-   0        0        0     1343 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/__init__.py
+-rw-rw-rw-   0        0        0     1745 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/future_salt.py
+-rw-rw-rw-   0        0        0     1954 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/future_salts.py
+-rw-rw-rw-   0        0        0     1876 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/gzip_packed.py
+-rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/list.py
+-rw-rw-rw-   0        0        0     1907 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/message.py
+-rw-rw-rw-   0        0        0     1667 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/msg_container.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.212402 fipper-0.0.4.dev1/fipper/raw/core/primitives/
+-rw-rw-rw-   0        0        0     1036 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/bool.py
+-rw-rw-rw-   0        0        0     1814 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/bytes.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/double.py
+-rw-rw-rw-   0        0        0     1403 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/int.py
+-rw-rw-rw-   0        0        0     1225 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/string.py
+-rw-rw-rw-   0        0        0     2081 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/primitives/vector.py
+-rw-rw-rw-   0        0        0     2575 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/raw/core/tl_object.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.219398 fipper-0.0.4.dev1/fipper/session/
+-rw-rw-rw-   0        0        0      891 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/__init__.py
+-rw-rw-rw-   0        0        0    10760 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/auth.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.231391 fipper-0.0.4.dev1/fipper/session/internals/
+-rw-rw-rw-   0        0        0      938 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/internals/__init__.py
+-rw-rw-rw-   0        0        0     2446 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/internals/data_center.py
+-rw-rw-rw-   0        0        0     1406 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/internals/msg_factory.py
+-rw-rw-rw-   0        0        0     1632 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/internals/msg_id.py
+-rw-rw-rw-   0        0        0     1291 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/internals/seq_no.py
+-rw-rw-rw-   0        0        0    12801 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/session/session.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.242384 fipper-0.0.4.dev1/fipper/storage/
+-rw-rw-rw-   0        0        0      949 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/storage/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/storage/file_storage.py
+-rw-rw-rw-   0        0        0     2823 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/storage/memory_storage.py
+-rw-rw-rw-   0        0        0     6638 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/storage/sqlite_storage.py
+-rw-rw-rw-   0        0        0     2872 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/storage/storage.py
+-rw-rw-rw-   0        0        0     3846 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/sync.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.252379 fipper-0.0.4.dev1/fipper/types/
+-rw-rw-rw-   0        0        0     1137 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.262373 fipper-0.0.4.dev1/fipper/types/authorization/
+-rw-rw-rw-   0        0        0      960 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/authorization/__init__.py
+-rw-rw-rw-   0        0        0     2336 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/authorization/sent_code.py
+-rw-rw-rw-   0        0        0     1978 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/authorization/terms_of_service.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.328331 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/
+-rw-rw-rw-   0        0        0     2901 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command.py
+-rw-rw-rw-   0        0        0     2841 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope.py
+-rw-rw-rw-   0        0        0     1319 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-rw-rw-   0        0        0     1284 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-rw-rw-   0        0        0     1275 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-rw-rw-   0        0        0     1599 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-rw-rw-   0        0        0     1676 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-rw-rw-   0        0        0     1859 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-rw-rw-   0        0        0     1335 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-rw-rw-   0        0        0     1058 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/callback_game.py
+-rw-rw-rw-   0        0        0    13062 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/callback_query.py
+-rw-rw-rw-   0        0        0     2443 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/force_reply.py
+-rw-rw-rw-   0        0        0     2276 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/game_high_score.py
+-rw-rw-rw-   0        0        0     8312 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0     2526 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-rw-rw-   0        0        0     3605 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/keyboard_button.py
+-rw-rw-rw-   0        0        0     3800 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/login_url.py
+-rw-rw-rw-   0        0        0     1633 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button.py
+-rw-rw-rw-   0        0        0     1235 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_commands.py
+-rw-rw-rw-   0        0        0     1238 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_default.py
+-rw-rw-rw-   0        0        0     1850 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_web_app.py
+-rw-rw-rw-   0        0        0     4221 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-rw-rw-   0        0        0     2391 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-rw-rw-   0        0        0     1604 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/sent_web_app_message.py
+-rw-rw-rw-   0        0        0     1350 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/web_app_info.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.378301 fipper-0.0.4.dev1/fipper/types/inline_mode/
+-rw-rw-rw-   0        0        0     2802 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/chosen_inline_result.py
+-rw-rw-rw-   0        0        0     7459 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query.py
+-rw-rw-rw-   0        0        0     2434 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result.py
+-rw-rw-rw-   0        0        0     5917 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_animation.py
+-rw-rw-rw-   0        0        0     3391 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     4611 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_audio.py
+-rw-rw-rw-   0        0        0     4339 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_animation.py
+-rw-rw-rw-   0        0        0     4116 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_audio.py
+-rw-rw-rw-   0        0        0     4487 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_document.py
+-rw-rw-rw-   0        0        0     4409 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_photo.py
+-rw-rw-rw-   0        0        0     3099 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-rw-rw-   0        0        0     4494 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_video.py
+-rw-rw-rw-   0        0        0     4296 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_voice.py
+-rw-rw-rw-   0        0        0     4236 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_contact.py
+-rw-rw-rw-   0        0        0     5371 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     4731 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_location.py
+-rw-rw-rw-   0        0        0     5394 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     4875 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_venue.py
+-rw-rw-rw-   0        0        0     5611 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_video.py
+-rw-rw-rw-   0        0        0     4460 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_voice.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.395290 fipper-0.0.4.dev1/fipper/types/input_media/
+-rw-rw-rw-   0        0        0     1344 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/__init__.py
+-rw-rw-rw-   0        0        0     1677 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media.py
+-rw-rw-rw-   0        0        0     3305 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media_animation.py
+-rw-rw-rw-   0        0        0     3358 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media_audio.py
+-rw-rw-rw-   0        0        0     2832 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media_document.py
+-rw-rw-rw-   0        0        0     2536 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media_photo.py
+-rw-rw-rw-   0        0        0     3500 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_media_video.py
+-rw-rw-rw-   0        0        0     1782 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_media/input_phone_contact.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.403285 fipper-0.0.4.dev1/fipper/types/input_message_content/
+-rw-rw-rw-   0        0        0     1030 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_message_content/__init__.py
+-rw-rw-rw-   0        0        0     1441 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_message_content/input_message_content.py
+-rw-rw-rw-   0        0        0     2696 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/input_message_content/input_text_message_content.py
+-rw-rw-rw-   0        0        0     1121 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/list.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.475242 fipper-0.0.4.dev1/fipper/types/messages_and_media/
+-rw-rw-rw-   0        0        0     1883 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/__init__.py
+-rw-rw-rw-   0        0        0     4153 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/animation.py
+-rw-rw-rw-   0        0        0     4178 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/audio.py
+-rw-rw-rw-   0        0        0     2270 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/contact.py
+-rw-rw-rw-   0        0        0     1628 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/dice.py
+-rw-rw-rw-   0        0        0     3495 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/document.py
+-rw-rw-rw-   0        0        0     3131 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/game.py
+-rw-rw-rw-   0        0        0     1709 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/location.py
+-rw-rw-rw-   0        0        0   150486 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/message.py
+-rw-rw-rw-   0        0        0     4456 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/message_entity.py
+-rw-rw-rw-   0        0        0     1846 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/message_reactions.py
+-rw-rw-rw-   0        0        0     4427 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/photo.py
+-rw-rw-rw-   0        0        0     7226 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/poll.py
+-rw-rw-rw-   0        0        0     1578 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/poll_option.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/reaction.py
+-rw-rw-rw-   0        0        0     7101 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/sticker.py
+-rw-rw-rw-   0        0        0     1472 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/stripped_thumbnail.py
+-rw-rw-rw-   0        0        0     3858 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/thumbnail.py
+-rw-rw-rw-   0        0        0     2355 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/venue.py
+-rw-rw-rw-   0        0        0     4511 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/video.py
+-rw-rw-rw-   0        0        0     3697 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/video_note.py
+-rw-rw-rw-   0        0        0     3292 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/voice.py
+-rw-rw-rw-   0        0        0     1614 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/web_app_data.py
+-rw-rw-rw-   0        0        0     6520 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/messages_and_media/web_page.py
+-rw-rw-rw-   0        0        0     3973 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/object.py
+-rw-rw-rw-   0        0        0     1023 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/update.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.532206 fipper-0.0.4.dev1/fipper/types/user_and_chats/
+-rw-rw-rw-   0        0        0     2364 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/__init__.py
+-rw-rw-rw-   0        0        0    33702 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat.py
+-rw-rw-rw-   0        0        0     2289 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-rw-rw-   0        0        0    20240 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_event.py
+-rw-rw-rw-   0        0        0     5687 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_event_filter.py
+-rw-rw-rw-   0        0        0     4699 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_invite_link.py
+-rw-rw-rw-   0        0        0     4364 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_join_request.py
+-rw-rw-rw-   0        0        0     2634 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_joiner.py
+-rw-rw-rw-   0        0        0     9647 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_member.py
+-rw-rw-rw-   0        0        0     3756 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_member_updated.py
+-rw-rw-rw-   0        0        0     4478 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_permissions.py
+-rw-rw-rw-   0        0        0     4066 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_photo.py
+-rw-rw-rw-   0        0        0     2659 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_preview.py
+-rw-rw-rw-   0        0        0     5061 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_privileges.py
+-rw-rw-rw-   0        0        0     2417 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_reactions.py
+-rw-rw-rw-   0        0        0     2749 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/dialog.py
+-rw-rw-rw-   0        0        0     2491 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/emoji_status.py
+-rw-rw-rw-   0        0        0     2006 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/invite_link_importer.py
+-rw-rw-rw-   0        0        0     1711 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/restriction.py
+-rw-rw-rw-   0        0        0    13477 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/user.py
+-rw-rw-rw-   0        0        0     1385 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_ended.py
+-rw-rw-rw-   0        0        0     1656 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_members_invited.py
+-rw-rw-rw-   0        0        0     1572 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_scheduled.py
+-rw-rw-rw-   0        0        0     1072 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_started.py
+-rw-rw-rw-   0        0        0    10933 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/fipper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:34.569770 fipper-0.0.4.dev1/fipper.egg-info/
+-rw-rw-rw-   0        0        0     2202 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17932 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       54 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 09:23:34.000000 fipper-0.0.4.dev1/fipper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       57 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 09:23:35.545199 fipper-0.0.4.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     2106 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.537203 fipper-0.0.4.dev1/tests/
+-rw-rw-rw-   0        0        0      835 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 09:23:35.540201 fipper-0.0.4.dev1/tests/filters/
+-rw-rw-rw-   0        0        0     1237 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/tests/filters/__init__.py
+-rw-rw-rw-   0        0        0     3518 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/tests/filters/test_command.py
+-rw-rw-rw-   0        0        0     8400 2023-06-02 04:40:39.000000 fipper-0.0.4.dev1/tests/test_file_id.py
```

### Comparing `fipper-0.0.3/LICENSE` & `fipper-0.0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/NOTICE` & `fipper-0.0.4.dev1/NOTICE`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/PKG-INFO` & `fipper-0.0.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fipper
-Version: 0.0.3
+Version: 0.0.4.dev1
 Summary: Fipper - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/fipper
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/fipper/issues
 Project-URL: Documentation, https://fipper.tech
```

### Comparing `fipper-0.0.3/README.md` & `fipper-0.0.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/__init__.py` & `fipper-0.0.4.dev1/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/__init__.py` & `fipper-0.0.4.dev1/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/compiler.py` & `fipper-0.0.4.dev1/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/source/auth_key.tl` & `fipper-0.0.4.dev1/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/source/main_api.tl` & `fipper-0.0.4.dev1/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/source/sys_msgs.tl` & `fipper-0.0.4.dev1/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/template/combinator.txt` & `fipper-0.0.4.dev1/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/api/template/type.txt` & `fipper-0.0.4.dev1/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/__init__.py` & `fipper-0.0.4.dev1/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/compiler.py` & `fipper-0.0.4.dev1/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/sort.py` & `fipper-0.0.4.dev1/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/source/400_BAD_REQUEST.tsv` & `fipper-0.0.4.dev1/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/source/401_UNAUTHORIZED.tsv` & `fipper-0.0.4.dev1/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/source/403_FORBIDDEN.tsv` & `fipper-0.0.4.dev1/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `fipper-0.0.4.dev1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `fipper-0.0.4.dev1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/__init__.py` & `fipper-0.0.4.dev1/fipper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.0.3"
+__version__ = "0.0.4.dev01"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `fipper-0.0.3/fipper/client.py` & `fipper-0.0.4.dev1/fipper/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             The *api_id* part of the Telegram API key, as integer or string.
             E.g.: 12345 or "12345".
 
         api_hash (``str``, *optional*):
             The *api_hash* part of the Telegram API key, as string.
             E.g.: "0123456789abcdef0123456789abcdef".
 
+        hndlr (``str`` | ``list`` | *optional*):
+            The *api_hash* part of the Client Handler, as string or list.
+            E.g.: "." or [".", ",", ">", "<", "?"].
+
         app_version (``str``, *optional*):
             Application version.
             Defaults to "Pyrogram x.y.z".
 
         device_model (``str``, *optional*):
             Device model.
             Defaults to *platform.python_implementation() + " " + platform.python_version()*.
@@ -190,14 +194,15 @@
     mimetypes.readfp(StringIO(mime_types))
 
     def __init__(
         self,
         name: str,
         api_id: Union[int, str] = None,
         api_hash: str = None,
+        hndlr: Union[str, list] = None,
         app_version: str = APP_VERSION,
         device_model: str = DEVICE_MODEL,
         system_version: str = SYSTEM_VERSION,
         lang_code: str = LANG_CODE,
         ipv6: bool = False,
         proxy: dict = None,
         test_mode: bool = False,
@@ -217,14 +222,15 @@
         hide_password: bool = False
     ):
         super().__init__()
 
         self.name = name
         self.api_id = int(api_id) if api_id else None
         self.api_hash = api_hash
+        self.hndlr = hndlr if hndlr else [".", ",", ">", "<", "?"]
         self.app_version = app_version
         self.device_model = device_model
         self.system_version = system_version
         self.lang_code = lang_code
         self.ipv6 = ipv6
         self.proxy = proxy
         self.test_mode = test_mode
@@ -273,14 +279,16 @@
         self.me: Optional[User] = None
 
         self.message_cache = Cache(10000)
 
         self.loop = asyncio.get_event_loop()
 
         self.listening = {}
+        
+        self.hndlring = {}
 
     def __enter__(self):
         return self.start()
 
     def __exit__(self, *args):
         try:
             self.stop()
@@ -324,14 +332,24 @@
         listener = self.listening.get(chat_id)
         if not listener or listener['future'].done():
             return
 
         listener['future'].set_exception(ListenerCanceled())
         self.clear_listener(chat_id, listener['future'])
 
+    async def load_hndlr(self):
+        await self.set_hndlr(self.hndlr)
+
+    async def set_hndlr(self, value: list):
+        return self.hndlring.update({"me": {"hndlr": value}})
+
+    def get_hndlr(self):
+        handle = self.hndlring.get("me")
+        return handle['hndlr']
+
 
     async def authorize(self) -> User:
         if self.bot_token:
             return await self.sign_in_bot(self.bot_token)
 
         print(f"Welcome to Pyrogram (version {__version__})")
         print(f"Pyrogram is free software and comes with ABSOLUTELY NO WARRANTY. Licensed\n"
```

### Comparing `fipper-0.0.3/fipper/connection/__init__.py` & `fipper-0.0.4.dev1/fipper/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/connection.py` & `fipper-0.0.4.dev1/fipper/connection/connection.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/__init__.py` & `fipper-0.0.4.dev1/fipper/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/__init__.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp_abridged.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp_abridged_o.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp_full.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp_intermediate.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/connection/transport/tcp/tcp_intermediate_o.py` & `fipper-0.0.4.dev1/fipper/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/crypto/__init__.py` & `fipper-0.0.4.dev1/fipper/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/crypto/aes.py` & `fipper-0.0.4.dev1/fipper/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/crypto/mtproto.py` & `fipper-0.0.4.dev1/fipper/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/crypto/prime.py` & `fipper-0.0.4.dev1/fipper/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/crypto/rsa.py` & `fipper-0.0.4.dev1/fipper/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/dispatcher.py` & `fipper-0.0.4.dev1/fipper/dispatcher.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/emoji.py` & `fipper-0.0.4.dev1/fipper/emoji.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/__init__.py` & `fipper-0.0.4.dev1/fipper/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/auto_name.py` & `fipper-0.0.4.dev1/fipper/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/chat_action.py` & `fipper-0.0.4.dev1/fipper/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/chat_event_action.py` & `fipper-0.0.4.dev1/fipper/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/chat_member_status.py` & `fipper-0.0.4.dev1/fipper/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/chat_members_filter.py` & `fipper-0.0.4.dev1/fipper/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/chat_type.py` & `fipper-0.0.4.dev1/fipper/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/message_entity_type.py` & `fipper-0.0.4.dev1/fipper/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/message_media_type.py` & `fipper-0.0.4.dev1/fipper/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/message_service_type.py` & `fipper-0.0.4.dev1/fipper/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/messages_filter.py` & `fipper-0.0.4.dev1/fipper/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/next_code_type.py` & `fipper-0.0.4.dev1/fipper/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/parse_mode.py` & `fipper-0.0.4.dev1/fipper/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/poll_type.py` & `fipper-0.0.4.dev1/fipper/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/sent_code_type.py` & `fipper-0.0.4.dev1/fipper/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/enums/user_status.py` & `fipper-0.0.4.dev1/fipper/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/errors/__init__.py` & `fipper-0.0.4.dev1/fipper/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/errors/rpc_error.py` & `fipper-0.0.4.dev1/fipper/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/file_id.py` & `fipper-0.0.4.dev1/fipper/file_id.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/filters.py` & `fipper-0.0.4.dev1/fipper/filters.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/__init__.py` & `fipper-0.0.4.dev1/fipper/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/callback_query_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/chat_join_request_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/chat_member_updated_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/chosen_inline_result_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/conversation_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/conversation_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/deleted_messages_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/disconnect_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/edited_message_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/handler.py` & `fipper-0.0.4.dev1/fipper/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/inline_query_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/message_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/poll_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/raw_update_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/handlers/user_status_handler.py` & `fipper-0.0.4.dev1/fipper/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/advanced/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/advanced/invoke.py` & `fipper-0.0.4.dev1/fipper/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/advanced/resolve_peer.py` & `fipper-0.0.4.dev1/fipper/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/advanced/save_file.py` & `fipper-0.0.4.dev1/fipper/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/accept_terms_of_service.py` & `fipper-0.0.4.dev1/fipper/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/check_password.py` & `fipper-0.0.4.dev1/fipper/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/connect.py` & `fipper-0.0.4.dev1/fipper/methods/auth/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             ConnectionError: In case you try to connect an already connected client.
         """
         if self.is_connected:
             raise ConnectionError("Client is already connected")
 
         await self.load_session()
 
+        await self.load_hndlr()
+
         self.session = Session(
             self, await self.storage.dc_id(),
             await self.storage.auth_key(), await self.storage.test_mode()
         )
 
         await self.session.start()
```

### Comparing `fipper-0.0.3/fipper/methods/auth/disconnect.py` & `fipper-0.0.4.dev1/fipper/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/get_password_hint.py` & `fipper-0.0.4.dev1/fipper/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/initialize.py` & `fipper-0.0.4.dev1/fipper/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/log_out.py` & `fipper-0.0.4.dev1/fipper/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/recover_password.py` & `fipper-0.0.4.dev1/fipper/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/resend_code.py` & `fipper-0.0.4.dev1/fipper/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/send_code.py` & `fipper-0.0.4.dev1/fipper/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/send_recovery_code.py` & `fipper-0.0.4.dev1/fipper/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/sign_in.py` & `fipper-0.0.4.dev1/fipper/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/sign_in_bot.py` & `fipper-0.0.4.dev1/fipper/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/sign_up.py` & `fipper-0.0.4.dev1/fipper/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/auth/terminate.py` & `fipper-0.0.4.dev1/fipper/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/answer_callback_query.py` & `fipper-0.0.4.dev1/fipper/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/answer_inline_query.py` & `fipper-0.0.4.dev1/fipper/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/answer_web_app_query.py` & `fipper-0.0.4.dev1/fipper/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/delete_bot_commands.py` & `fipper-0.0.4.dev1/fipper/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/get_bot_commands.py` & `fipper-0.0.4.dev1/fipper/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/get_bot_default_privileges.py` & `fipper-0.0.4.dev1/fipper/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/get_chat_menu_button.py` & `fipper-0.0.4.dev1/fipper/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/get_game_high_scores.py` & `fipper-0.0.4.dev1/fipper/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/get_inline_bot_results.py` & `fipper-0.0.4.dev1/fipper/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/request_callback_answer.py` & `fipper-0.0.4.dev1/fipper/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/send_game.py` & `fipper-0.0.4.dev1/fipper/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/send_inline_bot_result.py` & `fipper-0.0.4.dev1/fipper/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/set_bot_commands.py` & `fipper-0.0.4.dev1/fipper/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/set_bot_default_privileges.py` & `fipper-0.0.4.dev1/fipper/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/set_chat_menu_button.py` & `fipper-0.0.4.dev1/fipper/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/bots/set_game_score.py` & `fipper-0.0.4.dev1/fipper/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/add_chat_members.py` & `fipper-0.0.4.dev1/fipper/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/archive_chats.py` & `fipper-0.0.4.dev1/fipper/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/ban_chat_member.py` & `fipper-0.0.4.dev1/fipper/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/create_channel.py` & `fipper-0.0.4.dev1/fipper/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/create_group.py` & `fipper-0.0.4.dev1/fipper/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/create_supergroup.py` & `fipper-0.0.4.dev1/fipper/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/delete_channel.py` & `fipper-0.0.4.dev1/fipper/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/delete_chat_photo.py` & `fipper-0.0.4.dev1/fipper/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/delete_supergroup.py` & `fipper-0.0.4.dev1/fipper/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/delete_user_history.py` & `fipper-0.0.4.dev1/fipper/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat_event_log.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat_member.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat_members.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat_members_count.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_chat_online_count.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_dialogs.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_dialogs_count.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_nearby_chats.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/get_send_as_chats.py` & `fipper-0.0.4.dev1/fipper/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/join_chat.py` & `fipper-0.0.4.dev1/fipper/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/leave_chat.py` & `fipper-0.0.4.dev1/fipper/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/mark_chat_unread.py` & `fipper-0.0.4.dev1/fipper/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/pin_chat_message.py` & `fipper-0.0.4.dev1/fipper/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/promote_chat_member.py` & `fipper-0.0.4.dev1/fipper/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/restrict_chat_member.py` & `fipper-0.0.4.dev1/fipper/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_administrator_title.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_description.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_permissions.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_photo.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_protected_content.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_title.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_chat_username.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_send_as_chat.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/set_slow_mode.py` & `fipper-0.0.4.dev1/fipper/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/unarchive_chats.py` & `fipper-0.0.4.dev1/fipper/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/unban_chat_member.py` & `fipper-0.0.4.dev1/fipper/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/unpin_all_chat_messages.py` & `fipper-0.0.4.dev1/fipper/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/chats/unpin_chat_message.py` & `fipper-0.0.4.dev1/fipper/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/add_contact.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/delete_contacts.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/get_contacts.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/get_contacts_count.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/contacts/import_contacts.py` & `fipper-0.0.4.dev1/fipper/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_callback_query.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_chat_join_request.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_chat_member_updated.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_chosen_inline_result.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_deleted_messages.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_disconnect.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_edited_message.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_inline_query.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_message.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_poll.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_raw_update.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/decorators/on_user_status.py` & `fipper-0.0.4.dev1/fipper/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/approve_all_chat_join_requests.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/approve_chat_join_request.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/create_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/decline_all_chat_join_requests.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/decline_chat_join_request.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/delete_chat_admin_invite_links.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/delete_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/edit_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/export_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_admin_invite_links.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_admin_invite_links_count.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_admins_with_invite_links.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link_joiners.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/get_chat_join_requests.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/invite_links/revoke_chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/copy_media_group.py` & `fipper-0.0.4.dev1/fipper/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/copy_message.py` & `fipper-0.0.4.dev1/fipper/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/delete_messages.py` & `fipper-0.0.4.dev1/fipper/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/download_media.py` & `fipper-0.0.4.dev1/fipper/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_inline_caption.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_inline_media.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_inline_reply_markup.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_inline_text.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_message_caption.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_message_media.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_message_reply_markup.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/edit_message_text.py` & `fipper-0.0.4.dev1/fipper/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/forward_messages.py` & `fipper-0.0.4.dev1/fipper/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_chat_history.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_chat_history_count.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_custom_emoji_stickers.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_discussion_message.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_discussion_replies.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_discussion_replies_count.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_media_group.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/get_messages.py` & `fipper-0.0.4.dev1/fipper/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/inline_session.py` & `fipper-0.0.4.dev1/fipper/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/read_chat_history.py` & `fipper-0.0.4.dev1/fipper/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/retract_vote.py` & `fipper-0.0.4.dev1/fipper/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/search_global.py` & `fipper-0.0.4.dev1/fipper/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/search_global_count.py` & `fipper-0.0.4.dev1/fipper/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/search_messages.py` & `fipper-0.0.4.dev1/fipper/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/search_messages_count.py` & `fipper-0.0.4.dev1/fipper/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_animation.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_audio.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_cached_media.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_chat_action.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_contact.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_dice.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_document.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_location.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_media_group.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_message.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_photo.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_poll.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_reaction.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_sticker.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_venue.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_video.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_video_note.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/send_voice.py` & `fipper-0.0.4.dev1/fipper/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/stop_poll.py` & `fipper-0.0.4.dev1/fipper/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/stream_media.py` & `fipper-0.0.4.dev1/fipper/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/vote_poll.py` & `fipper-0.0.4.dev1/fipper/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/wait_for_callback_query.py` & `fipper-0.0.4.dev1/fipper/methods/messages/wait_for_callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/messages/wait_for_message.py` & `fipper-0.0.4.dev1/fipper/methods/messages/wait_for_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/password/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/password/change_cloud_password.py` & `fipper-0.0.4.dev1/fipper/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/password/enable_cloud_password.py` & `fipper-0.0.4.dev1/fipper/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/password/remove_cloud_password.py` & `fipper-0.0.4.dev1/fipper/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/block_user.py` & `fipper-0.0.4.dev1/fipper/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/delete_profile_photos.py` & `fipper-0.0.4.dev1/fipper/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_chat_photos.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_chat_photos_count.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_common_chats.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_default_emoji_statuses.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_me.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/get_users.py` & `fipper-0.0.4.dev1/fipper/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/set_emoji_status.py` & `fipper-0.0.4.dev1/fipper/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/set_profile_photo.py` & `fipper-0.0.4.dev1/fipper/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/set_username.py` & `fipper-0.0.4.dev1/fipper/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/unblock_user.py` & `fipper-0.0.4.dev1/fipper/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/users/update_profile.py` & `fipper-0.0.4.dev1/fipper/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/__init__.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/add_handler.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/compose.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/export_session_string.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/idle.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/remove_handler.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/restart.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/run.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/start.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/stop.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/methods/utilities/stop_transmission.py` & `fipper-0.0.4.dev1/fipper/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/mime_types.py` & `fipper-0.0.4.dev1/fipper/mime_types.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/parser/__init__.py` & `fipper-0.0.4.dev1/fipper/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/parser/html.py` & `fipper-0.0.4.dev1/fipper/parser/html.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/parser/markdown.py` & `fipper-0.0.4.dev1/fipper/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/parser/parser.py` & `fipper-0.0.4.dev1/fipper/parser/parser.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/parser/utils.py` & `fipper-0.0.4.dev1/fipper/parser/utils.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/__init__.py` & `fipper-0.0.4.dev1/fipper/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/__init__.py` & `fipper-0.0.4.dev1/fipper/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/future_salt.py` & `fipper-0.0.4.dev1/fipper/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/future_salts.py` & `fipper-0.0.4.dev1/fipper/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/gzip_packed.py` & `fipper-0.0.4.dev1/fipper/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/list.py` & `fipper-0.0.4.dev1/fipper/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/message.py` & `fipper-0.0.4.dev1/fipper/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/msg_container.py` & `fipper-0.0.4.dev1/fipper/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/__init__.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/bool.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/bytes.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/double.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/int.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/string.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/primitives/vector.py` & `fipper-0.0.4.dev1/fipper/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/raw/core/tl_object.py` & `fipper-0.0.4.dev1/fipper/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/__init__.py` & `fipper-0.0.4.dev1/fipper/session/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/auth.py` & `fipper-0.0.4.dev1/fipper/session/auth.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/internals/__init__.py` & `fipper-0.0.4.dev1/fipper/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/internals/data_center.py` & `fipper-0.0.4.dev1/fipper/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/internals/msg_factory.py` & `fipper-0.0.4.dev1/fipper/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/internals/msg_id.py` & `fipper-0.0.4.dev1/fipper/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/internals/seq_no.py` & `fipper-0.0.4.dev1/fipper/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/session/session.py` & `fipper-0.0.4.dev1/fipper/session/session.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/storage/__init__.py` & `fipper-0.0.4.dev1/fipper/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/storage/file_storage.py` & `fipper-0.0.4.dev1/fipper/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/storage/memory_storage.py` & `fipper-0.0.4.dev1/fipper/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/storage/sqlite_storage.py` & `fipper-0.0.4.dev1/fipper/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/storage/storage.py` & `fipper-0.0.4.dev1/fipper/storage/storage.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/sync.py` & `fipper-0.0.4.dev1/fipper/sync.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/__init__.py` & `fipper-0.0.4.dev1/fipper/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/authorization/__init__.py` & `fipper-0.0.4.dev1/fipper/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/authorization/sent_code.py` & `fipper-0.0.4.dev1/fipper/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/authorization/terms_of_service.py` & `fipper-0.0.4.dev1/fipper/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/__init__.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/bot_command_scope_default.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/callback_game.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/callback_query.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/force_reply.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/game_high_score.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/inline_keyboard_button.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/inline_keyboard_markup.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/keyboard_button.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/login_url.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_commands.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_default.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/menu_button_web_app.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/reply_keyboard_markup.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/reply_keyboard_remove.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/sent_web_app_message.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/bots_and_keyboards/web_app_info.py` & `fipper-0.0.4.dev1/fipper/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/__init__.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/chosen_inline_result.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_animation.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_article.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_audio.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_animation.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_audio.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_document.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_photo.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_sticker.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_video.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_cached_voice.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_contact.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_document.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_location.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_photo.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_venue.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_video.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/inline_mode/inline_query_result_voice.py` & `fipper-0.0.4.dev1/fipper/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/__init__.py` & `fipper-0.0.4.dev1/fipper/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media_animation.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media_audio.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media_document.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media_photo.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_media_video.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_media/input_phone_contact.py` & `fipper-0.0.4.dev1/fipper/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_message_content/__init__.py` & `fipper-0.0.4.dev1/fipper/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_message_content/input_message_content.py` & `fipper-0.0.4.dev1/fipper/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/input_message_content/input_text_message_content.py` & `fipper-0.0.4.dev1/fipper/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/list.py` & `fipper-0.0.4.dev1/fipper/types/list.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/__init__.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/animation.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/audio.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/contact.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/dice.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/document.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/game.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/location.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/message.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/message_entity.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/message_reactions.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/photo.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/poll.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/poll_option.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/reaction.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/sticker.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/stripped_thumbnail.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/thumbnail.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/venue.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/video.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/video_note.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/voice.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/web_app_data.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/messages_and_media/web_page.py` & `fipper-0.0.4.dev1/fipper/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/object.py` & `fipper-0.0.4.dev1/fipper/types/object.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/update.py` & `fipper-0.0.4.dev1/fipper/types/update.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/__init__.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_admin_with_invite_links.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_event.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_event_filter.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_invite_link.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_join_request.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_joiner.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_member.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_member_updated.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_permissions.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_photo.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_preview.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_privileges.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/chat_reactions.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/dialog.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/emoji_status.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/invite_link_importer.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/restriction.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/user.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/video_chat_ended.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/video_chat_members_invited.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/video_chat_scheduled.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/types/user_and_chats/video_chat_started.py` & `fipper-0.0.4.dev1/fipper/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper/utils.py` & `fipper-0.0.4.dev1/fipper/utils.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/fipper.egg-info/PKG-INFO` & `fipper-0.0.4.dev1/fipper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fipper
-Version: 0.0.3
+Version: 0.0.4.dev1
 Summary: Fipper - Telegram MTProto API Client Library for Python.
 Home-page: https://github.com/AyiinXd/fipper
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU Lesser General Public License v3.0 (LGPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/fipper/issues
 Project-URL: Documentation, https://fipper.tech
```

### Comparing `fipper-0.0.3/fipper.egg-info/SOURCES.txt` & `fipper-0.0.4.dev1/fipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/setup.py` & `fipper-0.0.4.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/tests/__init__.py` & `fipper-0.0.4.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/tests/filters/__init__.py` & `fipper-0.0.4.dev1/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/tests/filters/test_command.py` & `fipper-0.0.4.dev1/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `fipper-0.0.3/tests/test_file_id.py` & `fipper-0.0.4.dev1/tests/test_file_id.py`

 * *Files identical despite different names*

