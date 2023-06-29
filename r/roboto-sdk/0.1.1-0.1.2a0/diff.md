# Comparing `tmp/roboto_sdk-0.1.1.tar.gz` & `tmp/roboto_sdk-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.1.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.2a0.tar", max compression
```

## Comparing `roboto_sdk-0.1.1.tar` & `roboto_sdk-0.1.2a0.tar`

### file list

```diff
@@ -1,90 +1,121 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.1/README.md
--rw-r--r--   0        0        0      806 2023-06-27 16:56:42.083372 roboto_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.1/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.1/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     3892 2023-06-25 17:00:28.230327 roboto_sdk-0.1.1/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.1/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.1/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      788 2023-06-24 00:11:31.029362 roboto_sdk-0.1.1/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6690 2023-06-21 21:21:55.948875 roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3236 2023-06-25 17:23:12.369105 roboto_sdk-0.1.1/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.1/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.1/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3165 2023-06-24 00:34:28.168958 roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.1/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.1/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0        0 2023-06-01 19:18:26.922915 roboto_sdk-0.1.1/src/roboto_sdk/delegate/__init__.py
--rw-r--r--   0        0        0      621 2023-06-13 17:13:48.413704 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/__init__.py
--rw-r--r--   0        0        0     4981 2023-06-15 18:41:26.811336 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_delegate.py
--rw-r--r--   0        0        0      651 2023-06-15 18:41:26.811435 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_resources.py
--rw-r--r--   0        0        0     3463 2023-06-22 00:30:04.537634 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      448 2023-06-15 18:41:26.811604 roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_resources.py
--rw-r--r--   0        0        0      166 2023-06-13 17:13:48.414122 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/__init__.py
--rw-r--r--   0        0        0     4750 2023-06-14 17:40:40.588738 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_delegate.py
--rw-r--r--   0        0        0      363 2023-06-13 17:13:48.414231 roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_resources.py
--rw-r--r--   0        0        0      297 2023-06-13 17:13:48.414296 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/__init__.py
--rw-r--r--   0        0        0     2113 2023-06-14 17:40:40.588896 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-06-13 17:13:48.414393 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_resources.py
--rw-r--r--   0        0        0     2323 2023-06-14 17:40:40.589039 roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/s3_delegate.py
--rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.1/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0      520 2023-06-23 23:37:43.832600 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0      893 2023-06-24 00:19:03.182623 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     2243 2023-06-24 00:19:03.180345 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      177 2023-06-23 23:37:43.833111 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     1485 2023-06-24 00:19:03.185556 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1147 2023-06-23 23:37:43.833392 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      545 2023-06-23 23:37:43.833519 roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2685 2023-06-21 18:17:36.116508 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      623 2023-06-25 17:14:17.623374 roboto_sdk-0.1.1/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.1/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.1/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3032 2023-06-25 17:23:12.393083 roboto_sdk-0.1.1/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.1/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.416919 roboto_sdk-0.1.1/src/roboto_sdk/model/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-15 18:41:26.811706 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/__init__.py
--rw-r--r--   0        0        0     7019 2023-06-15 18:41:26.811800 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action.py
--rw-r--r--   0        0        0     2804 2023-06-15 18:41:26.811886 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_delegate.py
--rw-r--r--   0        0        0      792 2023-06-15 18:41:26.811996 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-06-13 17:13:48.416658 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/error.py
--rw-r--r--   0        0        0     2247 2023-06-21 18:21:45.309132 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation.py
--rw-r--r--   0        0        0     1413 2023-06-21 18:24:02.339440 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_delegate.py
--rw-r--r--   0        0        0     1464 2023-06-15 18:41:26.812185 roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_record.py
--rw-r--r--   0        0        0      395 2023-06-13 17:13:48.417131 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/__init__.py
--rw-r--r--   0        0        0     9580 2023-06-14 17:40:40.589162 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/dataset.py
--rw-r--r--   0        0        0     2132 2023-06-14 17:40:40.589271 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/delegate.py
--rw-r--r--   0        0        0      817 2023-06-13 17:13:48.417299 roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/record.py
--rw-r--r--   0        0        0      178 2023-06-14 17:40:40.589416 roboto_sdk-0.1.1/src/roboto_sdk/model/files/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-14 17:40:40.589560 roboto_sdk-0.1.1/src/roboto_sdk/model/files/delegate.py
--rw-r--r--   0        0        0      771 2023-06-14 17:40:40.589669 roboto_sdk-0.1.1/src/roboto_sdk/model/files/file.py
--rw-r--r--   0        0        0      385 2023-06-14 17:40:40.589805 roboto_sdk-0.1.1/src/roboto_sdk/model/files/record.py
--rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.1/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.1/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-25 17:05:30.425831 roboto_sdk-0.1.1/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.1/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.1/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.1/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 roboto_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/README.md
+-rw-r--r--   0        0        0      808 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-29 22:47:06.770668 roboto_sdk-0.1.2a0/src/roboto_sdk/auth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3596 2023-06-29 22:47:06.770668 roboto_sdk-0.1.2a0/src/roboto_sdk/auth/__pycache__/pat.cpython-310.pyc
+-rw-r--r--   0        0        0     3892 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/auth/pat.py
+-rw-r--r--   0        0        0      132 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/args.py
+-rw-r--r--   0        0        0     2033 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/model.py
+-rw-r--r--   0        0        0      790 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/context.py
+-rw-r--r--   0        0        0      110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     6691 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/datasets/commands.py
+-rw-r--r--   0        0        0     3223 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/entry.py
+-rw-r--r--   0        0        0      108 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/help/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/help/args.py
+-rw-r--r--   0        0        0      110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/orgs/__init__.py
+-rw-r--r--   0        0        0     3386 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/orgs/commands.py
+-rw-r--r--   0        0        0      110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/tokens/__init__.py
+-rw-r--r--   0        0        0     3301 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/tokens/commands.py
+-rw-r--r--   0        0        0      110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/triggers/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/triggers/commands.py
+-rw-r--r--   0        0        0      110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/users/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/cli/users/commands.py
+-rw-r--r--   0        0        0       48 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-29 22:47:06.398667 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1633 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__init__.py
+-rw-r--r--   0        0        0     1364 2023-06-29 22:47:06.402668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6124 2023-06-29 22:47:06.402668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/action.cpython-310.pyc
+-rw-r--r--   0        0        0     3512 2023-06-29 22:47:06.402668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/action_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     5066 2023-06-29 22:47:06.414667 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/action_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1246 2023-06-29 22:47:06.806668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/action_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      964 2023-06-29 22:47:06.402668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/action_record.cpython-310.pyc
+-rw-r--r--   0        0        0      494 2023-06-29 22:47:06.406668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/error.cpython-310.pyc
+-rw-r--r--   0        0        0     4527 2023-06-29 22:47:06.406668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/invocation.cpython-310.pyc
+-rw-r--r--   0        0        0     2155 2023-06-29 22:47:06.410668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/invocation_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4383 2023-06-29 22:47:06.810668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/invocation_http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1121 2023-06-29 22:47:06.810668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/invocation_http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     2179 2023-06-29 22:47:06.410668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__pycache__/invocation_record.cpython-310.pyc
+-rw-r--r--   0        0        0     7019 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action.py
+-rw-r--r--   0        0        0     2804 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_delegate.py
+-rw-r--r--   0        0        0     5167 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_delegate.py
+-rw-r--r--   0        0        0      651 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_resources.py
+-rw-r--r--   0        0        0      792 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_record.py
+-rw-r--r--   0        0        0      106 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/error.py
+-rw-r--r--   0        0        0     4294 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation.py
+-rw-r--r--   0        0        0     1653 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_delegate.py
+-rw-r--r--   0        0        0     4684 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_http_delegate.py
+-rw-r--r--   0        0        0      534 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_http_resources.py
+-rw-r--r--   0        0        0     1592 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_record.py
+-rw-r--r--   0        0        0      546 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      593 2023-06-29 22:47:06.826668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7138 2023-06-29 22:47:06.826668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     3000 2023-06-29 22:47:06.834668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     4911 2023-06-29 22:47:06.838668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      725 2023-06-29 22:47:06.838668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0     1116 2023-06-29 22:47:06.834668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     9572 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/dataset.py
+-rw-r--r--   0        0        0     2132 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/delegate.py
+-rw-r--r--   0        0        0     4759 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/http_delegate.py
+-rw-r--r--   0        0        0      340 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/http_resources.py
+-rw-r--r--   0        0        0      817 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/record.py
+-rw-r--r--   0        0        0      436 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__init__.py
+-rw-r--r--   0        0        0      570 2023-06-29 22:47:06.830669 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1736 2023-06-29 22:47:06.830669 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1350 2023-06-29 22:47:06.830669 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/file.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-06-29 22:47:06.834668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/http_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0      581 2023-06-29 22:47:06.834668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/http_resources.cpython-310.pyc
+-rw-r--r--   0        0        0      557 2023-06-29 22:47:06.830669 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0        0        0     3066 2023-06-29 22:47:06.834668 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/__pycache__/s3_delegate.cpython-310.pyc
+-rw-r--r--   0        0        0     1156 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/delegate.py
+-rw-r--r--   0        0        0      771 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/file.py
+-rw-r--r--   0        0        0     2110 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/http_delegate.py
+-rw-r--r--   0        0        0      168 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/http_resources.py
+-rw-r--r--   0        0        0      385 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/record.py
+-rw-r--r--   0        0        0     2320 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/s3_delegate.py
+-rw-r--r--   0        0        0      633 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/delegate.py
+-rw-r--r--   0        0        0     3610 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/http_delegate.py
+-rw-r--r--   0        0        0      359 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/http_resources.py
+-rw-r--r--   0        0        0     2381 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/org.py
+-rw-r--r--   0        0        0     1145 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/org_role.py
+-rw-r--r--   0        0        0      563 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/record.py
+-rw-r--r--   0        0        0      387 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/delegate.py
+-rw-r--r--   0        0        0     1968 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/http_delegate.py
+-rw-r--r--   0        0        0      184 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/http_resources.py
+-rw-r--r--   0        0        0      412 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/record.py
+-rw-r--r--   0        0        0     1807 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/token.py
+-rw-r--r--   0        0        0      391 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/http_delegate.py
+-rw-r--r--   0        0        0      205 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/http_resources.py
+-rw-r--r--   0        0        0     2661 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger.py
+-rw-r--r--   0        0        0      857 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger_delegate.py
+-rw-r--r--   0        0        0      249 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger_record.py
+-rw-r--r--   0        0        0      262 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/__init__.py
+-rw-r--r--   0        0        0     1016 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/http_delegate.py
+-rw-r--r--   0        0        0     1200 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/user.py
+-rw-r--r--   0        0        0      451 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/user_delegate.py
+-rw-r--r--   0        0        0      162 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/user_record.py
+-rw-r--r--   0        0        0      704 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__init__.py
+-rw-r--r--   0        0        0      699 2023-06-29 22:47:06.414667 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      358 2023-06-29 22:47:06.414667 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     9423 2023-06-29 22:47:06.418668 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__pycache__/http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     3698 2023-06-29 22:47:06.458668 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__pycache__/request_decorators.cpython-310.pyc
+-rw-r--r--   0        0        0     1512 2023-06-29 22:47:06.806668 roboto_sdk-0.1.2a0/src/roboto_sdk/http/__pycache__/testing_util.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/http/constants.py
+-rw-r--r--   0        0        0     8880 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/http/http_client.py
+-rw-r--r--   0        0        0     3032 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/http/request_decorators.py
+-rw-r--r--   0        0        0      994 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/http/testing_util.py
+-rw-r--r--   0        0        0      158 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/logging.py
+-rw-r--r--   0        0        0      211 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/pagination.py
+-rw-r--r--   0        0        0      168 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/profile/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-29 22:47:06.802668 roboto_sdk-0.1.2a0/src/roboto_sdk/profile/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2590 2023-06-29 22:47:06.802668 roboto_sdk-0.1.2a0/src/roboto_sdk/profile/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     2809 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/py.typed
+-rw-r--r--   0        0        0      651 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/serde.py
+-rw-r--r--   0        0        0      112 2023-06-29 22:42:46.000000 roboto_sdk-0.1.2a0/src/roboto_sdk/time.py
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 roboto_sdk-0.1.2a0/PKG-INFO
```

### Comparing `roboto_sdk-0.1.1/pyproject.toml` & `roboto_sdk-0.1.2a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.1"
+version = "0.1.2a0"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
+from ..domain.actions import ActionDelegate
+from ..domain.datasets import DatasetDelegate
 from ..domain.orgs import OrgDelegate
 from ..domain.tokens import TokenDelegate
 from ..domain.triggers import TriggerDelegate
 from ..http import HttpClient
