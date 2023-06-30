# Comparing `tmp/pyroherd-0.0.0.tar.gz` & `tmp/pyroherd-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroherd-0.0.0.tar", last modified: Fri Jun 30 03:08:08 2023, max compression
+gzip compressed data, was "pyroherd-0.0.1.tar", last modified: Fri Jun 30 03:49:13 2023, max compression
```

## Comparing `pyroherd-0.0.0.tar` & `pyroherd-0.0.1.tar`

### file list

```diff
@@ -1,478 +1,478 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.212864 pyroherd-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 03:07:56.000000 pyroherd-0.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 03:07:56.000000 pyroherd-0.0.0/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 03:07:56.000000 pyroherd-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 03:07:56.000000 pyroherd-0.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-30 03:08:08.212864 pyroherd-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 03:07:56.000000 pyroherd-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   148190 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.156863 pyroherd-0.0.0/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 03:07:56.000000 pyroherd-0.0.0/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.160863 pyroherd-0.0.0/pyroherd/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38806 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.160863 pyroherd-0.0.0/pyroherd/connection/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.160863 pyroherd-0.0.0/pyroherd/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.160863 pyroherd-0.0.0/pyroherd/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.164863 pyroherd-0.0.0/pyroherd/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   207202 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.164863 pyroherd-0.0.0/pyroherd/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.164863 pyroherd-0.0.0/pyroherd/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    23772 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.168863 pyroherd-0.0.0/pyroherd/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.168863 pyroherd-0.0.0/pyroherd/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.168863 pyroherd-0.0.0/pyroherd/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.168863 pyroherd-0.0.0/pyroherd/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.172863 pyroherd-0.0.0/pyroherd/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.176863 pyroherd-0.0.0/pyroherd/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.176863 pyroherd-0.0.0/pyroherd/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.180863 pyroherd-0.0.0/pyroherd/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_cb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.184863 pyroherd-0.0.0/pyroherd/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.188863 pyroherd-0.0.0/pyroherd/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.188863 pyroherd-0.0.0/pyroherd/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.192863 pyroherd-0.0.0/pyroherd/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.192863 pyroherd-0.0.0/pyroherd/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    60961 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.192863 pyroherd-0.0.0/pyroherd/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.192863 pyroherd-0.0.0/pyroherd/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/session/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.196863 pyroherd-0.0.0/pyroherd/types/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.200863 pyroherd-0.0.0/pyroherd/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.200863 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.204863 pyroherd-0.0.0/pyroherd/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.204863 pyroherd-0.0.0/pyroherd/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.204863 pyroherd-0.0.0/pyroherd/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.208863 pyroherd-0.0.0/pyroherd/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   142656 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.212864 pyroherd-0.0.0/pyroherd/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-30 03:07:56.000000 pyroherd-0.0.0/pyroherd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.160863 pyroherd-0.0.0/pyroherd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-30 03:08:08.000000 pyroherd-0.0.0/pyroherd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-06-30 03:08:08.000000 pyroherd-0.0.0/pyroherd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:08:08.000000 pyroherd-0.0.0/pyroherd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:08:07.000000 pyroherd-0.0.0/pyroherd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:08:08.000000 pyroherd-0.0.0/pyroherd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 03:08:08.000000 pyroherd-0.0.0/pyroherd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:07:56.000000 pyroherd-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:08:08.212864 pyroherd-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 03:07:56.000000 pyroherd-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.212864 pyroherd-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:07:56.000000 pyroherd-0.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:08:08.212864 pyroherd-0.0.0/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 03:07:56.000000 pyroherd-0.0.0/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 03:07:56.000000 pyroherd-0.0.0/tests/filters/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-30 03:07:56.000000 pyroherd-0.0.0/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.029754 pyroherd-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-30 03:48:58.000000 pyroherd-0.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-30 03:48:58.000000 pyroherd-0.0.1/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 03:48:58.000000 pyroherd-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-30 03:48:58.000000 pyroherd-0.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-30 03:49:13.029754 pyroherd-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-30 03:48:58.000000 pyroherd-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.961750 pyroherd-0.0.1/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.961750 pyroherd-0.0.1/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.961750 pyroherd-0.0.1/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   148190 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.965751 pyroherd-0.0.1/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.965751 pyroherd-0.0.1/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.965751 pyroherd-0.0.1/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.965751 pyroherd-0.0.1/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 03:48:58.000000 pyroherd-0.0.1/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38806 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207202 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.973751 pyroherd-0.0.1/pyroherd/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.973751 pyroherd-0.0.1/pyroherd/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23772 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.977751 pyroherd-0.0.1/pyroherd/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.977751 pyroherd-0.0.1/pyroherd/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.977751 pyroherd-0.0.1/pyroherd/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.977751 pyroherd-0.0.1/pyroherd/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.981752 pyroherd-0.0.1/pyroherd/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.989752 pyroherd-0.0.1/pyroherd/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.989752 pyroherd-0.0.1/pyroherd/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.989752 pyroherd-0.0.1/pyroherd/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_cb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.993752 pyroherd-0.0.1/pyroherd/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.001753 pyroherd-0.0.1/pyroherd/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.001753 pyroherd-0.0.1/pyroherd/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.005753 pyroherd-0.0.1/pyroherd/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.005753 pyroherd-0.0.1/pyroherd/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60961 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.005753 pyroherd-0.0.1/pyroherd/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.005753 pyroherd-0.0.1/pyroherd/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/session/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.009753 pyroherd-0.0.1/pyroherd/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.013754 pyroherd-0.0.1/pyroherd/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.017754 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.017754 pyroherd-0.0.1/pyroherd/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.021754 pyroherd-0.0.1/pyroherd/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.021754 pyroherd-0.0.1/pyroherd/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.025754 pyroherd-0.0.1/pyroherd/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142656 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.029754 pyroherd-0.0.1/pyroherd/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-30 03:48:58.000000 pyroherd-0.0.1/pyroherd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:12.969751 pyroherd-0.0.1/pyroherd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 03:49:12.000000 pyroherd-0.0.1/pyroherd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 03:48:58.000000 pyroherd-0.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:49:13.029754 pyroherd-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 03:48:58.000000 pyroherd-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.029754 pyroherd-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 03:48:58.000000 pyroherd-0.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:49:13.029754 pyroherd-0.0.1/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 03:48:58.000000 pyroherd-0.0.1/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 03:48:58.000000 pyroherd-0.0.1/tests/filters/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-30 03:48:58.000000 pyroherd-0.0.1/tests/test_file_id.py
```

### Comparing `pyroherd-0.0.0/COPYING` & `pyroherd-0.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/COPYING.lesser` & `pyroherd-0.0.1/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/NOTICE` & `pyroherd-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/PKG-INFO` & `pyroherd-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroherd
-Version: 0.0.0
+Version: 0.0.1
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/OnTheHerd
 Download-URL: https://github.com/OnTheHerd/pyroherd/releases/latest
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/OnTheHerd/pyroherd/issues
```

### Comparing `pyroherd-0.0.0/README.md` & `pyroherd-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/compiler.py` & `pyroherd-0.0.1/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/source/auth_key.tl` & `pyroherd-0.0.1/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/source/main_api.tl` & `pyroherd-0.0.1/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/source/sys_msgs.tl` & `pyroherd-0.0.1/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/template/combinator.txt` & `pyroherd-0.0.1/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/api/template/type.txt` & `pyroherd-0.0.1/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/compiler.py` & `pyroherd-0.0.1/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyroherd-0.0.1/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyroherd-0.0.1/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/source/403_FORBIDDEN.tsv` & `pyroherd-0.0.1/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyroherd-0.0.1/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyroherd-0.0.1/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/__init__.py` & `pyroherd-0.0.1/pyroherd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2023-present OTH <https://github.com/OTHFamily>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyroherd-0.0.0/pyroherd/client.py` & `pyroherd-0.0.1/pyroherd/client.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/connection.py` & `pyroherd-0.0.1/pyroherd/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import socket
 import time
 
 try:
     import socks
 except ImportError as e:
     e.msg = (
-        "PySocks is missing and Pyrogram can't run without. "
+        "PySocks is missing and Pyroherd can't run without. "
         "Please install it using \"pip3 install pysocks\"."
     )
 
     raise e
 
 log = logging.getLogger(__name__)
