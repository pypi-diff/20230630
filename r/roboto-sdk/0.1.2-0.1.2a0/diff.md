# Comparing `tmp/roboto_sdk-0.1.2.tar.gz` & `tmp/roboto_sdk-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboto_sdk-0.1.2.tar", max compression
+gzip compressed data, was "roboto_sdk-0.1.2a0.tar", max compression
```

## Comparing `roboto_sdk-0.1.2.tar` & `roboto_sdk-0.1.2a0.tar`

### file list

```diff
@@ -1,86 +1,121 @@
--rw-r--r--   0        0        0       22 2023-05-31 20:34:51.104994 roboto_sdk-0.1.2/README.md
--rw-r--r--   0        0        0      806 2023-06-29 22:49:43.261224 roboto_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       62 2023-05-31 20:34:51.105420 roboto_sdk-0.1.2/src/roboto_sdk/__init__.py
--rw-r--r--   0        0        0       48 2023-05-31 20:51:22.684541 roboto_sdk-0.1.2/src/roboto_sdk/auth/__init__.py
--rw-r--r--   0        0        0     3892 2023-06-25 17:00:28.230327 roboto_sdk-0.1.2/src/roboto_sdk/auth/pat.py
--rw-r--r--   0        0        0      132 2023-05-31 21:34:25.532839 roboto_sdk-0.1.2/src/roboto_sdk/cli/__init__.py
--rw-r--r--   0        0        0      334 2023-06-21 21:00:10.362037 roboto_sdk-0.1.2/src/roboto_sdk/cli/command/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-21 21:02:17.537089 roboto_sdk-0.1.2/src/roboto_sdk/cli/command/args.py
--rw-r--r--   0        0        0     2033 2023-06-21 21:18:40.940344 roboto_sdk-0.1.2/src/roboto_sdk/cli/command/model.py
--rw-r--r--   0        0        0      790 2023-06-29 16:05:04.384582 roboto_sdk-0.1.2/src/roboto_sdk/cli/context.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.2/src/roboto_sdk/cli/datasets/__init__.py
--rw-r--r--   0        0        0     6691 2023-06-29 16:05:04.385345 roboto_sdk-0.1.2/src/roboto_sdk/cli/datasets/commands.py
--rw-r--r--   0        0        0     3223 2023-06-29 16:05:04.385760 roboto_sdk-0.1.2/src/roboto_sdk/cli/entry.py
--rw-r--r--   0        0        0      108 2023-06-21 21:18:40.926071 roboto_sdk-0.1.2/src/roboto_sdk/cli/help/__init__.py
--rw-r--r--   0        0        0      167 2023-06-21 21:18:40.928579 roboto_sdk-0.1.2/src/roboto_sdk/cli/help/args.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.2/src/roboto_sdk/cli/orgs/__init__.py
--rw-r--r--   0        0        0     3386 2023-06-28 22:21:48.431065 roboto_sdk-0.1.2/src/roboto_sdk/cli/orgs/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.2/src/roboto_sdk/cli/tokens/__init__.py
--rw-r--r--   0        0        0     3301 2023-06-27 00:52:24.673209 roboto_sdk-0.1.2/src/roboto_sdk/cli/tokens/commands.py
--rw-r--r--   0        0        0      110 2023-06-21 18:17:36.115870 roboto_sdk-0.1.2/src/roboto_sdk/cli/triggers/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-21 21:18:41.332847 roboto_sdk-0.1.2/src/roboto_sdk/cli/triggers/commands.py
--rw-r--r--   0        0        0      110 2023-06-01 20:29:20.319243 roboto_sdk-0.1.2/src/roboto_sdk/cli/users/__init__.py
--rw-r--r--   0        0        0      733 2023-06-23 21:06:13.848323 roboto_sdk-0.1.2/src/roboto_sdk/cli/users/commands.py
--rw-r--r--   0        0        0       48 2023-06-21 18:17:36.116077 roboto_sdk-0.1.2/src/roboto_sdk/domain/__init__.py
--rw-r--r--   0        0        0     1633 2023-06-29 15:35:56.463310 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/__init__.py
--rw-r--r--   0        0        0     7019 2023-06-29 15:35:56.463411 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action.py
--rw-r--r--   0        0        0     2804 2023-06-29 15:35:56.463471 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_delegate.py
--rw-r--r--   0        0        0     5167 2023-06-29 15:35:56.463534 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_http_delegate.py
--rw-r--r--   0        0        0      651 2023-06-29 15:35:56.463581 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_http_resources.py
--rw-r--r--   0        0        0      792 2023-06-29 15:35:56.463632 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_record.py
--rw-r--r--   0        0        0      106 2023-06-29 15:35:56.463681 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/error.py
--rw-r--r--   0        0        0     4294 2023-06-29 15:35:56.463871 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation.py
--rw-r--r--   0        0        0     1653 2023-06-29 15:35:56.463945 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_delegate.py
--rw-r--r--   0        0        0     4684 2023-06-29 15:35:56.464027 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_http_delegate.py
--rw-r--r--   0        0        0      534 2023-06-29 15:35:56.464078 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_http_resources.py
--rw-r--r--   0        0        0     1592 2023-06-29 15:35:56.464142 roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_record.py
--rw-r--r--   0        0        0      546 2023-06-29 15:35:56.464218 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/__init__.py
--rw-r--r--   0        0        0     9572 2023-06-29 15:35:56.464288 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/dataset.py
--rw-r--r--   0        0        0     2132 2023-06-29 15:35:56.464354 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/delegate.py
--rw-r--r--   0        0        0     4759 2023-06-29 15:35:56.464409 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/http_delegate.py
--rw-r--r--   0        0        0      340 2023-06-29 15:35:56.464452 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/http_resources.py
--rw-r--r--   0        0        0      817 2023-06-29 15:35:56.464498 roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/record.py
--rw-r--r--   0        0        0      436 2023-06-29 15:35:56.464570 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-29 15:35:56.464729 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/delegate.py
--rw-r--r--   0        0        0      771 2023-06-29 15:35:56.464889 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/file.py
--rw-r--r--   0        0        0     2110 2023-06-29 15:35:56.464947 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/http_delegate.py
--rw-r--r--   0        0        0      168 2023-06-29 15:35:56.464990 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/http_resources.py
--rw-r--r--   0        0        0      385 2023-06-29 15:35:56.465086 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/record.py
--rw-r--r--   0        0        0     2320 2023-06-29 15:35:56.465141 roboto_sdk-0.1.2/src/roboto_sdk/domain/files/s3_delegate.py
--rw-r--r--   0        0        0      633 2023-06-29 21:05:11.294925 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-29 00:30:17.060813 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/delegate.py
--rw-r--r--   0        0        0     3610 2023-06-29 00:30:17.061047 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/http_delegate.py
--rw-r--r--   0        0        0      359 2023-06-28 06:35:03.341928 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/http_resources.py
--rw-r--r--   0        0        0     2381 2023-06-29 00:30:17.061322 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/org.py
--rw-r--r--   0        0        0     1145 2023-06-28 21:49:35.087173 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/org_role.py
--rw-r--r--   0        0        0      563 2023-06-29 21:05:11.295549 roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/record.py
--rw-r--r--   0        0        0      387 2023-06-23 21:06:13.848727 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/__init__.py
--rw-r--r--   0        0        0      818 2023-06-27 00:52:24.673479 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/delegate.py
--rw-r--r--   0        0        0     1968 2023-06-27 00:52:24.673652 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/http_delegate.py
--rw-r--r--   0        0        0      184 2023-06-27 00:52:24.673821 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/http_resources.py
--rw-r--r--   0        0        0      412 2023-06-27 00:52:24.673996 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/record.py
--rw-r--r--   0        0        0     1807 2023-06-27 00:52:24.674186 roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/token.py
--rw-r--r--   0        0        0      391 2023-06-21 18:17:36.116185 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-21 18:17:36.116295 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/http_delegate.py
--rw-r--r--   0        0        0      205 2023-06-21 18:17:36.116397 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/http_resources.py
--rw-r--r--   0        0        0     2661 2023-06-29 16:05:04.386157 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/trigger.py
--rw-r--r--   0        0        0      857 2023-06-21 18:17:36.116610 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/trigger_delegate.py
--rw-r--r--   0        0        0      249 2023-06-21 18:17:36.116722 roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/trigger_record.py
--rw-r--r--   0        0        0      262 2023-06-23 21:06:13.849582 roboto_sdk-0.1.2/src/roboto_sdk/domain/users/__init__.py
--rw-r--r--   0        0        0     1016 2023-06-23 21:17:31.788229 roboto_sdk-0.1.2/src/roboto_sdk/domain/users/http_delegate.py
--rw-r--r--   0        0        0     1200 2023-06-23 21:17:31.796065 roboto_sdk-0.1.2/src/roboto_sdk/domain/users/user.py
--rw-r--r--   0        0        0      451 2023-06-23 21:17:31.793509 roboto_sdk-0.1.2/src/roboto_sdk/domain/users/user_delegate.py
--rw-r--r--   0        0        0      162 2023-06-23 21:06:13.850109 roboto_sdk-0.1.2/src/roboto_sdk/domain/users/user_record.py
--rw-r--r--   0        0        0      704 2023-06-29 00:30:17.043102 roboto_sdk-0.1.2/src/roboto_sdk/http/__init__.py
--rw-r--r--   0        0        0      216 2023-06-23 21:06:13.850449 roboto_sdk-0.1.2/src/roboto_sdk/http/constants.py
--rw-r--r--   0        0        0     8880 2023-06-13 17:13:48.415283 roboto_sdk-0.1.2/src/roboto_sdk/http/http_client.py
--rw-r--r--   0        0        0     3032 2023-06-25 17:23:12.393083 roboto_sdk-0.1.2/src/roboto_sdk/http/request_decorators.py
--rw-r--r--   0        0        0      994 2023-06-29 00:30:17.043313 roboto_sdk-0.1.2/src/roboto_sdk/http/testing_util.py
--rw-r--r--   0        0        0      158 2023-05-31 20:51:22.686567 roboto_sdk-0.1.2/src/roboto_sdk/logging.py
--rw-r--r--   0        0        0      211 2023-06-26 18:41:27.400684 roboto_sdk-0.1.2/src/roboto_sdk/pagination.py
--rw-r--r--   0        0        0      168 2023-06-25 17:00:28.638279 roboto_sdk-0.1.2/src/roboto_sdk/profile/__init__.py
--rw-r--r--   0        0        0     2809 2023-06-25 17:05:30.425831 roboto_sdk-0.1.2/src/roboto_sdk/profile/profile.py
--rw-r--r--   0        0        0        0 2023-05-31 20:34:27.418611 roboto_sdk-0.1.2/src/roboto_sdk/py.typed
--rw-r--r--   0        0        0      651 2023-06-13 17:13:48.417645 roboto_sdk-0.1.2/src/roboto_sdk/serde.py
--rw-r--r--   0        0        0      112 2023-06-01 19:18:26.925334 roboto_sdk-0.1.2/src/roboto_sdk/time.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 roboto_sdk-0.1.2/PKG-INFO
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