-from ..model.actions import ActionDelegate
-from ..model.datasets import DatasetDelegate
 
 
 class CLIContext:
     _http: HttpClient | None
     datasets: DatasetDelegate
     orgs: OrgDelegate
     tokens: TokenDelegate
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/datasets/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 import argparse
 import json
 import pathlib
 import sys
 
-from ...model.datasets import Dataset
+from ...domain.datasets import Dataset
 from ..command import (
     ExistingPathlibPath,
     KeyValuePairsAction,
     RobotoCommand,
     RobotoCommandSet,
 )
 from ..context import CLIContext
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import argparse
 import logging
 import sys
 from typing import Any
 
-from ..delegate.actions import ActionHttpDelegate
-from ..delegate.datasets import (
-    DatasetHttpDelegate,
-)
+from ..domain.actions import ActionHttpDelegate
+from ..domain.datasets import DatasetHttpDelegate
 from ..domain.orgs import OrgHttpDelegate
 from ..domain.tokens import TokenHttpDelegate
 from ..domain.triggers import TriggerHttpDelegate
 from ..http import (
     HttpClient,
     LocalAuthDecorator,
     PATAuthDecorator,
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/orgs/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 def create(args, context: CLIContext, parser: argparse.ArgumentParser):
     record = Org.create(
         creator_user_id=None,
         name=args.name,
         org_type=args.type,
         org_delegate=context.orgs,
+        bind_email_domain=args.bind_email_domain,
     )
     sys.stdout.write(json.dumps(record.to_dict()) + "\n")
 
 
 def create_setup_parser(parser):
     parser.add_argument(
         "--name", type=str, required=True, help="A human readable name for this org"
@@ -29,14 +30,20 @@
     parser.add_argument(
         "--type",
         type=str,
         choices=OrgType._member_names_,
         help="The type of org you're creating",
     )
 
+    parser.add_argument(
+        "--bind-email-domain",
+        action="store_true",
+        help="Automatically add new users with your email domain to this org",
+    )
+
 
 def delete(args, context: CLIContext, parser: argparse.ArgumentParser):
     Org.by_org_id(org_id=args.org, org_delegate=context.orgs).delete()
     sys.stdout.write("Successfully deleted!\n")
 
 
 def delete_setup_parser(parser):
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import http
 import json
 from typing import Any
 
 from ...http import ClientError, HttpClient
 from ...logging import default_logger
-from ...model.actions import (
+from ...pagination import PaginatedList
+from ...serde import pydantic_jsonable_dict
+from .action_delegate import (
     ActionDelegate,
-    ActionRecord,
-    ActionUpdateConditionCheckFailure,
     ContainerCredentials,
     UpdateCondition,
 )
-from ...pagination import PaginatedList
-from ...serde import pydantic_jsonable_dict
 from .action_http_resources import (
     CreateActionRequest,
     UpdateActionRequest,
 )
+from .action_record import ActionRecord
+from .error import (
+    ActionUpdateConditionCheckFailure,
+)
 
 logger = default_logger()
 
 
 class ActionHttpDelegate(ActionDelegate):
     """
     Use in any context that does not have direct database access.
@@ -52,26 +54,29 @@
             description=description,
             metadata=metadata,
             tags=tags,
         )
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
-            headers={"Content-Type": "application/json"},
+            headers={"Content-Type": "application/json", "X-Roboto-Org-Id": tenant_id},
         )
         return ActionRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def get_action_by_primary_key(
         self, name: str, tenant_id: str | None = None
     ) -> ActionRecord:
         """
         `tenant_id` is ignored, as it is determined server-side by the identity of the caller.
         """
         url = f"{self.__roboto_service_base_url}/v1/actions/{name}"
-        res = self.__http_client.get(url)
+        headers = {}
+        if tenant_id:
+            headers["X-Roboto-Org-Id"] = tenant_id
+        res = self.__http_client.get(url, headers=headers)
         return ActionRecord.parse_obj(res.from_json(json_path=["data"]))
 
     def register_container(
         self,
         record: ActionRecord,
         image_name: str,
         image_tag: str,
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/action_http_resources.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 import pydantic
 
-from ...model.actions import UpdateCondition
+from .action_delegate import UpdateCondition
 
 
 class CreateActionRequest(pydantic.BaseModel):
     # Required
     name: str
 
     # Optional
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import json
 from typing import Any
 
 from ...http import HttpClient
 from ...logging import default_logger
-from ...model.actions import (
-    InvocationDataSourceType,
-    InvocationDelegate,
-    InvocationRecord,
-    InvocationSource,
-    InvocationStatus,
-)
 from ...pagination import PaginatedList
 from ...serde import pydantic_jsonable_dict
+from .invocation_delegate import (
+    InvocationDelegate,
+)
 from .invocation_http_resources import (
     CreateInvocationRequest,
+    SetLogsLocationRequest,
+)
+from .invocation_record import (
+    InvocationDataSourceType,
+    InvocationRecord,
+    InvocationSource,
+    InvocationStatus,
 )
 
 logger = default_logger()
 
 
 class InvocationHttpDelegate(InvocationDelegate):
     """
@@ -49,36 +52,67 @@
         request_body = CreateInvocationRequest(
             input_data=input_data,
             data_source_id=data_source_id,
             data_source_type=data_source_type,
             invocation_source=invocation_source,
             invocation_source_id=invocation_source_id,
         )
+        headers = {"Content-Type": "application/json"}
+        if tenant_id:
+            headers["X-Roboto-Org-Id"] = tenant_id
         response = self.__http_client.post(
             url,
             data=pydantic_jsonable_dict(request_body, exclude_none=True),
-            headers={"Content-Type": "application/json"},
+            headers=headers,
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def get_by_id(self, invocation_id: str) -> InvocationRecord:
-        """Get an Invocation by ID"""
-        raise NotImplementedError("get_by_id")
+    def get_by_id(
+        self, invocation_id: str, org_id: str | None = None
+    ) -> InvocationRecord:
+        url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{invocation_id}"
+        headers = {}
+        if org_id:
+            headers["X-Roboto-Org-Id"] = org_id
+        response = self.__http_client.get(url, headers=headers)
+        return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
+
+    def set_logs_location(
+        self, record: InvocationRecord, bucket: str, prefix: str
+    ) -> InvocationRecord:
+        url = (
+            f"{self.__roboto_service_base_url}/v1/actions/invocations/{record.id}/logs"
+        )
+        headers = {
+            "Content-Type": "application/json",
+            "X-Roboto-Org-Id": record.tenant_id,
+        }
+        request_body = SetLogsLocationRequest(bucket=bucket, prefix=prefix)
+        response = self.__http_client.patch(
+            url,
+            data=pydantic_jsonable_dict(request_body, exclude_none=True),
+            headers=headers,
+        )
+        return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def update_invocation_status(
         self,
         invocation: InvocationRecord,
         status: InvocationStatus,
         detail: str | None = None,
     ) -> InvocationRecord:
-        url = f"{self.__roboto_service_base_url}/v1/actions/{invocation.action_name}/invoke/{invocation.id}/status"
+        url = f"{self.__roboto_service_base_url}/v1/actions/invocations/{invocation.id}/status"
+        headers = {
+            "Content-Type": "application/json",
+            "X-Roboto-Org-Id": invocation.tenant_id,
+        }
         response = self.__http_client.post(
             url,
             data={"status": status.value, "detail": detail},
-            headers={"Content-Type": "application/json"},
+            headers=headers,
         )
         return InvocationRecord.parse_obj(response.from_json(json_path=["data"]))
 
     def query_invocations(
         self, filters: dict[str, Any], page_token: dict[str, str] | None = None
     ) -> PaginatedList[InvocationRecord]:
         if page_token:
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/datasets/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 from typing import Any
 import urllib.parse
 
 from ...http import HttpClient
-from ...model.datasets import (
+from ...pagination import PaginatedList
+from ...serde import pydantic_jsonable_dict
+from ..files import FileRecord
+from .delegate import (
     AccessMode,
-    Administrator,
     Credentials,
     DatasetDelegate,
+)
+from .http_resources import CreateDatasetRequest
+from .record import (
+    Administrator,
     DatasetRecord,
     StorageLocation,
 )
-from ...model.files import FileRecord
-from ...pagination import PaginatedList
-from ...serde import pydantic_jsonable_dict
-from .http_resources import CreateDatasetRequest
 
 
 class DatasetHttpDelegate(DatasetDelegate):
     __http_client: HttpClient
     __roboto_service_base_url: str
 
     def __init__(self, roboto_service_base_url: str, http_client: HttpClient) -> None:
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import pathlib
 
 from ...http import HttpClient
-from ...model.files import (
-    FileDelegate,
-    FileRecord,
-    FileTag,
-)
 from ...serde import pydantic_jsonable_dict
+from .delegate import FileDelegate, FileTag
 from .http_resources import (
     CreateFileRequest,
     DeleteFileRequest,
 )
+from .record import FileRecord
 
 
 class FileHttpDelegate(FileDelegate):
     """
     A file delegate intended for service/admin-use only. Public methods are not implemented.
     Capable of making HTTP requests to the Roboto API to memorialize file records.
     """
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/delegate/files/s3_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import pathlib
 from typing import Any, Protocol
 import urllib.parse
 
 import boto3
 
-from ...model.files import (
-    FileDelegate,
-    FileRecord,
-    FileTag,
-)
+from .delegate import FileDelegate, FileTag
+from .record import FileRecord
 
 
 class S3Credentials(Protocol):
     access_key_id: str
     secret_access_key: str
     session_token: str
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 
 from .delegate import OrgDelegate
 from .http_delegate import OrgHttpDelegate
-from .http_resources import CreateOrgRequest
+from .http_resources import (
+    BindEmailDomainRequest,
+    CreateOrgRequest,
+    InviteUserRequest,
+)
 from .org import Org
 from .org_role import OrgRole
 from .record import (
     OrgRecord,
-    OrgRoleLevel,
+    OrgRoleName,
     OrgRoleRecord,
     OrgTier,
     OrgType,
 )
 
 __all__ = [
-    "OrgDelegate",
-    "OrgHttpDelegate",
+    "BindEmailDomainRequest",
     "CreateOrgRequest",
+    "InviteUserRequest",
     "Org",
-    "OrgRole",
+    "OrgDelegate",
+    "OrgHttpDelegate",
     "OrgRecord",
+    "OrgRole",
+    "OrgRoleName",
     "OrgRoleRecord",
-    "OrgType",
     "OrgTier",
-    "OrgRoleLevel",
+    "OrgType",
 ]
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 
 from ...http import (
-    ORG_OVERRIDE_HEADER,
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...serde import pydantic_jsonable_dict
-from .delegate import OrgDelegate
-from .http_resources import CreateOrgRequest
-from .record import (
-    OrgRecord,
-    OrgRoleRecord,
-    OrgType,
-)
+from .delegate import TokenDelegate
+from .http_resources import CreateTokenRequest
+from .record import TokenRecord
 
 
-class OrgHttpDelegate(OrgDelegate):
+class TokenHttpDelegate(TokenDelegate):
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
-    def create_org(
-        self, creator_user_id: str | None, name: str, org_type: OrgType
-    ) -> OrgRecord:
-        url = self.__http_client.url("v1/orgs")
+    def get_tokens_for_user(self, user_id: str | None) -> list[TokenRecord]:
+        url = self.__http_client.url("v1/tokens")
+        headers = {}
+        if user_id is not None:
+            headers[USER_OVERRIDE_HEADER] = user_id
+
+        response = self.__http_client.get(url=url, headers=headers)
+        unmarshalled = response.from_json(json_path=["data"])
+        return [TokenRecord.parse_obj(record) for record in unmarshalled]
+
+    def create_token(
+        self, user_id: str | None, expiry_days: int, name: str, description: str | None
+    ) -> TokenRecord:
+        url = self.__http_client.url("v1/tokens")
         headers = {"Content-Type": "application/json"}
+        if user_id is not None:
+            headers[USER_OVERRIDE_HEADER] = user_id
 
-        if creator_user_id is not None:
-            headers[USER_OVERRIDE_HEADER] = creator_user_id
+        data = CreateTokenRequest(
+            expiry_days=expiry_days, name=name, description=description
+        )
 
-        request_body = CreateOrgRequest(name=name, org_type=org_type)
         response = self.__http_client.post(
-            url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
+            url=url, headers=headers, data=pydantic_jsonable_dict(data)
         )
-        return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
+        return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def orgs_for_user(self, user_id: str | None) -> list[OrgRecord]:
-        url = self.__http_client.url("v1/orgs/list")
-        response = self.__http_client.get(url=url)
-        return [
-            OrgRecord.parse_obj(record)
-            for record in response.from_json(json_path=["data"])
-        ]
+    def delete_token(self, token_id: str) -> None:
+        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
+        self.__http_client.delete(url=url)
 
-    def org_roles_for_user(self, user_id: str | None) -> list[OrgRoleRecord]:
-        url = self.__http_client.url("v1/orgs/roles")
+    def get_token_by_token_id(self, token_id: str) -> TokenRecord:
+        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
         response = self.__http_client.get(url=url)
-        return [
-            OrgRoleRecord.parse_obj(record)
-            for record in response.from_json(json_path=["data"])
-        ]
-
-    def get_org_by_id(self, org_id: str) -> OrgRecord:
-        url = self.__http_client.url("v1/orgs")
-        headers = {ORG_OVERRIDE_HEADER: org_id}
-        response = self.__http_client.get(url=url, headers=headers)
-        return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
-
-    def delete_org(self, org_id: str) -> None:
-        url = self.__http_client.url("v1/orgs")
-        headers = {ORG_OVERRIDE_HEADER: org_id}
-        self.__http_client.delete(url=url, headers=headers)
+        return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/token.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Any
 
 from ...serde import pydantic_jsonable_dict
-from .delegate import OrgDelegate
-from .record import OrgRecord, OrgType
+from .delegate import TokenDelegate
+from .record import TokenRecord
 
 
-class Org:
-    __record: OrgRecord
-    __org_delegate: OrgDelegate
+class Token:
+    __record: TokenRecord
+    __token_delegate: TokenDelegate
+
+    @classmethod
+    def by_token_id(cls, token_id: str, token_delegate: TokenDelegate) -> "Token":
+        record = token_delegate.get_token_by_token_id(token_id=token_id)
+        return cls(record=record, token_delegate=token_delegate)
+
+    @classmethod
+    def by_user_id(
+        cls, user_id: str | None, token_delegate: TokenDelegate
+    ) -> list["Token"]:
+        records = token_delegate.get_tokens_for_user(user_id=user_id)
+        return [cls(record=record, token_delegate=token_delegate) for record in records]
 
     @classmethod
     def create(
         cls,
-        creator_user_id: str | None,
+        user_id: str | None,
+        expiry_days: int,
         name: str,
-        org_type: OrgType,
-        org_delegate: OrgDelegate,
+        description: str | None,
+        token_delegate: TokenDelegate,
     ):
-        record = org_delegate.create_org(
-            creator_user_id=creator_user_id, name=name, org_type=org_type
+        record = token_delegate.create_token(
+            user_id=user_id, expiry_days=expiry_days, name=name, description=description
         )
-        return cls(record=record, org_delegate=org_delegate)
-
-    @classmethod
-    def by_org_id(cls, org_id: str, org_delegate: OrgDelegate) -> "Org":
-        record = org_delegate.get_org_by_id(org_id=org_id)
-        return cls(record=record, org_delegate=org_delegate)
+        return cls(record=record, token_delegate=token_delegate)
 
-    @classmethod
-    def by_user_id(cls, user_id: str | None, org_delegate: OrgDelegate) -> list["Org"]:
-        records = org_delegate.orgs_for_user(user_id=user_id)
-        return [cls(record=record, org_delegate=org_delegate) for record in records]
-
-    def delete(self) -> None:
-        self.__org_delegate.delete_org(org_id=self.org_id)
+    def delete(self):
+        assert self.__record.context is not None
+        return self.__token_delegate.delete_token(
+            token_id=self.__record.context.token_id
+        )
 
-    def __init__(self, record: OrgRecord, org_delegate: OrgDelegate):
+    def __init__(self, record: TokenRecord, token_delegate: TokenDelegate):
         self.__record = record
-        self.__org_delegate = org_delegate
+        self.__token_delegate = token_delegate
 
     def to_dict(self) -> dict[str, Any]:
         return pydantic_jsonable_dict(self.__record)
 
     @property
-    def org_id(self):
-        return self.__record.org_id
+    def secret(self) -> str | None:
+        return self.__record.secret
+
+    @property
+    def user_id(self) -> str | None:
+        return self.__record.user_id
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 from typing import Any
 
 from ...serde import pydantic_jsonable_dict
 from .delegate import OrgDelegate
 from .org import Org
-from .record import OrgRoleLevel, OrgRoleRecord
+from .record import OrgRoleName, OrgRoleRecord
 
 
 class OrgRole:
     __record: OrgRoleRecord
     __org_delegate: OrgDelegate
     __org: Org
 
@@ -33,9 +33,9 @@
         return self.__record.org.org_id
 
     @property
     def org(self) -> Org:
         return self.__org
 
     @property
-    def roles(self) -> list[OrgRoleLevel]:
+    def roles(self) -> list[OrgRoleName]:
         return self.__record.roles
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/record.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     org_id: str
     name: str
     org_type: OrgType
     tier: OrgTier
     members: int
 
 
-class OrgRoleLevel(str, enum.Enum):
+class OrgRoleName(str, enum.Enum):
     user = "user"
     admin = "admin"
+    owner = "owner"
 
 
 class OrgRoleRecord(pydantic.BaseModel):
     user_id: str
     org: OrgRecord
-    roles: list[OrgRoleLevel]
+    roles: list[OrgRoleName]
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,102 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 
 from ...http import (
+    ORG_OVERRIDE_HEADER,
     USER_OVERRIDE_HEADER,
     HttpClient,
 )
 from ...serde import pydantic_jsonable_dict
-from .delegate import TokenDelegate
-from .http_resources import CreateTokenRequest
-from .record import TokenRecord
+from .delegate import OrgDelegate
+from .http_resources import (
+    BindEmailDomainRequest,
+    CreateOrgRequest,
+    InviteUserRequest,
+)
+from .record import (
+    OrgRecord,
+    OrgRoleRecord,
+    OrgType,
+)
 
 
-class TokenHttpDelegate(TokenDelegate):
+class OrgHttpDelegate(OrgDelegate):
     __http_client: HttpClient
 
     def __init__(self, http_client: HttpClient):
         super().__init__()
         self.__http_client = http_client
 
-    def get_tokens_for_user(self, user_id: str | None) -> list[TokenRecord]:
-        url = self.__http_client.url("v1/tokens")
-        headers = {}
-        if user_id is not None:
-            headers[USER_OVERRIDE_HEADER] = user_id
-
-        response = self.__http_client.get(url=url, headers=headers)
-        unmarshalled = response.from_json(json_path=["data"])
-        return [TokenRecord.parse_obj(record) for record in unmarshalled]
-
-    def create_token(
-        self, user_id: str | None, expiry_days: int, name: str, description: str | None
-    ) -> TokenRecord:
-        url = self.__http_client.url("v1/tokens")
+    def create_org(
+        self,
+        creator_user_id: str | None,
+        name: str,
+        org_type: OrgType,
+        bind_email_domain: bool = False,
+    ) -> OrgRecord:
+        url = self.__http_client.url("v1/orgs")
         headers = {"Content-Type": "application/json"}
-        if user_id is not None:
-            headers[USER_OVERRIDE_HEADER] = user_id
 
-        data = CreateTokenRequest(
-            expiry_days=expiry_days, name=name, description=description
-        )
+        if creator_user_id is not None:
+            headers[USER_OVERRIDE_HEADER] = creator_user_id
 
+        request_body = CreateOrgRequest(
+            name=name, org_type=org_type, bind_email_domain=bind_email_domain
+        )
         response = self.__http_client.post(
-            url=url, headers=headers, data=pydantic_jsonable_dict(data)
+            url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
         )
-        return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
+        return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
 
-    def delete_token(self, token_id: str) -> None:
-        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
-        self.__http_client.delete(url=url)
+    def orgs_for_user(self, user_id: str | None) -> list[OrgRecord]:
+        url = self.__http_client.url("v1/orgs/list")
+        response = self.__http_client.get(url=url)
+        return [
+            OrgRecord.parse_obj(record)
+            for record in response.from_json(json_path=["data"])
+        ]
 
-    def get_token_by_token_id(self, token_id: str) -> TokenRecord:
-        url = self.__http_client.url(f"v1/tokens/id/{token_id}")
+    def org_roles_for_user(self, user_id: str | None) -> list[OrgRoleRecord]:
+        url = self.__http_client.url("v1/orgs/roles")
         response = self.__http_client.get(url=url)
-        return TokenRecord.parse_obj(response.from_json(json_path=["data"]))
+        return [
+            OrgRoleRecord.parse_obj(record)
+            for record in response.from_json(json_path=["data"])
+        ]
+
+    def get_org_by_id(self, org_id: str) -> OrgRecord:
+        url = self.__http_client.url("v1/orgs")
+        headers = {ORG_OVERRIDE_HEADER: org_id}
+        response = self.__http_client.get(url=url, headers=headers)
+        return OrgRecord.parse_obj(response.from_json(json_path=["data"]))
+
+    def delete_org(self, org_id: str) -> None:
+        url = self.__http_client.url("v1/orgs")
+        headers = {ORG_OVERRIDE_HEADER: org_id}
+        self.__http_client.delete(url=url, headers=headers)
+
+    def bind_email_domain(self, org_id: str, email_domain: str):
+        url = self.__http_client.url("v1/orgs/subdomains")
+        headers = {ORG_OVERRIDE_HEADER: org_id}
+        request_body = BindEmailDomainRequest(email_domain=email_domain)
+        self.__http_client.put(
+            url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
+        )
+
+    def invite_user_to_org(
+        self, invited_user_id: str, org_id: str, inviting_user_id: str | None = None
+    ):
+        url = self.__http_client.url("v1/orgs/invites")
+        headers = {ORG_OVERRIDE_HEADER: org_id}
+        request_body = InviteUserRequest(invited_user_id=invited_user_id)
+        self.__http_client.post(
+            url=url, headers=headers, data=pydantic_jsonable_dict(request_body)
+        )
+
+    def accept_org_invite(self, invite_id: str, user_id: str | None = None):
+        url = self.__http_client.url(f"v1/orgs/invites/accept/{invite_id}")
+        self.__http_client.post(url=url)
+
+    def decline_org_invite(self, invite_id: str, user_id: str | None = None):
+        url = self.__http_client.url(f"v1/orgs/invites/decline/{invite_id}")
+        self.__http_client.post(url=url)
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 
 import collections.abc
 from typing import Any
 
-from ...model.actions.action_delegate import (
-    ActionDelegate,
-)
+from ...domain.actions import ActionDelegate
 from ...serde import pydantic_jsonable_dict
 from .trigger_delegate import TriggerDelegate
 from .trigger_record import TriggerRecord
 
 
 class Trigger:
     __record: TriggerRecord
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,17 +11,19 @@
     ServerError,
 )
 from .request_decorators import (
     LocalAuthDecorator,
     PATAuthDecorator,
     SigV4AuthDecorator,
 )
+from .testing_util import FakeHttpResponseFactory
 
 __all__ = (
     "ClientError",
+    "FakeHttpResponseFactory",
     "HttpClient",
     "HttpError",
     "LocalAuthDecorator",
     "PATAuthDecorator",
     "ServerError",
     "SigV4AuthDecorator",
     "ORG_OVERRIDE_HEADER",
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,68 @@
 #  Copyright (c) 2023 Roboto Technologies, Inc.
 from .action import Action
 from .action_delegate import (
     ActionDelegate,
     ContainerCredentials,
     UpdateCondition,
 )
+from .action_http_delegate import (
+    ActionHttpDelegate,
+)
+from .action_http_resources import (
+    ContainerUploadCredentials,
+    CreateActionRequest,
+    UpdateActionRequest,
+)
 from .action_record import ActionRecord
 from .error import (
     ActionUpdateConditionCheckFailure,
     InvocationError,
 )
 from .invocation import Invocation
 from .invocation_delegate import (
     InvocationDelegate,
 )
+from .invocation_http_delegate import (
+    InvocationHttpDelegate,
+)
+from .invocation_http_resources import (
+    CreateInvocationRequest,
+    SetLogsLocationRequest,
+    UpdateInvocationStatus,
+)
 from .invocation_record import (
     InvocationDataSource,
     InvocationDataSourceType,
     InvocationDetail,
     InvocationRecord,
     InvocationSource,
     InvocationStatus,
     InvocationStatusRecord,
 )
 
 __all__ = (
     "Action",
     "ActionDelegate",
+    "ActionHttpDelegate",
     "ActionRecord",
     "ActionUpdateConditionCheckFailure",
     "ContainerCredentials",
+    "ContainerUploadCredentials",
+    "CreateActionRequest",
+    "CreateInvocationRequest",
     "Invocation",
     "InvocationDataSource",
     "InvocationDataSourceType",
     "InvocationDelegate",
     "InvocationDetail",
     "InvocationError",
+    "InvocationHttpDelegate",
     "InvocationRecord",
     "InvocationSource",
     "InvocationStatus",
     "InvocationStatusRecord",
+    "SetLogsLocationRequest",
+    "UpdateActionRequest",
     "UpdateCondition",
+    "UpdateInvocationStatus",
 )
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/action_record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,55 @@
-import collections.abc
+import abc
 from typing import Any
 
-from ...serde import pydantic_jsonable_dict
-from .invocation_delegate import (
-    InvocationDelegate,
-)
+from ...pagination import PaginatedList
 from .invocation_record import (
+    InvocationDataSourceType,
     InvocationRecord,
+    InvocationSource,
     InvocationStatus,
 )
 
 
-class Invocation:
-    __invocation_delegate: InvocationDelegate
-    __record: InvocationRecord
-
-    @classmethod
-    def from_id(
-        cls, invocation_id: str, invocation_delegate: InvocationDelegate
-    ) -> "Invocation":
-        record = invocation_delegate.get_by_id(invocation_id)
-        return cls(record, invocation_delegate)
-
-    @classmethod
-    def query(
-        cls, filters: dict[str, Any], invocation_delegate: InvocationDelegate
-    ) -> collections.abc.Generator["Invocation", None, None]:
-        known_keys = set(InvocationRecord.__fields__.keys())
-        actual_keys = set(filters.keys())
-        unknown_keys = actual_keys - known_keys
-        if unknown_keys:
-            plural = len(unknown_keys) > 1
-            msg = (
-                "are not known attributes of Invocation"
-                if plural
-                else "is not a known attribute of Invocation"
-            )
-            raise ValueError(f"{unknown_keys} {msg}. Known attributes: {known_keys}")
-
-        paginated_results = invocation_delegate.query_invocations(filters)
-        while True:
-            for record in paginated_results.items:
-                yield cls(record, invocation_delegate)
-            if paginated_results.next_token:
-                paginated_results = invocation_delegate.query_invocations(
-                    filters, paginated_results.next_token
-                )
-            else:
-                break
-
-    def __init__(
-        self, record: InvocationRecord, invocation_delegate: InvocationDelegate
-    ) -> None:
-        self.__invocation_delegate = invocation_delegate
-        self.__record = record
-
-    def to_dict(self) -> dict[str, Any]:
-        return pydantic_jsonable_dict(self.__record)
-
-    def update_status(
-        self, next_status: InvocationStatus, detail: str | None = "None"
-    ) -> None:
-        updated_record = self.__invocation_delegate.update_invocation_status(
-            self.__record, next_status, detail
-        )
-        self.__record = updated_record
+class InvocationDelegate(abc.ABC):
+    @abc.abstractmethod
+    def create_invocation(
+        self,
+        action_name: str,
+        input_data: list[str],
+        data_source_id: str,
+        data_source_type: InvocationDataSourceType,
+        invocation_source: InvocationSource,
+        invocation_source_id: str | None = None,
+        tenant_id: str | None = None,
+    ) -> InvocationRecord:
+        """Create an Invocation"""
+        raise NotImplementedError("create_invocation")
+
+    @abc.abstractmethod
+    def get_by_id(
+        self, invocation_id: str, org_id: str | None = None
+    ) -> InvocationRecord:
+        """Get an Invocation by ID"""
+        raise NotImplementedError("get_by_id")
+
+    @abc.abstractmethod
+    def set_logs_location(
+        self, record: InvocationRecord, bucket: str, prefix: str
+    ) -> InvocationRecord:
+        raise NotImplementedError("set_logs_location")
+
+    @abc.abstractmethod
+    def update_invocation_status(
+        self,
+        invocation: InvocationRecord,
+        status: InvocationStatus,
+        detail: str | None = None,
+    ) -> InvocationRecord:
+        """Update the status of an Invocation"""
+        raise NotImplementedError("update_invocation_status")
+
+    @abc.abstractmethod
+    def query_invocations(
+        self, filters: dict[str, Any], page_token: dict[str, str] | None = None
+    ) -> PaginatedList[InvocationRecord]:
+        raise NotImplementedError("query_actions")
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/actions/invocation_record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     """Source of data for an Action's InputBinding"""
 
     Dataset = "Dataset"
 
 
 class InvocationDataSource(pydantic.BaseModel):
     type: InvocationDataSourceType
-    id: str | None = None
+    # The "type" determines the meaning of "id":
+    #   - if type is "Dataset," id is a dataset_id
+    id: str
 
 
 class InvocationSource(enum.Enum):
     Trigger = "Trigger"
     Manual = "Manual"
 
 
@@ -47,13 +49,14 @@
     timestamp: datetime.datetime  # Persisted as ISO 8601 string in UTC
 
 
 class InvocationRecord(pydantic.BaseModel):
     id: str
     tenant_id: str
     action_name: str
+    created: datetime.datetime  # Persisted as ISO 8601 string in UTC
     data_source: InvocationDataSource
     input_data: list[str]
-    logs: str | None = None
-    created: datetime.datetime  # Persisted as ISO 8601 string in UTC
     invoked_by: InvocationDetail
+    logs_bucket: str | None = None
+    logs_prefix: str | None = None
     status: list[InvocationStatusRecord] = pydantic.Field(default_factory=list)
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/dataset.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import collections.abc
 import pathlib
 from typing import Any
 
 import pathspec
 
-from ...delegate.files import FileS3Delegate
 from ...serde import pydantic_jsonable_dict
-from ..files import File, FileDelegate, FileTag
+from ..files import (
+    File,
+    FileDelegate,
+    FileS3Delegate,
+    FileTag,
+)
 from .delegate import (
     AccessMode,
     Credentials,
     DatasetDelegate,
     StorageLocation,
 )
 from .record import Administrator, DatasetRecord
```

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/datasets/record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/files/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/model/files/file.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.1/PKG-INFO` & `roboto_sdk-0.1.2a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.1
+Version: 0.1.2a0
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