```

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_abridged.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_abridged_o.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_full.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_intermediate.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/connection/transport/tcp/tcp_intermediate_o.py` & `pyroherd-0.0.1/pyroherd/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/crypto/aes.py` & `pyroherd-0.0.1/pyroherd/crypto/aes.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             "big",
         )
 except ImportError:
     import pyaes
 
     log.warning(
         "TgCrypto is missing! "
-        "Pyrogram will work the same, but at a much slower speed. "
-        "More info: https://docs.pyrogram.org/topics/speedups"
+        "Pyrogram will work the same, but at a much slower speed."
     )
 
 
     def ige256_encrypt(data: bytes, key: bytes, iv: bytes) -> bytes:
         return ige(data, key, iv, True)
```

### Comparing `pyroherd-0.0.0/pyroherd/crypto/mtproto.py` & `pyroherd-0.0.1/pyroherd/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/crypto/prime.py` & `pyroherd-0.0.1/pyroherd/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/crypto/rsa.py` & `pyroherd-0.0.1/pyroherd/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/dispatcher.py` & `pyroherd-0.0.1/pyroherd/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/emoji.py` & `pyroherd-0.0.1/pyroherd/emoji.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/enums/__init__.py` & `pyroherd-0.0.1/pyroherd/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/enums/chat_action.py` & `pyroherd-0.0.1/pyroherd/enums/chat_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
 class ChatAction(AutoName):
