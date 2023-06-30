# Comparing `tmp/tarantool-1.0.0.tar.gz` & `tmp/tarantool-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarantool-1.0.0.tar", last modified: Mon Apr 17 11:04:13 2023, max compression
+gzip compressed data, was "tarantool-1.1.0.tar", last modified: Fri Jun 30 09:38:46 2023, max compression
```

## Comparing `tarantool-1.0.0.tar` & `tarantool-1.1.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.290784 tarantool-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-17 11:03:59.000000 tarantool-1.0.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-17 11:03:59.000000 tarantool-1.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/scripts/remove_source_code.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)    15987 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/packing.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/reusable_testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12676 2023-04-17 11:03:59.000000 tarantool-1.0.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-17 11:03:59.000000 tarantool-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-17 11:03:59.000000 tarantool-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-17 11:03:59.000000 tarantool-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-17 11:03:59.000000 tarantool-1.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    14512 2023-04-17 11:03:59.000000 tarantool-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-04-17 11:03:59.000000 tarantool-1.0.0/INSTALL
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-04-17 11:03:59.000000 tarantool-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-17 11:03:59.000000 tarantool-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-04-17 11:03:59.000000 tarantool-1.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-04-17 11:04:13.290784 tarantool-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-04-17 11:03:59.000000 tarantool-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-17 11:03:59.000000 tarantool-1.0.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/debian/
--rw-r--r--   0 runner    (1001) docker     (122)    27362 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/compat
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (122)      517 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/debian/source/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-17 11:03:59.000000 tarantool-1.0.0/debian/source/options
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.274784 tarantool-1.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/docs/source/_static/favicon/
--rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (122)    14138 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (122)     5571 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-76x76.png
--rwxr-xr-x   0 runner    (1001) docker     (122)      266 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/generate-png.sh
--rw-r--r--   0 runner    (1001) docker     (122)    11989 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (122)    21876 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-196x196.png
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     7747 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/_static/favicon/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/module-tarantool.rst
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-connection-pool.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-connection.rst
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-crud.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-dbapi.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-error.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-mesh-connection.rst
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-msgpack-ext-types.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-msgpack-ext.rst
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-request.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-response.rst
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-schema.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-space.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-types.rst
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/api/submodule-utils.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10929 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/dev-guide.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    14953 2023-04-17 11:03:59.000000 tarantool-1.0.0/docs/source/quick-start.rst
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-17 11:03:59.000000 tarantool-1.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-17 11:03:59.000000 tarantool-1.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.270784 tarantool-1.0.0/rpm/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.278784 tarantool-1.0.0/rpm/SPECS/
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-04-17 11:03:59.000000 tarantool-1.0.0/rpm/SPECS/python-tarantool.spec
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 11:04:13.290784 tarantool-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     3136 2023-04-17 11:03:59.000000 tarantool-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/
--rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   103863 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    56825 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/crud.py
--rw-r--r--   0 runner    (1001) docker     (122)    12894 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    20552 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/error.py
--rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/mesh_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     9985 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/interval.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/packer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/types/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26728 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     6527 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2254 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh
--rw-r--r--   0 runner    (1001) docker     (122)    48588 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/timezones.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/unpacker.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/msgpack_ext/uuid.py
--rw-r--r--   0 runner    (1001) docker     (122)    17713 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/request.py
--rw-r--r--   0 runner    (1001) docker     (122)    10967 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/response.py
--rw-r--r--   0 runner    (1001) docker     (122)    13804 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/space.py
--rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-04-17 11:03:59.000000 tarantool-1.0.0/tarantool/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/tarantool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 11:04:13.000000 tarantool-1.0.0/tarantool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.282784 tarantool-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.286784 tarantool-1.0.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/ca.crt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/empty
--rwxr-xr-x   0 runner    (1001) docker     (122)     1702 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/generate.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/invalidhost.crt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/invalidpasswords
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.crt
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.enc.key
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/localhost.key
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/data/passwords
--rwxr-xr-x   0 runner    (1001) docker     (122)     1176 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/setup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.286784 tarantool-1.0.0/test/suites/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/box.lua
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/crud_server.lua
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 11:04:13.290784 tarantool-1.0.0/test/suites/lib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/remote_tarantool_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     8386 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/skip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_python_ci.lua
--rw-r--r--   0 runner    (1001) docker     (122)    11116 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/lib/tarantool_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (122)    30406 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     4218 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_dbapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    18278 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)    19641 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_dml.py
--rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_error_ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)     8583 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_reconnect.py
--rw-r--r--   0 runner    (1001) docker     (122)    25356 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    33077 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-04-17 11:03:59.000000 tarantool-1.0.0/test/suites/test_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-30 09:38:29.000000 tarantool-1.1.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-30 09:38:29.000000 tarantool-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/scripts/remove_source_code.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)    15987 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/packing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/reusable_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12038 2023-06-30 09:38:29.000000 tarantool-1.1.0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-30 09:38:29.000000 tarantool-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-06-30 09:38:29.000000 tarantool-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-30 09:38:29.000000 tarantool-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-30 09:38:29.000000 tarantool-1.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-30 09:38:29.000000 tarantool-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-06-30 09:38:29.000000 tarantool-1.1.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-06-30 09:38:29.000000 tarantool-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-30 09:38:29.000000 tarantool-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-06-30 09:38:29.000000 tarantool-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-06-30 09:38:46.814899 tarantool-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-06-30 09:38:29.000000 tarantool-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-30 09:38:29.000000 tarantool-1.1.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)    27953 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (122)      517 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-30 09:38:29.000000 tarantool-1.1.0/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.794899 tarantool-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.798899 tarantool-1.1.0/docs/source/_static/favicon/
+-rw-r--r--   0 runner    (1001) docker     (122)    10003 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10722 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14138 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3743 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5571 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-76x76.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)      266 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/generate-png.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    11989 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21876 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-196x196.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7747 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/_static/favicon/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.802899 tarantool-1.1.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/module-tarantool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-connection-pool.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-crud.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-dbapi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-error.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-mesh-connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-msgpack-ext-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-msgpack-ext.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-request.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-response.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-schema.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-space.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/api/submodule-utils.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10929 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14953 2023-06-30 09:38:29.000000 tarantool-1.1.0/docs/source/quick-start.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-30 09:38:29.000000 tarantool-1.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-30 09:38:29.000000 tarantool-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.790899 tarantool-1.1.0/rpm/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.802899 tarantool-1.1.0/rpm/SPECS/
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-06-30 09:38:29.000000 tarantool-1.1.0/rpm/SPECS/python-tarantool.spec
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 09:38:46.814899 tarantool-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3136 2023-06-30 09:38:29.000000 tarantool-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/
+-rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105958 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56825 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12894 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20552 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/mesh_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5279 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10336 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/packer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/types/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26310 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6527 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2254 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    48588 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/unpacker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/msgpack_ext/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17713 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10967 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13804 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/space.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-06-30 09:38:29.000000 tarantool-1.1.0/tarantool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.806899 tarantool-1.1.0/tarantool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5549 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-30 09:38:46.000000 tarantool-1.1.0/tarantool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.810899 tarantool-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.810899 tarantool-1.1.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/ca.crt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/empty
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1702 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/generate.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/invalidhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/invalidpasswords
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.enc.key
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/localhost.key
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/data/passwords
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1176 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/setup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/test/suites/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/box.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     2580 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/crud_server.lua
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:46.814899 tarantool-1.1.0/test/suites/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3363 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/remote_tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9432 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/skip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_python_ci.lua
+-rw-r--r--   0 runner    (1001) docker     (122)    11383 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/lib/tarantool_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30563 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19668 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19641 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_dml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7419 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_error_ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20214 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6153 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8583 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_reconnect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26049 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33077 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-06-30 09:38:29.000000 tarantool-1.1.0/test/suites/test_uuid.py
```

### Comparing `tarantool-1.0.0/.github/workflows/packing.yml` & `tarantool-1.1.0/.github/workflows/packing.yml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         # Checkout all tags for correct version computation.
         with:
           fetch-depth: 0
 
       - name: Setup Python and basic packing tools
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
 
       - name: Install tools for packing and verification
         run: pip3 install wheel twine
 
       - name: Pack source and binary files
         run: make pip-dist
 