### Comparing `roboto_sdk-0.1.2/pyproject.toml` & `roboto_sdk-0.1.2a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires-python = ">=3.10"
 # Ignore this version attribute, it is here to satisfy setuptools.
 # The actual version is set by Poetry in the [tool.poetry] section.
 version = "0.0.0"
 
 [tool.poetry]
 name = "roboto_sdk"
-version = "0.1.2"
+version = "0.1.2a0"
 description = "Tools for interacting with roboto.ai"
 license = "MIT"
 readme = "README.md"
 authors = ["Roboto <admin@roboto.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/auth/pat.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/auth/pat.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/command/args.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/args.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/command/model.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/command/model.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/context.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/context.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/datasets/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/entry.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/entry.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/orgs/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/orgs/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/tokens/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/tokens/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/triggers/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/triggers/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/cli/users/commands.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/cli/users/commands.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_http_resources.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/action_record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/action_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_http_resources.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_http_resources.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/actions/invocation_record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/actions/invocation_record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/dataset.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/datasets/record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/datasets/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/files/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/files/file.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/file.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/files/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/files/s3_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/files/s3_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/org.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/org.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/org_role.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/org_role.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/orgs/record.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/orgs/record.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/tokens/token.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/tokens/token.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/trigger.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/triggers/trigger_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/triggers/trigger_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/users/http_delegate.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/http_delegate.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/domain/users/user.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/domain/users/user.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/http/__init__.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/__init__.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/http/http_client.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/http_client.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/http/request_decorators.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/request_decorators.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/http/testing_util.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/http/testing_util.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/profile/profile.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/profile/profile.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/src/roboto_sdk/serde.py` & `roboto_sdk-0.1.2a0/src/roboto_sdk/serde.py`

 * *Files identical despite different names*

### Comparing `roboto_sdk-0.1.2/PKG-INFO` & `roboto_sdk-0.1.2a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboto-sdk
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Tools for interacting with roboto.ai
 License: MIT
 Author: Roboto
 Author-email: admin@roboto.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