-    """Chat action enumeration used in :obj:`~pyrosex.types.ChatEvent`."""
+    """Chat action enumeration used in :obj:`~pyroherd.types.ChatEvent`."""
 
     TYPING = raw.types.SendMessageTypingAction
     "Typing text message"
 
     UPLOAD_PHOTO = raw.types.SendMessageUploadPhotoAction
     "Uploading photo"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/chat_event_action.py` & `pyroherd-0.0.1/pyroherd/enums/chat_event_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import auto
 
 from .auto_name import AutoName
 
 
 class ChatEventAction(AutoName):
-    """Chat event action enumeration used in :meth:`~pyrosex.Client.get_chat_event_log`."""
+    """Chat event action enumeration used in :meth:`~pyroherd.Client.get_chat_event_log`."""
 
     DESCRIPTION_CHANGED = auto()
     "The chat description has been changed (see ``old_description`` and ``new_description``)"
 
     HISTORY_TTL_CHANGED = auto()
     "The history time-to-live has been changed (see ``old_history_ttl`` and ``new_history_ttl``)"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/chat_members_filter.py` & `pyroherd-0.0.1/pyroherd/enums/chat_members_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
 class ChatMembersFilter(AutoName):
-    """Chat members filter enumeration used in :meth:`~pyrosex.Client.get_chat_members`"""
+    """Chat members filter enumeration used in :meth:`~pyroherd.Client.get_chat_members`"""
 
     SEARCH = raw.types.ChannelParticipantsSearch
     "Search for members"
 
     BANNED = raw.types.ChannelParticipantsKicked
     "Banned members"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/message_entity_type.py` & `pyroherd-0.0.1/pyroherd/enums/message_entity_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
 class MessageEntityType(AutoName):
-    """Message entity type enumeration used in :obj:`~pyrosex.types.MessageEntity`."""
+    """Message entity type enumeration used in :obj:`~pyroherd.types.MessageEntity`."""
 
     MENTION = raw.types.MessageEntityMention
     "``@username``"
 
     HASHTAG = raw.types.MessageEntityHashtag
     "``#hashtag``"
 
     CASHTAG = raw.types.MessageEntityCashtag
     "``$USD``"
 
     BOT_COMMAND = raw.types.MessageEntityBotCommand
-    "``/start@pyrosexbot``"
+    "``/start@pyroherdbot``"
 
     URL = raw.types.MessageEntityUrl
-    "``https://pyrosex.org`` (see ``url``)"
+    "``https://pyroherd.org`` (see ``url``)"
 
     EMAIL = raw.types.MessageEntityEmail
-    "``do-not-reply@pyrosex.org``"
+    "``do-not-reply@pyroherd.org``"
 
     PHONE_NUMBER = raw.types.MessageEntityPhone
     "``+1-123-456-7890``"
 
     BOLD = raw.types.MessageEntityBold
     "Bold text"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/message_media_type.py` & `pyroherd-0.0.1/pyroherd/enums/message_media_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import auto
 
 from .auto_name import AutoName
 
 
 class MessageMediaType(AutoName):
-    """Message media type enumeration used in :obj:`~pyrosex.types.Message`."""
+    """Message media type enumeration used in :obj:`~pyroherd.types.Message`."""
 
     AUDIO = auto()
     "Audio media"
 
     DOCUMENT = auto()
     "Document media"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/message_service_type.py` & `pyroherd-0.0.1/pyroherd/enums/message_service_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import auto
 
 from .auto_name import AutoName
 
 
 class MessageServiceType(AutoName):