@@ -69,23 +69,23 @@
     steps:
       - name: Clone the connector repo
         uses: actions/checkout@v3
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
 
       - name: Remove connector source code
         run: python3 .github/scripts/remove_source_code.py
 
       - name: Install tarantool
         uses: tarantool/setup-tarantool@v2
         with:
-          tarantool-version: '2.10'
+          tarantool-version: '2.11'
 
       - name: Download pip package artifacts
         uses: actions/download-artifact@v3
         with:
           name: pip_dist
           path: pip_dist
 
@@ -124,15 +124,15 @@
     steps:
       - name: Clone the connector repo
         uses: actions/checkout@v3
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
 
       - name: Remove connector source code
         run: python3 .github/scripts/remove_source_code.py
 
       - name: Download pip package artifacts
         uses: actions/download-artifact@v3
         with:
@@ -192,15 +192,15 @@
     steps:
       - name: Clone the connector repo
         uses: actions/checkout@v3
 
       - name: Setup Python and basic packing tools
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
 
       - name: Install tools for package publishing
         run: pip3 install twine
 
       - name: Download pip package artifacts
         uses: actions/download-artifact@v3
         with:
```

### Comparing `tarantool-1.0.0/.github/workflows/reusable_testing.yml` & `tarantool-1.1.0/.github/workflows/reusable_testing.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         # Now we're lucky: all dependencies are already installed. Check package
         # dependencies when migrating to other OS version.
         run: sudo dpkg -i tarantool*.deb
 
       - name: Setup python3 for tests
         uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: '3.11'
 
       - name: Install connector requirements
         run: pip3 install -r requirements.txt
 
       - name: Install test requirements
         run: pip3 install -r requirements-test.txt
```

### Comparing `tarantool-1.0.0/.github/workflows/testing.yml` & `tarantool-1.1.0/.github/workflows/testing.yml`

 * *Files 3% similar despite different names*

```diff
@@ -22,40 +22,39 @@
     strategy:
       fail-fast: false
       matrix:
         tarantool:
           - '1.10'
           - '2.8'
           - '2.10'
+          - '2.11'
         python:
           - '3.6'
           - '3.7'
           - '3.8'
           - '3.9'
           - '3.10'
+          - '3.11'
         msgpack-deps:
           # latest msgpack will be installed as a part of requirements.txt
           - ''
 
         # Adding too many elements to three-dimentional matrix results in
         # too many test cases. It causes GitHub webpages to fail with
         # "This page is taking too long to load." error. Thus we use
         # pairwise testing.
         include:
-          - tarantool: '2.8'
-            python: '3.10'
-            msgpack-deps: 'msgpack-python==0.4.0'
-          - tarantool: '2.8'
-            python: '3.10'
+          - tarantool: '2.11'
+            python: '3.11'
             msgpack-deps: 'msgpack==0.5.0'
-          - tarantool: '2.8'
-            python: '3.10'
+          - tarantool: '2.11'
+            python: '3.11'
             msgpack-deps: 'msgpack==0.6.2'
-          - tarantool: '2.8'
-            python: '3.10'
+          - tarantool: '2.11'
+            python: '3.11'
             msgpack-deps: 'msgpack==1.0.4'
 
     steps:
       - name: Clone the connector
         uses: actions/checkout@v3
 
       - name: Install tarantool ${{ matrix.tarantool }}
@@ -109,23 +108,23 @@
 
     runs-on: ubuntu-20.04
 
     strategy:
       fail-fast: false
       matrix:
         tarantool:
-          - bundle: 'bundle-1.10.11-0-gf0b0e7ecf-r470'
-            path: ''
-          - bundle: 'bundle-2.8.3-21-g7d35cd2be-r470'
-            path: ''
-          - bundle: 'bundle-2.10.0-1-gfa775b383-r486-linux-x86_64'
-            path: ''
-          - bundle: 'sdk-gc64-2.11.0-entrypoint-113-g803baaffe-r529.linux.x86_64'
-            path: 'dev/linux/x86_64/master/'
-        python: ['3.6', '3.7', '3.8', '3.9', '3.10']
+          - bundle: 'sdk-1.10.15-0-r563'
+            path: 'release/linux/x86_64/1.10/'
+          - bundle: 'sdk-2.8.4-0-r563'
+            path: 'release/linux/x86_64/2.8/'
+          - bundle: 'sdk-gc64-2.10.7-0-r563.linux.x86_64'
+            path: 'release/linux/x86_64/2.10/'
+          - bundle: 'sdk-gc64-2.11.0-0-r563.linux.x86_64'
+            path: 'release/linux/x86_64/2.11/'
+        python: ['3.6', '3.11']
 
     steps:
       - name: Clone the connector
         # `ref` as merge request is needed for pull_request_target because this
         # target runs in the context of the base commit of the pull request.
         uses: actions/checkout@v3
         if: github.event_name == 'pull_request_target'
@@ -164,16 +163,16 @@
           tt rocks install crud TARANTOOL_DIR=$PWD/tarantool-enterprise
 
       - name: Run tests
         run: |
           source tarantool-enterprise/env.sh
           make test
         env:
-          TEST_TNT_SSL: ${{ matrix.tarantool.bundle == 'bundle-2.10.0-1-gfa775b383-r486-linux-x86_64' ||
-                            matrix.tarantool.bundle == 'sdk-gc64-2.11.0-entrypoint-113-g803baaffe-r529.linux.x86_64'}}
+          TEST_TNT_SSL: ${{ matrix.tarantool.bundle == 'sdk-gc64-2.10.7-0-r563.linux.x86_64' ||
+                            matrix.tarantool.bundle == 'sdk-gc64-2.11.0-0-r563.linux.x86_64'}}
 
   run_tests_pip_branch_install_linux:
     # We want to run on external PRs, but not on our own internal
     # PRs as they'll be run by the push to the branch.
     #
     # The main trick is described here:
     # https://github.com/Dart-Code/Dart-Code/pull/2375
@@ -183,21 +182,18 @@
     runs-on: ubuntu-20.04
 
     strategy:
       fail-fast: false
 
       matrix:
         tarantool:
-          - '2.10'
+          - '2.11'
         python:
           - '3.6'
-          - '3.7'
-          - '3.8'
-          - '3.9'
-          - '3.10'
+          - '3.11'
     steps:
       - name: Clone the connector repo
         uses: actions/checkout@v3
 
       - name: Install tarantool ${{ matrix.tarantool }}
         uses: tarantool/setup-tarantool@v2
         with:
@@ -239,20 +235,18 @@
     runs-on: windows-2022
 
     strategy:
       fail-fast: false
       matrix:
         # Use reduced test matrix cause Windows pipelines are long.
         tarantool:
-          - '1.10'
-          - '2.8'
-          - '2.10.0.g0a5ce0b9c-1'
+          - '2.11.0.g247a9a418-1'
         python:
           - '3.6'
-          - '3.10'
+          - '3.11'
 
     steps:
       - name: Clone the connector
         uses: actions/checkout@v3
 
       - name: Setup Python for tests
         uses: actions/setup-python@v4
@@ -266,23 +260,15 @@
         run: pip3 install -r requirements-test.txt
 
       - name: Setup WSL for tarantool
         uses: Vampire/setup-wsl@v2
         with:
           distribution: Ubuntu-20.04
 
-      - name: Install tarantool ${{ matrix.tarantool }} for WSL (2.8 and older)
-        if: (matrix.tarantool == '1.10') || (matrix.tarantool == '2.8')
-        shell: wsl-bash_Ubuntu-20.04 {0}
-        run: |
-          curl -L https://tarantool.io/installer.sh | VER=${{ matrix.tarantool }} bash -s -- --type "release"
-          sudo apt install -y tarantool tarantool-dev
-
       - name: Install tarantool ${{ matrix.tarantool }} for WSL (2.10 and newer)
-        if: (matrix.tarantool != '1.10') && (matrix.tarantool != '2.8')
         shell: wsl-bash_Ubuntu-20.04 {0}
         run: |
           curl -L https://tarantool.io/release/2/installer.sh | bash -s
           sudo apt install -y tarantool=${{ matrix.tarantool }} tarantool-dev=${{ matrix.tarantool }}
 
       - name: Setup test tarantool instance
         shell: wsl-bash_Ubuntu-20.04 {0}
@@ -319,18 +305,18 @@
 
     strategy:
       fail-fast: false
 
       matrix:
         # Use reduced test matrix cause Windows pipelines are long.
         tarantool:
-          - '2.10.0.g0a5ce0b9c-1'
+          - '2.11.0.g247a9a418-1'
         python:
           - '3.6'
-          - '3.10'
+          - '3.11'
     steps:
       - name: Clone the connector repo
         uses: actions/checkout@v3
 
       - name: Setup Python for tests
         uses: actions/setup-python@v4
         with:
```

### Comparing `tarantool-1.0.0/.gitignore` & `tarantool-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/AUTHORS` & `tarantool-1.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/CHANGELOG.md` & `tarantool-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.0 - 2023-06-30
+
+### Added
+- Allow to require specific server protocol version and features (#267).
+
+### Changed
+- Drop `msgpack-python` support. Use `msgpack` instead.
+
+### Fixed
+- Parsing of E-notation Tarantool decimals with positive exponent (PR #298).
+
 ## 1.0.0 - 2023-04-17
 
 ### Changed
 - **Breaking**: Allow only named `on_push` and `on_push_ctx` for `insert` and `replace`.
 - Migrate to built-in `Warning` instead of a custom one.
 - Migrate to built-in `RecursionError` instead of a custom one.
 - Collect full exception traceback.
```

### Comparing `tarantool-1.0.0/LICENSE` & `tarantool-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/Makefile` & `tarantool-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/PKG-INFO` & `tarantool-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarantool
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client library for Tarantool
 Home-page: https://github.com/tarantool/tarantool-python
 Author: tarantool-python AUTHORS
 Author-email: admin@tarantool.org
 License: BSD
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `tarantool-1.0.0/README.rst` & `tarantool-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/debian/changelog` & `tarantool-1.1.0/debian/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+python3-tarantool (1.1.0-0) unstable; urgency=medium
+
+    ## Overview
+
+    This release introduces API to request server protocol version and
+    feature, as well as introduce decimal bugfix.
+
+    ## Breaking changes
+
+    - Drop `msgpack-python` support. (Package not supported since 2019.)
+      Use `msgpack` instead.
+
+    ## Added
+    - Allow to require specific server protocol version and features (#267).
+
+    ## Fixed
+    - Parsing of E-notation Tarantool decimals with positive exponent (PR #298).
+
+ -- Georgy Moiseev <georgy.moiseev@tarantool.org>  Fri, 30 Jun 2023 10:00:00 +0300
+
 python3-tarantool (1.0.0-0) unstable; urgency=medium
 
     ## Overview
 
     This release introduces several minor behavior changes
     to make API more consistent.
 
@@ -24,15 +44,15 @@
     - Collect full exception traceback.
     - Package no longer depends on `pandas` (#290).
 
     ## Infrastructure
 
     - Lint the code with `pylint`, `flake8` and `codespell`.
 
- -- Georgy.moiseev <georgy.moiseev@tarantool.org>  Mon, 17 Apr 2023 13:00:00 +0300
+ -- Georgy Moiseev <georgy.moiseev@tarantool.org>  Mon, 17 Apr 2023 13:00:00 +0300
 
 python3-tarantool (0.12.1-0) unstable; urgency=medium
 
     ## Overview
 
     This release introduces several bugfixes and behavior improvements.
```

### Comparing `tarantool-1.0.0/debian/control` & `tarantool-1.1.0/debian/control`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/debian/rules` & `tarantool-1.1.0/debian/rules`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-114x114.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-120x120.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-144x144.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-152x152.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-57x57.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-60x60.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-72x72.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/apple-touch-icon-76x76.png` & `tarantool-1.1.0/docs/source/_static/favicon/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon-128x128.png` & `tarantool-1.1.0/docs/source/_static/favicon/icon-128x128.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon-16x16.png` & `tarantool-1.1.0/docs/source/_static/favicon/icon-16x16.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon-196x196.png` & `tarantool-1.1.0/docs/source/_static/favicon/icon-196x196.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon-32x32.png` & `tarantool-1.1.0/docs/source/_static/favicon/icon-32x32.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon-96x96.png` & `tarantool-1.1.0/docs/source/_static/favicon/icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/_static/favicon/icon.svg` & `tarantool-1.1.0/docs/source/_static/favicon/icon.svg`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/api/module-tarantool.rst` & `tarantool-1.1.0/docs/source/api/module-tarantool.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/api/submodule-connection.rst` & `tarantool-1.1.0/docs/source/api/submodule-connection.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/api/submodule-mesh-connection.rst` & `tarantool-1.1.0/docs/source/api/submodule-mesh-connection.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/api/submodule-msgpack-ext-types.rst` & `tarantool-1.1.0/docs/source/api/submodule-msgpack-ext-types.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/api/submodule-msgpack-ext.rst` & `tarantool-1.1.0/docs/source/api/submodule-msgpack-ext.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/conf.py` & `tarantool-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/dev-guide.rst` & `tarantool-1.1.0/docs/source/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/index.rst` & `tarantool-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/docs/source/quick-start.rst` & `tarantool-1.1.0/docs/source/quick-start.rst`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/rpm/SPECS/python-tarantool.spec` & `tarantool-1.1.0/rpm/SPECS/python-tarantool.spec`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/setup.py` & `tarantool-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/__init__.py` & `tarantool-1.1.0/tarantool/__init__.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/connection.py` & `tarantool-1.1.0/tarantool/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import sys
 import abc
 
 import ctypes
 import ctypes.util
 from ctypes import c_ssize_t
 from typing import Optional, Union
+from copy import copy
 
 import msgpack
 
 from tarantool.response import (
     unpacker_factory as default_unpacker_factory,
 )
 from tarantool.request import (
@@ -61,14 +62,17 @@
     ITERATOR_ALL,
     CONNECTOR_IPROTO_VERSION,
     CONNECTOR_FEATURES,
     IPROTO_FEATURE_STREAMS,
     IPROTO_FEATURE_TRANSACTIONS,
     IPROTO_FEATURE_ERROR_EXTENSION,
     IPROTO_FEATURE_WATCHERS,
+    IPROTO_FEATURE_PAGINATION,
+    IPROTO_FEATURE_SPACE_AND_INDEX_NAMES,
+    IPROTO_FEATURE_WATCH_ONCE,
     IPROTO_CHUNK,
     AUTH_TYPE_CHAP_SHA1,
     AUTH_TYPE_PAP_SHA256,
     AUTH_TYPES,
 )
 from tarantool.error import (
     Error,
@@ -603,15 +607,17 @@
                  ssl_ca_file=DEFAULT_SSL_CA_FILE,
                  ssl_ciphers=DEFAULT_SSL_CIPHERS,
                  ssl_password=DEFAULT_SSL_PASSWORD,
                  ssl_password_file=DEFAULT_SSL_PASSWORD_FILE,
                  packer_factory=default_packer_factory,
                  unpacker_factory=default_unpacker_factory,
                  auth_type=None,
-                 fetch_schema=True):
+                 fetch_schema=True,
+                 required_protocol_version=None,
+                 required_features=None):
         """
         :param host: Server hostname or IP address. Use ``None`` for
             Unix sockets.
         :type host: :obj:`str` or :obj:`None`
 
         :param port: Server port or Unix socket path.
         :type port: :obj:`int` or :obj:`str`
@@ -772,23 +778,31 @@
             :meth:`~tarantool.Connection.delete`,
             :meth:`~tarantool.Connection.upsert`,
             :meth:`~tarantool.Connection.update`,
             :meth:`~tarantool.Connection.select`,
             :meth:`~tarantool.Connection.space`.
         :type fetch_schema: :obj:`bool`, optional
 
+        :param required_protocol_version: Minimal protocol version that
+            should be supported by Tarantool server.
+        :type required_protocol_version: :obj:`int` or :obj:`None`, optional
+
+        :param required_features: List of protocol features that
+            should be supported by Tarantool server.
+        :type required_features: :obj:`list` or :obj:`None`, optional
+
         :raise: :exc:`~tarantool.error.ConfigurationError`,
             :meth:`~tarantool.Connection.connect` exceptions
 
         .. _socket.settimeout(): https://docs.python.org/3/library/socket.html#socket.socket.settimeout
         .. _mp_str: https://github.com/msgpack/msgpack/blob/master/spec.md#str-format-family
         .. _mp_bin: https://github.com/msgpack/msgpack/blob/master/spec.md#bin-format-family
         .. _mp_array: https://github.com/msgpack/msgpack/blob/master/spec.md#array-format-family
         """
-        # pylint: disable=too-many-arguments,too-many-locals
+        # pylint: disable=too-many-arguments,too-many-locals,too-many-statements
 
         if msgpack.version >= (1, 0, 0) and encoding not in (None, 'utf-8'):
             raise ConfigurationError("msgpack>=1.0.0 only supports None and "
                                      + "'utf-8' encoding option values")
 
         if os.name == 'nt':
             libc = ctypes.WinDLL(
@@ -826,22 +840,31 @@
         self.ssl_password_file = ssl_password_file
         self._protocol_version = None
         self._features = {
             IPROTO_FEATURE_STREAMS: False,
             IPROTO_FEATURE_TRANSACTIONS: False,
             IPROTO_FEATURE_ERROR_EXTENSION: False,
             IPROTO_FEATURE_WATCHERS: False,
+            IPROTO_FEATURE_PAGINATION: False,
+            IPROTO_FEATURE_SPACE_AND_INDEX_NAMES: False,
+            IPROTO_FEATURE_WATCH_ONCE: False,
         }
         self._packer_factory_impl = packer_factory
         self._unpacker_factory_impl = unpacker_factory
         self._client_auth_type = auth_type
         self._server_auth_type = None
         self.version_id = None
         self.uuid = None
         self._salt = None
+        self._client_protocol_version = CONNECTOR_IPROTO_VERSION
+        self._client_features = copy(CONNECTOR_FEATURES)
+        self._server_protocol_version = None
+        self._server_features = None
+        self.required_protocol_version = required_protocol_version
+        self.required_features = copy(required_features)
 
         if connect_now:
             self.connect()
 
     def close(self):
         """
         Close a connection to the server. The method is idempotent.
@@ -1040,18 +1063,19 @@
         """
 
         greeting_buf = self._recv(IPROTO_GREETING_SIZE)
         greeting = greeting_decode(greeting_buf)
         if greeting.protocol != "Binary":
             raise NetworkError("Unsupported protocol: " + greeting.protocol)
         self.version_id = greeting.version_id
-        if self.version_id >= version_id(2, 10, 0):
-            self._check_features()
         self.uuid = greeting.uuid
         self._salt = greeting.salt
+
+        self._check_features()
+
         if self.user:
             self.authenticate(self.user, self.password)
 
     def connect(self):
         """
         Create a connection to the host and port specified on
         initialization. There is no need to call this method explicitly
@@ -2053,40 +2077,55 @@
         :raise: :exc:`~AssertionError`,
             :exc:`~tarantool.error.DatabaseError`,
             :exc:`~tarantool.error.SchemaError`,
             :exc:`~tarantool.error.NetworkError`,
             :exc:`~tarantool.error.SslError`
         """
 
-        try:
-            request = RequestProtocolVersion(self,
-                                             CONNECTOR_IPROTO_VERSION,
-                                             CONNECTOR_FEATURES)
-            response = self._send_request(request)
-            server_protocol_version = response.protocol_version
-            server_features = response.features
-            server_auth_type = response.auth_type
-        except DatabaseError as exc:
-            if exc.code == ER_UNKNOWN_REQUEST_TYPE:
-                server_protocol_version = None
-                server_features = []
-                server_auth_type = None
+        if self.version_id >= version_id(2, 10, 0):
+            try:
+                request = RequestProtocolVersion(self,
+                                                 self._client_protocol_version,
+                                                 self._client_features)
+                response = self._send_request(request)
+                self._server_protocol_version = response.protocol_version
+                self._server_features = response.features
+                self._server_auth_type = response.auth_type
+            except DatabaseError as exc:
+                if exc.code != ER_UNKNOWN_REQUEST_TYPE:
+                    raise exc
+
+        if self.required_protocol_version is not None:
+            if self._server_protocol_version is None or \
+                    self._server_protocol_version < self.required_protocol_version:
+                raise ConfigurationError('Server protocol version is '
+                                         f'{self._server_protocol_version}, '
+                                         f'protocol version {self.required_protocol_version} '
+                                         'is required')
+
+        if self.required_features is not None:
+            if self._server_features is None:
+                failed_features = self.required_features
             else:
-                raise exc
+                failed_features = [val for val in self.required_features
+                                   if val not in self._server_features]
 
-        if server_protocol_version is not None:
-            self._protocol_version = min(server_protocol_version,
-                                         CONNECTOR_IPROTO_VERSION)
+            if len(failed_features) > 0:
+                str_features = ', '.join([str(v) for v in failed_features])
+                raise ConfigurationError(f'Server missing protocol features with id {str_features}')
+
+        if self._server_protocol_version is not None:
+            self._protocol_version = min(self._server_protocol_version,
+                                         self._client_protocol_version)
 
         # Intercept lists of features
-        features_list = [val for val in CONNECTOR_FEATURES if val in server_features]
-        for val in features_list:
-            self._features[val] = True
-
-        self._server_auth_type = server_auth_type
+        if self._server_features is not None:
+            features_list = [val for val in self._client_features if val in self._server_features]
+            for val in features_list:
+                self._features[val] = True
 
     def _packer_factory(self):
         return self._packer_factory_impl(self)
 
     def _unpacker_factory(self):
         return self._unpacker_factory_impl(self)
```

### Comparing `tarantool-1.0.0/tarantool/connection_pool.py` & `tarantool-1.1.0/tarantool/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/const.py` & `tarantool-1.1.0/tarantool/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 ITERATOR_OVERLAPS = 10
 ITERATOR_NEIGHBOR = 11
 
 IPROTO_FEATURE_STREAMS = 0
 IPROTO_FEATURE_TRANSACTIONS = 1
 IPROTO_FEATURE_ERROR_EXTENSION = 2
 IPROTO_FEATURE_WATCHERS = 3
+IPROTO_FEATURE_PAGINATION = 4
+IPROTO_FEATURE_SPACE_AND_INDEX_NAMES = 5
+IPROTO_FEATURE_WATCH_ONCE = 6
 
 # Default value for connection timeout (seconds)
 CONNECTION_TIMEOUT = None
 # Default value for socket timeout (seconds)
 SOCKET_TIMEOUT = None
 # Default maximum number of attempts to reconnect
 RECONNECT_MAX_ATTEMPTS = 10
@@ -129,16 +132,16 @@
 # Default cluster nodes state refresh interval (seconds)
 POOL_REFRESH_DELAY = 1
 # Default maximum number of attempts to reconnect for pool instance
 POOL_INSTANCE_RECONNECT_MAX_ATTEMPTS = 0
 # Default delay between attempts to reconnect (seconds)
 POOL_INSTANCE_RECONNECT_DELAY = 0
 
-# Tarantool 2.10 protocol version is 3
-CONNECTOR_IPROTO_VERSION = 3
+# Tarantool master 970ea48 protocol version is 6
+CONNECTOR_IPROTO_VERSION = 6
 # List of connector-supported features
 CONNECTOR_FEATURES = [IPROTO_FEATURE_ERROR_EXTENSION]
 
 # Authenticate with CHAP-SHA1 (Tarantool CE and EE)
 AUTH_TYPE_CHAP_SHA1 = "chap-sha1"
 # Authenticate with PAP-SHA256 (Tarantool EE)
 AUTH_TYPE_PAP_SHA256 = "pap-sha256"
```

### Comparing `tarantool-1.0.0/tarantool/crud.py` & `tarantool-1.1.0/tarantool/crud.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/dbapi.py` & `tarantool-1.1.0/tarantool/dbapi.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/error.py` & `tarantool-1.1.0/tarantool/error.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/mesh_connection.py` & `tarantool-1.1.0/tarantool/mesh_connection.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/datetime.py` & `tarantool-1.1.0/tarantool/msgpack_ext/datetime.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/decimal.py` & `tarantool-1.1.0/tarantool/msgpack_ext/decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 .. _decimal: https://www.tarantool.io/en/doc/latest/dev_guide/internals/msgpack_extensions/#the-decimal-type
 .. _mp_int:
 .. _mp_uint: https://github.com/msgpack/msgpack/blob/master/spec.md#int-format-family
 """
 
 from decimal import Decimal
 
+import msgpack
+
 from tarantool.error import MsgpackError, MsgpackWarning, warn
 
 EXT_ID = 1
 """
 `decimal`_ type id.
 """
 
@@ -349,29 +351,40 @@
 
     :return: Decoded decimal.
     :rtype: :obj:`decimal.Decimal`
 
     :raise: :exc:`~tarantool.error.MsgpackError`
     """
 
-    scale = data[0]
+    # A decimal starts with mp_int or mp_uint followed by raw bytes.
+    unpacker = msgpack.Unpacker()
+    unpacker.feed(data)
+
+    scale = unpacker.unpack()
+    scale_size = unpacker.tell()
 
     sign = get_str_sign(data[-1] & 0x0f)
 
     # Parse from tail since scale is counted from the tail.
     digits_reverted = []
 
     add_str_digit(data[-1] >> 4, digits_reverted, scale)
 
-    for i in range(len(data) - 2, 0, -1):
+    for i in range(len(data) - 2, scale_size - 1, -1):
         add_str_digit(data[i] & 0x0f, digits_reverted, scale)
         add_str_digit(data[i] >> 4, digits_reverted, scale)
 
     # Add leading zeroes in case of 0.000... number
     for i in range(len(digits_reverted), scale + 1):
         add_str_digit(0, digits_reverted, scale)
 
     digits_reverted.append(sign)
 
-    str_repr = ''.join(digits_reverted[::-1])
+    digits = digits_reverted[::-1]
+
+    # Add trailing zeroes in case of a negative scale
+    for i in range(0, -1 * scale):
+        add_str_digit(0, digits, scale)
+
+    str_repr = ''.join(digits)
 
     return Decimal(str_repr)
```

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/error.py` & `tarantool-1.1.0/tarantool/msgpack_ext/error.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/interval.py` & `tarantool-1.1.0/tarantool/msgpack_ext/interval.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/packer.py` & `tarantool-1.1.0/tarantool/msgpack_ext/packer.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/types/datetime.py` & `tarantool-1.1.0/tarantool/msgpack_ext/types/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,26 +528,14 @@
         :raise: :exc:`TypeError`
         """
 
         if isinstance(other, Datetime):
             self_dt = self._datetime
             other_dt = other._datetime
 
-            # Tarantool datetime subtraction ignores timezone info, but it is a bug:
-            #
-            # Tarantool 2.10.1-0-g482d91c66
-            #
-            # tarantool> datetime.new{tz='MSK'} - datetime.new{tz='UTC'}
-            # ---
-            # - +0 seconds
-            # ...
-            #
-            # Refer to https://github.com/tarantool/tarantool/issues/7698
-            # for possible updates.
-
             if self_dt.tzinfo != other_dt.tzinfo:
                 other_dt = other_dt.astimezone(self_dt.tzinfo)
 
             self_nsec = self_dt.microsecond * NSEC_IN_MKSEC + self._datetime_nsec
             other_nsec = other_dt.microsecond * NSEC_IN_MKSEC + other._datetime_nsec
 
             return Interval(
```

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/types/interval.py` & `tarantool-1.1.0/tarantool/msgpack_ext/types/interval.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh` & `tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/gen-timezones.sh`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/types/timezones/timezones.py` & `tarantool-1.1.0/tarantool/msgpack_ext/types/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/unpacker.py` & `tarantool-1.1.0/tarantool/msgpack_ext/unpacker.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/msgpack_ext/uuid.py` & `tarantool-1.1.0/tarantool/msgpack_ext/uuid.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/request.py` & `tarantool-1.1.0/tarantool/request.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/response.py` & `tarantool-1.1.0/tarantool/response.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/schema.py` & `tarantool-1.1.0/tarantool/schema.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/space.py` & `tarantool-1.1.0/tarantool/space.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/types.py` & `tarantool-1.1.0/tarantool/types.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool/utils.py` & `tarantool-1.1.0/tarantool/utils.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/tarantool.egg-info/PKG-INFO` & `tarantool-1.1.0/tarantool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarantool
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client library for Tarantool
 Home-page: https://github.com/tarantool/tarantool-python
 Author: tarantool-python AUTHORS
 Author-email: admin@tarantool.org
 License: BSD
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `tarantool-1.0.0/tarantool.egg-info/SOURCES.txt` & `tarantool-1.1.0/tarantool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/ca.crt` & `tarantool-1.1.0/test/data/ca.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/generate.sh` & `tarantool-1.1.0/test/data/generate.sh`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/invalidhost.crt` & `tarantool-1.1.0/test/data/invalidhost.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/localhost.crt` & `tarantool-1.1.0/test/data/localhost.crt`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/localhost.enc.key` & `tarantool-1.1.0/test/data/localhost.enc.key`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/data/localhost.key` & `tarantool-1.1.0/test/data/localhost.key`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/setup_command.py` & `tarantool-1.1.0/test/setup_command.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/__init__.py` & `tarantool-1.1.0/test/suites/__init__.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/crud_server.lua` & `tarantool-1.1.0/test/suites/crud_server.lua`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 #!/usr/bin/env tarantool
 
+local function replicaset_uuid()
+    if box.info().replicaset ~= nil and box.info().replicaset.uuid ~= nil then
+        return box.info().replicaset.uuid
+    end
+
+    return box.info().cluster.uuid
+end
+
 local function configure_crud_instance(primary_listen, crud, vshard)
     box.schema.create_space(
     'tester', {
     format = {
         {name = 'id', type = 'unsigned'},
         {name = 'bucket_id', type = 'unsigned'},
         {name = 'name', type = 'string'},
@@ -26,15 +34,15 @@
     box.once('guest', function()
         box.schema.user.grant('guest', 'super')
     end)
     local uri = 'guest@0.0.0.0:' .. primary_listen
     local cfg = {
         bucket_count = 300,
         sharding = {
-            [box.info().cluster.uuid] = {
+            [replicaset_uuid()] = {
                 replicas = {
                     [box.info().uuid] = {
                         uri = uri,
                         name = 'storage',
                         master = true,
                     },
                 },
```

### Comparing `tarantool-1.0.0/test/suites/lib/remote_tarantool_server.py` & `tarantool-1.1.0/test/suites/lib/remote_tarantool_server.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/lib/skip.py` & `tarantool-1.1.0/test/suites/lib/skip.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,14 +201,27 @@
     See https://github.com/tarantool/tarantool/issues/5941
     """
 
     return skip_or_run_test_pcall_require(func, 'datetime',
                                           'does not support datetime type')
 
 
+def skip_or_run_datetime_2_11_test(func):
+    """
+    Decorator to skip or run tests related to datetime module with
+    fixes introduced in 2.11 release.
+
+    See https://github.com/tarantool/tarantool/issues/7698 and
+    https://github.com/tarantool/tarantool/issues/7700
+    """
+
+    return skip_or_run_test_tarantool(func, '2.11.0',
+                                      'does not provide required datetime fixes')
+
+
 def skip_or_run_error_extra_info_test(func):
     """
     Decorator to skip or run tests related to extra error info
     provided over iproto depending on the tarantool version.
 
     Tarantool provides extra error info only since 2.4.1 version.
     See https://github.com/tarantool/tarantool/issues/4398
@@ -273,7 +286,23 @@
 
     Tarantool supports schema constraints only since 2.10.0 version.
     See https://github.com/tarantool/tarantool/issues/6436
     """
 
     return skip_or_run_test_tarantool(func, '2.10.0',
                                       'does not support schema constraints')
+
+
+def skip_or_run_iproto_basic_features_test(func):
+    """
+    Decorator to skip or run tests related to iproto ID requests,
+    protocol version and features.
+
+    Tarantool supports iproto ID requests only since 2.10.0 version.
+    Protocol version is 3 for Tarantool 2.10.0,
+    IPROTO_FEATURE_STREAMS, IPROTO_FEATURE_TRANSACTIONS
+    and IPROTO_FEATURE_ERROR_EXTENSION are supported in Tarantool 2.10.0.
+    See https://github.com/tarantool/tarantool/issues/6253
+    """
+
+    return skip_or_run_test_tarantool(func, '2.10.0',
+                                      'does not support iproto ID and iproto basic features')
```

### Comparing `tarantool-1.0.0/test/suites/lib/tarantool_admin.py` & `tarantool-1.1.0/test/suites/lib/tarantool_admin.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/lib/tarantool_python_ci.lua` & `tarantool-1.1.0/test/suites/lib/tarantool_python_ci.lua`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/lib/tarantool_server.py` & `tarantool-1.1.0/test/suites/lib/tarantool_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,15 +185,16 @@
                 ssl_key_file=None,
                 ssl_cert_file=None,
                 ssl_ca_file=None,
                 ssl_ciphers=None,
                 ssl_password=None,
                 ssl_password_file=None,
                 create_unix_socket=False,
-                auth_type=None):
+                auth_type=None,
+                sql_seq_scan_default=None):
         # pylint: disable=unused-argument
 
         if os.name == 'nt':
             return RemoteTarantoolServer()
         return super(TarantoolServer, cls).__new__(cls)
 
     def __init__(self,
@@ -201,15 +202,16 @@
                  ssl_key_file=None,
                  ssl_cert_file=None,
                  ssl_ca_file=None,
                  ssl_ciphers=None,
                  ssl_password=None,
                  ssl_password_file=None,
                  create_unix_socket=False,
-                 auth_type=None):
+                 auth_type=None,
+                 sql_seq_scan_default=None):
         # pylint: disable=consider-using-with
 
         os.popen('ulimit -c unlimited').close()
 
         if create_unix_socket:
             self.host = None
             self.args = {}
@@ -231,14 +233,15 @@
         self.ssl_key_file = ssl_key_file
         self.ssl_cert_file = ssl_cert_file
         self.ssl_ca_file = ssl_ca_file
         self.ssl_ciphers = ssl_ciphers
         self.ssl_password = ssl_password
         self.ssl_password_file = ssl_password_file
         self.auth_type = auth_type
+        self.sql_seq_scan_default = sql_seq_scan_default
         self._binary = None
         self._log_des = None
 
     def find_exe(self):
         """
         Find Tarantool executable.
         """
@@ -285,14 +288,16 @@
         admin_listen = self.generate_listen(self.args['admin'], True)
         os.putenv("LISTEN", primary_listen)
         os.putenv("ADMIN", admin_listen)
         if self.auth_type is not None:
             os.putenv("AUTH_TYPE", self.auth_type)
         else:
             os.putenv("AUTH_TYPE", "")
+        if self.sql_seq_scan_default is not None:
+            os.putenv("SQL_SEQ_SCAN_DEFAULT", self.sql_seq_scan_default)
 
     def prepare_args(self):
         """
         Prepare Tarantool server init.lua script.
         """
 
         return shlex.split(self.binary if not self.script else self.script_dst)
```

### Comparing `tarantool-1.0.0/test/suites/test_connection.py` & `tarantool-1.1.0/test/suites/test_connection.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_crud.py` & `tarantool-1.1.0/test/suites/test_crud.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_datetime.py` & `tarantool-1.1.0/test/suites/test_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import tarantool
 from tarantool.error import MsgpackError
 from tarantool.msgpack_ext.packer import default as packer_default
 from tarantool.msgpack_ext.unpacker import ext_hook as unpacker_ext_hook
 
 from .lib.tarantool_server import TarantoolServer
-from .lib.skip import skip_or_run_datetime_test
+from .lib.skip import skip_or_run_datetime_test, skip_or_run_datetime_2_11_test
 
 
 class TestSuiteDatetime(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         print(' DATETIME EXT TYPE '.center(70, '='), file=sys.stderr)
         print('-' * 70, file=sys.stderr)
@@ -377,29 +377,31 @@
             with self.subTest(msg=name):
                 self.assertSequenceEqual(self.con.call('sub', case['arg_1'], case['arg_2']),
                                          [case['res']])
 
     datetime_subtraction_different_timezones_case = {
         'arg_1': tarantool.Datetime(year=2001, month=2, day=3, tz='UTC'),
         'arg_2': tarantool.Datetime(year=2001, month=2, day=3, tz='MSK'),
-        'res': tarantool.Interval(day=1, hour=-21),
+        # Tarantool datetime comparison is naive, our tarantool.Interval comparison is naive too.
+        # So even though day=1, hour=-21 is the same as minute=180, test assertion fails.
+        'res_python': tarantool.Interval(day=1, hour=-21),
+        'res_tarantool': tarantool.Interval(minute=180),
     }
 
     def test_python_datetime_subtraction_different_timezones(self):
         case = self.datetime_subtraction_different_timezones_case
 
-        self.assertEqual(case['arg_1'] - case['arg_2'], case['res'])
+        self.assertEqual(case['arg_1'] - case['arg_2'], case['res_python'])
 
-    @skip_or_run_datetime_test
-    @unittest.skip('See https://github.com/tarantool/tarantool/issues/7698')
+    @skip_or_run_datetime_2_11_test
     def test_tarantool_datetime_subtraction_different_timezones(self):
         case = self.datetime_subtraction_different_timezones_case
 
         self.assertSequenceEqual(self.con.call('sub', case['arg_1'], case['arg_2']),
-                                 [case['res']])
+                                 [case['res_tarantool']])
 
     interval_arithmetic_cases = {
         'year': {
             'arg_1': tarantool.Datetime(year=2008, month=2, day=3),
             'arg_2': tarantool.Interval(year=1),
             'res_add': tarantool.Datetime(year=2009, month=2, day=3),
             'res_sub': tarantool.Datetime(year=2007, month=2, day=3),
@@ -511,16 +513,15 @@
     }
 
     def test_python_datetime_addition_winter_time_switch(self):
         case = self.datetime_addition_winter_time_switch_case
 
         self.assertEqual(case['arg_1'] + case['arg_2'], case['res'])
 
-    @skip_or_run_datetime_test
-    @unittest.skip('See https://github.com/tarantool/tarantool/issues/7700')
+    @skip_or_run_datetime_2_11_test
     def test_tarantool_datetime_addition_winter_time_switch(self):
         case = self.datetime_addition_winter_time_switch_case
 
         self.assertSequenceEqual(self.con.call('add', case['arg_1'], case['arg_2']),
                                  [case['res']])
 
     @skip_or_run_datetime_test
```

### Comparing `tarantool-1.0.0/test/suites/test_dbapi.py` & `tarantool-1.1.0/test/suites/test_dbapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     ddl2 = f'create table {table_prefix}barflys (name varchar(20) primary key, ' \
            'drink varchar(30))'
 
     @classmethod
     def setUpClass(cls):
         print(' DBAPI '.center(70, '='), file=sys.stderr)
         print('-' * 70, file=sys.stderr)
-        cls.srv = TarantoolServer()
+        # Select scans are not allowed with compat.sql_seq_scan_default = "new",
+        # but tests create cursors with fullscan.
+        cls.srv = TarantoolServer(sql_seq_scan_default="old")
         cls.srv.script = 'test/suites/box.lua'
         cls.srv.start()
         cls.con = tarantool.Connection(cls.srv.host, cls.srv.args['primary'])
         cls.driver = dbapi
         cls.connect_kw_args = {
             "host": cls.srv.host,
             "port": cls.srv.args['primary']
```

### Comparing `tarantool-1.0.0/test/suites/test_decimal.py` & `tarantool-1.1.0/test/suites/test_decimal.py`

 * *Files 14% similar despite different names*

```diff
@@ -222,14 +222,47 @@
         },
         'decimal_limits_12': {
             'python': decimal.Decimal('-1234567891234567890.0987654321987654321'),
             'msgpack': (b'\x13\x01\x23\x45\x67\x89\x12\x34\x56\x78\x90'
                         b'\x09\x87\x65\x43\x21\x98\x76\x54\x32\x1d'),
             'tarantool': "decimal.new('-1234567891234567890.0987654321987654321')",
         },
+        'decimal_exponent_1': {
+            'python': decimal.Decimal('1e33'),
+            'msgpack': (b'\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+                        b'\x00\x00\x00\x00\x00\x00\x00\x0c'),
+            'tarantool': "decimal.new('1e33')",
+        },
+        'decimal_exponent_2': {
+            'python': decimal.Decimal('1.2345e33'),
+            'msgpack': (b'\x00\x01\x23\x45\x00\x00\x00\x00\x00\x00\x00'
+                        b'\x00\x00\x00\x00\x00\x00\x00\x0c'),
+            'tarantool': "decimal.new('1.2345e33')",
+        },
+        'decimal_exponent_3': {
+            'python': decimal.Decimal('1.2345e2'),
+            'msgpack': (b'\x02\x12\x34\x5c'),
+            'tarantool': "decimal.new('1.2345e2')",
+        },
+        'decimal_exponent_4': {
+            'python': decimal.Decimal('1.2345e4'),
+            'msgpack': (b'\x00\x12\x34\x5c'),
+            'tarantool': "decimal.new('1.2345e4')",
+        },
+        'decimal_exponent_5': {
+            'python': decimal.Decimal('-1e33'),
+            'msgpack': (b'\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00'
+                        b'\x00\x00\x00\x00\x00\x00\x00\x0d'),
+            'tarantool': "decimal.new('-1e33')",
+        },
+        'decimal_exponent_6': {
+            'python': decimal.Decimal('1e-33'),
+            'msgpack': (b'\x21\x1c'),
+            'tarantool': "decimal.new('1e-33')",
+        },
     }
 
     def test_msgpack_decode(self):
         for name, case in self.valid_cases.items():
             with self.subTest(msg=name):
                 self.assertEqual(unpacker_ext_hook(1, case['msgpack']),
                                  case['python'])
```

### Comparing `tarantool-1.0.0/test/suites/test_dml.py` & `tarantool-1.1.0/test/suites/test_dml.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_encoding.py` & `tarantool-1.1.0/test/suites/test_encoding.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_error_ext.py` & `tarantool-1.1.0/test/suites/test_error_ext.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_execute.py` & `tarantool-1.1.0/test/suites/test_execute.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_interval.py` & `tarantool-1.1.0/test/suites/test_interval.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_mesh.py` & `tarantool-1.1.0/test/suites/test_mesh.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_package.py` & `tarantool-1.1.0/test/suites/test_package.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_pool.py` & `tarantool-1.1.0/test/suites/test_pool.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_push.py` & `tarantool-1.1.0/test/suites/test_push.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_reconnect.py` & `tarantool-1.1.0/test/suites/test_reconnect.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_schema.py` & `tarantool-1.1.0/test/suites/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,18 +450,29 @@
             },
         },
     }
 
     def _run_test_schema_fetch_disable(self, con, mode=None):
         # Enable SQL test case for tarantool 2.* and higher.
         if int(str(self.srv.admin.tnt_version)[0]) > 1:
-            self.testing_methods['available']['execute'] = {
-                'input': ['SELECT * FROM "tester"'],
-                'output': [[1, None]],
-            }
+            if self.srv.admin.tnt_version >= pkg_resources.parse_version('2.11.0'):
+                # SEQSCAN keyword is explicitly allowing to use seqscan
+                # https://github.com/tarantool/tarantool/commit/77648827326ad268ec0ffbcd620c2371b65ef2b4
+                # It was introduced in 2.11.0-rc1. If compat.sql_seq_scan_default
+                # set to "new" (default value since 3.0), returns error
+                # if trying to scan without keyword.
+                self.testing_methods['available']['execute'] = {
+                    'input': ['SELECT * FROM SEQSCAN "tester"'],
+                    'output': [[1, None]],
+                }
+            else:
+                self.testing_methods['available']['execute'] = {
+                    'input': ['SELECT * FROM "tester"'],
+                    'output': [[1, None]],
+                }
 
         # Testing the schemaless connection with methods
         # that should NOT be available.
         if mode is not None:
             for addr in con.pool.keys():
                 self.assertEqual(con.pool[addr].conn.schema_version, 0)
                 self.assertEqual(con.pool[addr].conn.schema, None)
```

### Comparing `tarantool-1.0.0/test/suites/test_ssl.py` & `tarantool-1.1.0/test/suites/test_ssl.py`

 * *Files identical despite different names*

### Comparing `tarantool-1.0.0/test/suites/test_uuid.py` & `tarantool-1.1.0/test/suites/test_uuid.py`

 * *Files identical despite different names*

