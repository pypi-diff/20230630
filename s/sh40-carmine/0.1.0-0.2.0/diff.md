# Comparing `tmp/sh40_carmine-0.1.0.tar.gz` & `tmp/sh40_carmine-0.2.0.tar.gz`

## Comparing `sh40_carmine-0.1.0.tar` & `sh40_carmine-0.2.0.tar`

### file list

```diff
@@ -1,212 +1,8 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.coverage
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/target.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/__future__.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/__future__.meta.json
--rw-r--r--   0        0        0   108426 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_collections_abc.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_collections_abc.meta.json
--rw-r--r--   0        0        0    23590 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_thread.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_thread.meta.json
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_warnings.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_warnings.meta.json
--rw-r--r--   0        0        0    19402 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0        0        0    60911 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/array.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0        0        0   123959 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/ast.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/ast.meta.json
--rw-r--r--   0        0        0   970019 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0        0        0   127086 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/codecs.meta.json
--rw-r--r--   0        0        0    86649 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/contextlib.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/contextlib.meta.json
--rw-r--r--   0        0        0    54155 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/dataclasses.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/dataclasses.meta.json
--rw-r--r--   0        0        0   141694 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/datetime.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/datetime.meta.json
--rw-r--r--   0        0        0    43075 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/dis.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/dis.meta.json
--rw-r--r--   0        0        0    61346 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/enum.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/enum.meta.json
--rw-r--r--   0        0        0   131830 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/functools.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/functools.meta.json
--rw-r--r--   0        0        0    19070 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/genericpath.meta.json
--rw-r--r--   0        0        0   310434 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/inspect.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/inspect.meta.json
--rw-r--r--   0        0        0    86155 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/io.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0        0        0   255327 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/itertools.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/itertools.meta.json
--rw-r--r--   0        0        0    25472 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/mmap.meta.json
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/opcode.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/opcode.meta.json
--rw-r--r--   0        0        0    87573 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/pathlib.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/pathlib.meta.json
--rw-r--r--   0        0        0    47463 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/pickle.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/pickle.meta.json
--rw-r--r--   0        0        0    71992 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/posixpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/posixpath.meta.json
--rw-r--r--   0        0        0    54774 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/re.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/re.meta.json
--rw-r--r--   0        0        0    71005 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/shutil.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/shutil.meta.json
--rw-r--r--   0        0        0    14940 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_compile.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_compile.meta.json
--rw-r--r--   0        0        0    29609 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_constants.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_constants.meta.json
--rw-r--r--   0        0        0    51285 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_parse.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sre_parse.meta.json
--rw-r--r--   0        0        0    17858 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/string.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/string.meta.json
--rw-r--r--   0        0        0   153845 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/subprocess.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/subprocess.meta.json
--rw-r--r--   0        0        0   135640 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0        0        0   128599 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/tempfile.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/tempfile.meta.json
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/textwrap.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/textwrap.meta.json
--rw-r--r--   0        0        0    65034 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/threading.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/threading.meta.json
--rw-r--r--   0        0        0    41906 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/time.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/time.meta.json
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/token.data.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/token.meta.json
--rw-r--r--   0        0        0    53001 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/tokenize.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/tokenize.meta.json
--rw-r--r--   0        0        0   243481 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/types.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0        0        0   493876 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0        0        0    49604 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/typing_extensions.meta.json
--rw-r--r--   0        0        0    23410 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/warnings.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/warnings.meta.json
--rw-r--r--   0        0        0    73995 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/carmine/__about__.data.json
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/carmine/__about__.meta.json
--rw-r--r--   0        0        0   350041 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/collections/abc.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/collections/abc.meta.json
--rw-r--r--   0        0        0   130826 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/__init__.meta.json
--rw-r--r--   0        0        0    12280 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/charset.data.json
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/charset.meta.json
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/contentmanager.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24099 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/errors.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/errors.meta.json
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/header.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/header.meta.json
--rw-r--r--   0        0        0    55947 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/message.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/message.meta.json
--rw-r--r--   0        0        0    31210 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/policy.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/email/policy.meta.json
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/__init__.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/__init__.meta.json
--rw-r--r--   0        0        0    13318 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/collections.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/collections.meta.json
--rw-r--r--   0        0        0   125187 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/dataclasses.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/dataclasses.meta.json
--rw-r--r--   0        0        0    53697 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/diff.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/diff.meta.json
--rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/encoders.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/encoders.meta.json
--rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/exceptions.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/exceptions.meta.json
--rw-r--r--   0        0        0    21311 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/expressions.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/expressions.meta.json
--rw-r--r--   0        0        0    21814 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/finder.data.json
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/finder.meta.json
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/git.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/git.meta.json
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/importer.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/importer.meta.json
--rw-r--r--   0        0        0    29253 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/loader.data.json
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/loader.meta.json
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/logger.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/logger.meta.json
--rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/merger.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/merger.meta.json
--rw-r--r--   0        0        0    16260 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/mixins.data.json
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/mixins.meta.json
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/stats.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/stats.meta.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/__init__.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/__init__.meta.json
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/base.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/base.meta.json
--rw-r--r--   0        0        0    27930 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/inspector.data.json
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/inspector.meta.json
--rw-r--r--   0        0        0   122574 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/nodes.data.json
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/nodes.meta.json
--rw-r--r--   0        0        0    27970 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/visitor.data.json
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/visitor.meta.json
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/extensions/__init__.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/extensions/__init__.meta.json
--rw-r--r--   0        0        0    31543 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/extensions/base.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/agents/extensions/base.meta.json
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/__init__.meta.json
--rw-r--r--   0        0        0    65741 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/dataclasses.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/dataclasses.meta.json
--rw-r--r--   0        0        0    26141 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/google.data.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/google.meta.json
--rw-r--r--   0        0        0    26965 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/numpy.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/numpy.meta.json
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/parsers.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/parsers.meta.json
--rw-r--r--   0        0        0    38471 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/sphinx.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/sphinx.meta.json
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/utils.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/griffe/docstrings/utils.meta.json
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73793 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0        0        0    66425 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/machinery.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/machinery.meta.json
--rw-r--r--   0        0        0    68725 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    16008 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/__init__.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/__init__.meta.json
--rw-r--r--   0        0        0    15054 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/decoder.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/decoder.meta.json
--rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/encoder.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/json/encoder.meta.json
--rw-r--r--   0        0        0   144492 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/logging/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/logging/__init__.meta.json
--rw-r--r--   0        0        0   314876 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine/__about__.py
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine_scuffed/__about__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine_scuffed/__init__.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/carmine_scuffed/__main__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/experiments/__main__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/experiments/cli.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/experiments/filename
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/README.md
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sh40_carmine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__about__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__init__.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/carmine/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/README.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 sh40_carmine-0.2.0/PKG-INFO
```