-    """Message service type enumeration used in :obj:`~pyrosex.types.Message`."""
+    """Message service type enumeration used in :obj:`~pyroherd.types.Message`."""
 
     NEW_CHAT_MEMBERS = auto()
     "New members join"
 
     LEFT_CHAT_MEMBERS = auto()
     "Left chat members"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/messages_filter.py` & `pyroherd-0.0.1/pyroherd/enums/messages_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
 class MessagesFilter(AutoName):
-    """Messages filter enumeration used in :meth:`~pyrosex.Client.search_messages` and :meth:`~pyrosex.Client.search_global`"""
+    """Messages filter enumeration used in :meth:`~pyroherd.Client.search_messages` and :meth:`~pyroherd.Client.search_global`"""
 
     EMPTY = raw.types.InputMessagesFilterEmpty
     "Empty filter (any kind of messages)"
 
     PHOTO = raw.types.InputMessagesFilterPhotos
     "Photo messages"
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/next_code_type.py` & `pyroherd-0.0.1/pyroherd/enums/sent_code_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
-class NextCodeType(AutoName):
-    """Next code type enumeration used in :obj:`~pyrosex.types.SentCode`."""
+class SentCodeType(AutoName):
+    """Sent code type enumeration used in :obj:`~pyroherd.types.SentCode`."""
 
-    CALL = raw.types.auth.CodeTypeCall
+    APP = raw.types.auth.SentCodeTypeApp
+    "The code was sent through the telegram app."
+
+    CALL = raw.types.auth.SentCodeTypeCall
     "The code will be sent via a phone call. A synthesized voice will tell the user which verification code to input."
 
-    FLASH_CALL = raw.types.auth.CodeTypeFlashCall
+    FLASH_CALL = raw.types.auth.SentCodeTypeFlashCall
     "The code will be sent via a flash phone call, that will be closed immediately."
 
-    MISSED_CALL = raw.types.auth.CodeTypeMissedCall
+    MISSED_CALL = raw.types.auth.SentCodeTypeMissedCall
     "Missed call."
 
-    SMS = raw.types.auth.CodeTypeSms
+    SMS = raw.types.auth.SentCodeTypeSms
     "The code was sent via SMS."
```

### Comparing `pyroherd-0.0.0/pyroherd/enums/sent_code_type.py` & `pyroherd-0.0.1/pyroherd/enums/next_code_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from pyrosex import raw
+from pyroherd import raw
 from .auto_name import AutoName
 
 
-class SentCodeType(AutoName):
-    """Sent code type enumeration used in :obj:`~pyrosex.types.SentCode`."""
+class NextCodeType(AutoName):
+    """Next code type enumeration used in :obj:`~pyroherd.types.SentCode`."""
 
-    APP = raw.types.auth.SentCodeTypeApp
-    "The code was sent through the telegram app."
-
-    CALL = raw.types.auth.SentCodeTypeCall
+    CALL = raw.types.auth.CodeTypeCall
     "The code will be sent via a phone call. A synthesized voice will tell the user which verification code to input."
 
-    FLASH_CALL = raw.types.auth.SentCodeTypeFlashCall
+    FLASH_CALL = raw.types.auth.CodeTypeFlashCall
     "The code will be sent via a flash phone call, that will be closed immediately."
 
-    MISSED_CALL = raw.types.auth.SentCodeTypeMissedCall
+    MISSED_CALL = raw.types.auth.CodeTypeMissedCall
     "Missed call."
 
-    SMS = raw.types.auth.SentCodeTypeSms
+    SMS = raw.types.auth.CodeTypeSms
     "The code was sent via SMS."
```

### Comparing `pyroherd-0.0.0/pyroherd/errors/__init__.py` & `pyroherd-0.0.1/pyroherd/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/errors/rpc_error.py` & `pyroherd-0.0.1/pyroherd/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/file_id.py` & `pyroherd-0.0.1/pyroherd/file_id.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/filters.py` & `pyroherd-0.0.1/pyroherd/filters.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/__init__.py` & `pyroherd-0.0.1/pyroherd/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/callback_query_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/chat_join_request_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/chat_member_updated_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/chosen_inline_result_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/deleted_messages_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/disconnect_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/edited_message_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/handler.py` & `pyroherd-0.0.1/pyroherd/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/inline_query_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/message_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/poll_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/raw_update_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/handlers/user_status_handler.py` & `pyroherd-0.0.1/pyroherd/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/advanced/invoke.py` & `pyroherd-0.0.1/pyroherd/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/advanced/resolve_peer.py` & `pyroherd-0.0.1/pyroherd/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/advanced/save_file.py` & `pyroherd-0.0.1/pyroherd/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/accept_terms_of_service.py` & `pyroherd-0.0.1/pyroherd/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/check_password.py` & `pyroherd-0.0.1/pyroherd/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/connect.py` & `pyroherd-0.0.1/pyroherd/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/disconnect.py` & `pyroherd-0.0.1/pyroherd/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/initialize.py` & `pyroherd-0.0.1/pyroherd/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/log_out.py` & `pyroherd-0.0.1/pyroherd/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/recover_password.py` & `pyroherd-0.0.1/pyroherd/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/resend_code.py` & `pyroherd-0.0.1/pyroherd/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/send_code.py` & `pyroherd-0.0.1/pyroherd/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/send_recovery_code.py` & `pyroherd-0.0.1/pyroherd/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/sign_in.py` & `pyroherd-0.0.1/pyroherd/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/sign_in_bot.py` & `pyroherd-0.0.1/pyroherd/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/sign_up.py` & `pyroherd-0.0.1/pyroherd/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/auth/terminate.py` & `pyroherd-0.0.1/pyroherd/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/answer_callback_query.py` & `pyroherd-0.0.1/pyroherd/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/answer_inline_query.py` & `pyroherd-0.0.1/pyroherd/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/answer_web_app_query.py` & `pyroherd-0.0.1/pyroherd/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/delete_bot_commands.py` & `pyroherd-0.0.1/pyroherd/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/get_bot_commands.py` & `pyroherd-0.0.1/pyroherd/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/get_bot_default_privileges.py` & `pyroherd-0.0.1/pyroherd/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/get_chat_menu_button.py` & `pyroherd-0.0.1/pyroherd/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/get_game_high_scores.py` & `pyroherd-0.0.1/pyroherd/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/get_inline_bot_results.py` & `pyroherd-0.0.1/pyroherd/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/request_callback_answer.py` & `pyroherd-0.0.1/pyroherd/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/send_game.py` & `pyroherd-0.0.1/pyroherd/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/send_inline_bot_result.py` & `pyroherd-0.0.1/pyroherd/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/set_bot_commands.py` & `pyroherd-0.0.1/pyroherd/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/set_bot_default_privileges.py` & `pyroherd-0.0.1/pyroherd/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/set_chat_menu_button.py` & `pyroherd-0.0.1/pyroherd/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/bots/set_game_score.py` & `pyroherd-0.0.1/pyroherd/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/add_chat_members.py` & `pyroherd-0.0.1/pyroherd/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/archive_chats.py` & `pyroherd-0.0.1/pyroherd/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/ban_chat_member.py` & `pyroherd-0.0.1/pyroherd/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/create_channel.py` & `pyroherd-0.0.1/pyroherd/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/create_group.py` & `pyroherd-0.0.1/pyroherd/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/create_supergroup.py` & `pyroherd-0.0.1/pyroherd/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/delete_channel.py` & `pyroherd-0.0.1/pyroherd/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/delete_chat_photo.py` & `pyroherd-0.0.1/pyroherd/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/delete_supergroup.py` & `pyroherd-0.0.1/pyroherd/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/delete_user_history.py` & `pyroherd-0.0.1/pyroherd/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat_event_log.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat_member.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat_members.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat_members_count.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_chat_online_count.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_dialogs.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_dialogs_count.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_nearby_chats.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/get_send_as_chats.py` & `pyroherd-0.0.1/pyroherd/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/join_chat.py` & `pyroherd-0.0.1/pyroherd/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/leave_chat.py` & `pyroherd-0.0.1/pyroherd/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/mark_chat_unread.py` & `pyroherd-0.0.1/pyroherd/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/pin_chat_message.py` & `pyroherd-0.0.1/pyroherd/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/promote_chat_member.py` & `pyroherd-0.0.1/pyroherd/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/restrict_chat_member.py` & `pyroherd-0.0.1/pyroherd/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_administrator_title.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_description.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_permissions.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_photo.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_protected_content.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_title.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_chat_username.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_send_as_chat.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/set_slow_mode.py` & `pyroherd-0.0.1/pyroherd/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/unarchive_chats.py` & `pyroherd-0.0.1/pyroherd/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/unban_chat_member.py` & `pyroherd-0.0.1/pyroherd/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/unpin_all_chat_messages.py` & `pyroherd-0.0.1/pyroherd/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/chats/unpin_chat_message.py` & `pyroherd-0.0.1/pyroherd/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/contacts/add_contact.py` & `pyroherd-0.0.1/pyroherd/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/contacts/delete_contacts.py` & `pyroherd-0.0.1/pyroherd/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/contacts/get_contacts.py` & `pyroherd-0.0.1/pyroherd/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/contacts/get_contacts_count.py` & `pyroherd-0.0.1/pyroherd/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/contacts/import_contacts.py` & `pyroherd-0.0.1/pyroherd/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_cb.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_cb.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_chat_join_request.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_chat_member_updated.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_chosen_inline_result.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_deleted_messages.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_disconnect.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_edited_message.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_inline_query.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_msg.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_msg.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_poll.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_raw_update.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/decorators/on_user_status.py` & `pyroherd-0.0.1/pyroherd/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/approve_all_chat_join_requests.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/approve_chat_join_request.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/create_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/decline_all_chat_join_requests.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/decline_chat_join_request.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/delete_chat_admin_invite_links.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/delete_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/edit_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/export_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admin_invite_links.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Union
 