### Comparing `sh40_carmine-0.1.0/target.py` & `sh40_carmine-0.2.0/carmine/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,74 @@
+"""The Carmine utility."""
+
+from pathlib import Path
+
+from . import Carmine, CLIRuntimeError
+
+TEMPLATE = """\
+\"\"\"My Carmine project.\"\"\"
+
 from carmine import Carmine
 
 
-def command_generate(
-    directory: Path,
-    filename: str = "__main__.py",
+def command_example(name: str, age: int = -1) -> None:
+    \"\"\"Prints out your name and age.
+
+    Args:
+        name: Your name.
+        age: Your age.
+    \"\"\"
+
+    age_text = "I don't know your age." if age == -1 else f"You are {age}."
+
+    print(f"Hello, {name}. {age_text}")
+
+
+def main(argv: list[str] | None = None) -> None:
+    \"\"\"Runs the application.\"\"\"
+
+    with Carmine(__doc__, argv) as cli:
+        cli += command_example
+
+
+if __name__ == "__main__":
+    import sys
+
+    main(sys.argv)
+"""
+
+
+def command_init(
+    filepath: Path,
     force: bool = False,
 ) -> int:
     """Generates a new CLI-runner file to use as a template.
 
     Args:
-        directory: Where the file should be stored.
-        filename: The name of the file.
+        filepath: The path of the generated file.
         force: If set, an already existing file at `<directory>/<filename>` will be
             overwritten.
     """
 
-    if not directory.exists():
-        cli.error(f"Path {str(directory)!r} does not exist.")
-        return 1
-
-    if not directory.is_dir():
-        cli.error(f"Path {str(directory)!r} is not a directory.")
-        return 2
-
-    filepath = directory / filename
-
     if filepath.exists() and not force:
-        cli.error(
+        raise CLIRuntimeError(
             f"File {str(filepath)!r} already exists."
-            + " Overwrite this restriction with --force."
+            + " Overwrite this restriction with '--force'."
         )
-        return 3
 
     with open(filepath, "w") as file:
-        file.write("This is a cool file.")
+        file.write(TEMPLATE)
 
     return 0
 
 
 def main(argv: list[str] | None = None) -> None:
-    """Runs the application.
-
-    Args:
-        argv: A list of command line arguments.
-    """
+    """Runs the application."""
 
     with Carmine(argv) as cli:
-        cli += command_generate
+        cli += command_init
 
 
 if __name__ == "__main__":
-    main()
+    import sys
+
+    main(sys.argv)
```

### Comparing `sh40_carmine-0.1.0/carmine/__init__.py` & `sh40_carmine-0.2.0/carmine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,36 @@
 import re
 from dataclasses import dataclass, field
 from inspect import Signature, signature, cleandoc
 from typing import Any, NamedTuple, TypeVar, Callable, Protocol
 
 from griffe.dataclasses import Docstring
 from griffe.docstrings.parsers import Parser, parse
-from zenith import markup, Palette
+from zenith import zml, Palette
 
 Empty = object()
 
 T = TypeVar("T")
 
 RE_REPR = re.compile(r"[\'|\"](.*?)[\'|\"]")
+RE_CODE = re.compile(r"`(.*?)`")
 
 INDENT = 2 * " "
 
 HELP = """\
 {usage}
 
 {doc}
 
 {options}
 {commands}"""
 
-logging.getLogger("griffe").setLevel(logging.ERROR)
+HELP_MESSAGE = "Prints this message and exits."
 
-Palette.from_hex("#D70040").alias()
+logging.getLogger("griffe").setLevel(logging.ERROR)
 
 
 @dataclass
 class CLIException(Exception):
     """An exception raised during the preparation or execution of a CLI."""
 
     def __init__(self, value: str, code: int = 1) -> None:
@@ -263,21 +264,29 @@
         output += "\n" + commands_text
 
     print(output.rstrip("\n"))
 
 
 @dataclass
 class Carmine:
-    argv: list[str] | None = None
+    module_doc: str
+    argv: list[str] | None
+
     name: str = field(init=False)
     help_printer: HelpPrinter = print_help
 
     _commands: dict[str, Command] = field(init=None, default_factory=dict)
 
     def __post_init__(self) -> None:
+        palette = Palette.from_hex("#D70040")
+        palette.color_mapping = {
+            f"cli.{key}": value for key, value in palette.color_mapping.items()
+        }
+        palette.alias()
+
         if self.argv is None:
             self.argv = sys.argv
 
         self.name = self.argv[0].split("/")[-1]
         self.argv.pop(0)
 
     def __iadd__(self, obj: object) -> Carmine:
@@ -311,33 +320,40 @@
 
         except CLIRuntimeError as exc:
             self.error_and_exit(exc.value, exc.code)
 
     def register(self, command: Callable[..., None]) -> None:
         """Registers a new command."""
 
+        if not hasattr(command, "__doc__"):
+            raise CLIParserError(f"No documentation for `{command.__name__}`.")
+
         schema = _get_schema(command)
         name = command.__name__.removeprefix("command_").replace("_", "-")
 
         docstring = Docstring(command.__doc__, lineno=1)
         parsed = parse(docstring, parser=Parser.google)
 
         description = parsed[0].value
         params = parsed[1].value if len(parsed) > 1 else []
 
         param_doc = {}
         for param in params:
             param_doc[param.name] = " ".join(param.description.splitlines())
 
+            if param.name not in schema:
+                raise CLIParserError(
+                    f"Parameter {param.name!r} not found in signature, but documented."
+                )
             default = schema[param.name][1]
 
             if default is not Empty:
                 param_doc[param.name] += f" Defaults to {default!r}."
 
-        param_doc["help"] = "Prints this message and exits."
+        param_doc["help"] = HELP_MESSAGE
 
         positionals = [key for key, param in schema.items() if param.default is Empty]
 
         options = []
         used_shorthands = []
 
         for key, param in schema.items():
@@ -390,22 +406,35 @@
             command(**args)
 
         self._commands[name] = Command(description, _execute)
 
     def error_and_exit(self, content: str, code: int) -> None:
         """Prints out `content` and exits with given the status code."""
 
-        content = RE_REPR.sub(r"[success]'\1'[/fg]", content)
-        print(markup(f"[error bold]Error:[/] {content}"))
+        content = RE_REPR.sub(r"[cli.success]'\1'[/fg]", content)
+        content = RE_CODE.sub(r"[@#212121 grey]\1[/]", content)
+        print(zml(f"[cli.error bold]Error:[/] {content}"))
 
         sys.exit(code)
 
     def run(self) -> None:
         """Runs the CLI."""
 
         command = "command" if self.argv in ([], ["-h"], ["--help"]) else self.argv[0]
 
+        if self.argv in ([], ["-h"], ["--help"]):
+            commands = {cmd_name: cmd.doc for cmd_name, cmd in self._commands.items()}
+
+            self.help_printer(
+                exec_line=self.name,
+                documentation=cleandoc(self.module_doc).splitlines(),
+                options=[("help", "h", bool, HELP_MESSAGE)],
+                positionals=[],
+                commands=commands,
+            )
+            return
+
         if command not in self._commands:
             raise CLIRuntimeError(f"Unknown command {command!r}.")
 
         self._command = command
         self._commands[command](self.argv[1:])
```

### Comparing `sh40_carmine-0.1.0/LICENSE.txt` & `sh40_carmine-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_carmine-0.1.0/pyproject.toml` & `sh40_carmine-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 Documentation = "https://github.com/shade40/carmine#readme"
 Issues = "https://github.com/shade40/carmine/issues"
 Source = "https://github.com/shade40/carmine"
 
 [project.scripts]
 carmine = "carmine.__main__:main"
 
+[tool.hatch.build]
+include = [
+  "carmine/*.py",
+  "/tests",
+]
+
 [tool.hatch.version]
 path = "carmine/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
```

### Comparing `sh40_carmine-0.1.0/PKG-INFO` & `sh40_carmine-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-carmine
-Version: 0.1.0
+Version: 0.2.0
 Summary: A dynamic CLI generator utilizing Python function signatures.
 Project-URL: Documentation, https://github.com/shade40/carmine#readme
 Project-URL: Issues, https://github.com/shade40/carmine/issues
 Project-URL: Source, https://github.com/shade40/carmine
 Author-email: bczsalba <bczsalba@gmail.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 ![carmine](https://singlecolorimage.com/get/D70040/1600x200)
 
 ## carmine
 
 A dynamic CLI generator utilizing Python function signatures.
 
 ```
-pip install carmine
+pip install sh40-carmine
 ```
 
 ![rule](https://singlecolorimage.com/get/D70040/1600x5)
 
 ### Purpose
 
 ![rule](https://singlecolorimage.com/get/D70040/1600x5)
```