-import pyrosex
-from pyrosex import raw
+import pyroherd
+from pyroherd import raw
 
 
 class GetChatAdminInviteLinksCount:
     async def get_chat_admin_invite_links_count(
-        self: "pyrosex.Client",
+        self: "pyroherd.Client",
         chat_id: Union[int, str],
         admin_id: Union[int, str],
         revoked: bool = False,
     ) -> int:
         """Get the count of the invite links created by an administrator in a chat.
 
         Parameters:
```

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link_joiners.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/get_chat_join_requests.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/invite_links/revoke_chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/copy_media_group.py` & `pyroherd-0.0.1/pyroherd/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/copy_message.py` & `pyroherd-0.0.1/pyroherd/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/delete_messages.py` & `pyroherd-0.0.1/pyroherd/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/download_media.py` & `pyroherd-0.0.1/pyroherd/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_caption.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_media.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_reply_markup.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_inline_text.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_message_caption.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_message_media.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_message_reply_markup.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/edit_message_text.py` & `pyroherd-0.0.1/pyroherd/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/forward_messages.py` & `pyroherd-0.0.1/pyroherd/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_chat_history.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_chat_history_count.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_chat_history_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         chat_id: Union[int, str]
     ) -> int:
         """Get the total count of messages in a chat.
 
         .. note::
 
             Due to Telegram latest internal changes, the server can't reliably find anymore the total count of messages
-            a **private** or a **basic group** chat has with a single method call. To overcome this limitation, Pyrogram
+            a **private** or a **basic group** chat has with a single method call. To overcome this limitation, Pyroherd
             has to iterate over all the messages. Channels and supergroups are not affected by this limitation.
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
         Returns:
```

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_message.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_replies.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_discussion_replies_count.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_media_group.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/get_messages.py` & `pyroherd-0.0.1/pyroherd/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/inline_session.py` & `pyroherd-0.0.1/pyroherd/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/read_chat_history.py` & `pyroherd-0.0.1/pyroherd/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/retract_vote.py` & `pyroherd-0.0.1/pyroherd/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/search_global.py` & `pyroherd-0.0.1/pyroherd/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/search_global_count.py` & `pyroherd-0.0.1/pyroherd/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/search_messages.py` & `pyroherd-0.0.1/pyroherd/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/search_messages_count.py` & `pyroherd-0.0.1/pyroherd/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_animation.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_audio.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_cached_media.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_chat_action.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_contact.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_dice.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_document.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_location.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_media_group.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_message.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         Returns:
             :obj:`~pyroherd.types.Message`: On success, the sent text message is returned.
 
         Example:
             .. code-block:: python
 
                 # Simple example
-                await app.send_message("me", "Message sent with **Pyrogram**!")
+                await app.send_message("me", "Message sent with **Pyroherd**!")
 
                 # Disable web page previews
                 await app.send_message("me", "https://docs.pyroherd.org",
                     disable_web_page_preview=True)
 
                 # Reply to a message using its id
                 await app.send_message("me", "this is a reply", reply_to_message_id=123)
```

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_photo.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_poll.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_reaction.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_sticker.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_venue.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_video.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_video_note.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/send_voice.py` & `pyroherd-0.0.1/pyroherd/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/stop_poll.py` & `pyroherd-0.0.1/pyroherd/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/stream_media.py` & `pyroherd-0.0.1/pyroherd/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/messages/vote_poll.py` & `pyroherd-0.0.1/pyroherd/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/password/change_cloud_password.py` & `pyroherd-0.0.1/pyroherd/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/password/enable_cloud_password.py` & `pyroherd-0.0.1/pyroherd/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/password/remove_cloud_password.py` & `pyroherd-0.0.1/pyroherd/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/__init__.py` & `pyroherd-0.0.1/pyroherd/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/block_user.py` & `pyroherd-0.0.1/pyroherd/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/delete_profile_photos.py` & `pyroherd-0.0.1/pyroherd/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/get_chat_photos.py` & `pyroherd-0.0.1/pyroherd/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/get_chat_photos_count.py` & `pyroherd-0.0.1/pyroherd/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/get_common_chats.py` & `pyroherd-0.0.1/pyroherd/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/get_me.py` & `pyroherd-0.0.1/pyroherd/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/get_users.py` & `pyroherd-0.0.1/pyroherd/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/set_profile_photo.py` & `pyroherd-0.0.1/pyroherd/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/set_username.py` & `pyroherd-0.0.1/pyroherd/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/unblock_user.py` & `pyroherd-0.0.1/pyroherd/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/users/update_profile.py` & `pyroherd-0.0.1/pyroherd/methods/users/update_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         Returns:
             ``bool``: True on success.
 
         Example:
             .. code-block:: python
 
                 # Update your first name only
-                await app.update_profile(first_name="Pyrogram")
+                await app.update_profile(first_name="Pyroherd")
 
                 # Update first name and bio
-                await app.update_profile(first_name="Pyrogram", bio="https://docs.pyroherd.org/")
+                await app.update_profile(first_name="Pyroherd", bio="https://docs.pyroherd.org/")
 
                 # Remove the last name
                 await app.update_profile(last_name="")
         """
 
         return bool(
             await self.invoke(
```

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/add_handler.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/compose.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/export_session_string.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/idle.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/remove_handler.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/restart.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/run.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         """Start the client, idle the main script and finally stop the client.
 
         When calling this method without any argument it acts as a convenience method that calls
         :meth:`~pyroherd.Client.start`, :meth:`~pyroherd.idle` and :meth:`~pyroherd.Client.stop` in sequence.
         It makes running a single client less verbose.
 
         In case a coroutine is passed as argument, runs the coroutine until it's completed and doesn't do any client
-        operation. This is almost the same as :py:obj:`asyncio.run` except for the fact that Pyrogram's ``run`` uses the
+        operation. This is almost the same as :py:obj:`asyncio.run` except for the fact that Pyroherd's ``run`` uses the
         current event loop instead of a new one.
 
         If you want to run multiple clients at once, see :meth:`pyroherd.compose`.
 
         Parameters:
             coroutine (``Coroutine``, *optional*):
                 Pass a coroutine to run it until it completes.
```

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/start.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/stop.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/methods/utilities/stop_transmission.py` & `pyroherd-0.0.1/pyroherd/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/mime_types.py` & `pyroherd-0.0.1/pyroherd/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/parser/html.py` & `pyroherd-0.0.1/pyroherd/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/parser/markdown.py` & `pyroherd-0.0.1/pyroherd/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/parser/parser.py` & `pyroherd-0.0.1/pyroherd/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/parser/utils.py` & `pyroherd-0.0.1/pyroherd/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/future_salt.py` & `pyroherd-0.0.1/pyroherd/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/future_salts.py` & `pyroherd-0.0.1/pyroherd/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/gzip_packed.py` & `pyroherd-0.0.1/pyroherd/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/message.py` & `pyroherd-0.0.1/pyroherd/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/msg_container.py` & `pyroherd-0.0.1/pyroherd/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/primitives/bool.py` & `pyroherd-0.0.1/pyroherd/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/primitives/bytes.py` & `pyroherd-0.0.1/pyroherd/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/primitives/int.py` & `pyroherd-0.0.1/pyroherd/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/primitives/vector.py` & `pyroherd-0.0.1/pyroherd/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/raw/core/tl_object.py` & `pyroherd-0.0.1/pyroherd/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/session/auth.py` & `pyroherd-0.0.1/pyroherd/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/session/internals/data_center.py` & `pyroherd-0.0.1/pyroherd/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/session/internals/msg_factory.py` & `pyroherd-0.0.1/pyroherd/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/session/internals/msg_id.py` & `pyroherd-0.0.1/pyroherd/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/session/session.py` & `pyroherd-0.0.1/pyroherd/session/session.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/storage/file_storage.py` & `pyroherd-0.0.1/pyroherd/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/storage/memory_storage.py` & `pyroherd-0.0.1/pyroherd/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/storage/sqlite_storage.py` & `pyroherd-0.0.1/pyroherd/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/storage/storage.py` & `pyroherd-0.0.1/pyroherd/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/sync.py` & `pyroherd-0.0.1/pyroherd/sync.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/authorization/sent_code.py` & `pyroherd-0.0.1/pyroherd/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/authorization/terms_of_service.py` & `pyroherd-0.0.1/pyroherd/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/__init__.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/callback_query.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/force_reply.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/game_high_score.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/inline_keyboard_button.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/keyboard_button.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/login_url.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/menu_button_web_app.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/bots_and_keyboards/sent_web_app_message.py` & `pyroherd-0.0.1/pyroherd/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/__init__.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/chosen_inline_result.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_animation.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_article.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_audio.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_animation.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_audio.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_document.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_photo.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_sticker.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_video.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_cached_voice.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_contact.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_document.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_location.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_photo.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_venue.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_video.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/inline_mode/inline_query_result_voice.py` & `pyroherd-0.0.1/pyroherd/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media_animation.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media_audio.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media_document.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media_photo.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_media_video.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_media/input_phone_contact.py` & `pyroherd-0.0.1/pyroherd/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_message_content/input_message_content.py` & `pyroherd-0.0.1/pyroherd/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/input_message_content/input_text_message_content.py` & `pyroherd-0.0.1/pyroherd/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/__init__.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/animation.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/audio.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/contact.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/dice.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/document.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/game.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/location.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/message.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/message_entity.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/photo.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/poll.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/poll_option.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/reaction.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/sticker.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/stripped_thumbnail.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/thumbnail.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/venue.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/video.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/video_note.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/voice.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/web_app_data.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/messages_and_media/web_page.py` & `pyroherd-0.0.1/pyroherd/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/object.py` & `pyroherd-0.0.1/pyroherd/types/object.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 class Object:
     def __init__(self, client: "pyroherd.Client" = None):
         self._client = client
 
     def bind(self, client: "pyroherd.Client"):
-        """Bind a Client instance to this and to all nested Pyrosex objects.
+        """Bind a Client instance to this and to all nested Pyroherd objects.
 
         Parameters:
             client (:obj:`~pyroherd.types.Client`):
                 The Client instance to bind this object with. Useful to re-enable bound methods after serializing and
-                deserializing Pyrosex objects with ``repr`` and ``eval``.
+                deserializing Pyroherd objects with ``repr`` and ``eval``.
         """
         self._client = client
 
         for i in self.__dict__:
             o = getattr(self, i)
 
             if isinstance(o, Object):
```

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/__init__.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_admin_with_invite_links.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_event.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_event_filter.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_invite_link.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_join_request.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_joiner.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_member.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_member_updated.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_permissions.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_photo.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_preview.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/chat_privileges.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/dialog.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/invite_link_importer.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/restriction.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/user.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_ended.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_members_invited.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/types/user_and_chats/video_chat_scheduled.py` & `pyroherd-0.0.1/pyroherd/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd/utils.py` & `pyroherd-0.0.1/pyroherd/utils.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/pyroherd.egg-info/PKG-INFO` & `pyroherd-0.0.1/pyroherd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroherd
-Version: 0.0.0
+Version: 0.0.1
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/OnTheHerd
 Download-URL: https://github.com/OnTheHerd/pyroherd/releases/latest
 Author: OnTheHerd
 Author-email: ontheherd@onmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/OnTheHerd/pyroherd/issues
```

### Comparing `pyroherd-0.0.0/pyroherd.egg-info/SOURCES.txt` & `pyroherd-0.0.1/pyroherd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/setup.py` & `pyroherd-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/tests/filters/test_command.py` & `pyroherd-0.0.1/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `pyroherd-0.0.0/tests/test_file_id.py` & `pyroherd-0.0.1/tests/test_file_id.py`

 * *Files identical despite different names*

